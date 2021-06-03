# Allen's Notes for KDB+ / Q
<a name="top"></a>


# q-SQL
1. [Select from where](#select_from_where)
2. [Select by](#select_by)
3. [Select count](#select_count)
4. [Using operations and functions](#using_ops_functions)
5. [In function](#in_function)
6. [Within function](#within_function)
7. [xbar function](#xbar_function)
# [q-SQL Problem Set](#qsql_problem_set)


<a name="select_from_where"></a>
### Select from where

Load the trades.q script first

```q
\l trades.q
```
General Rules
* column =
* sym=`A 
* cond="A"
* .z.d means today
* use comma , for multiple expressions
* put most restrictive clause first, starting from left (saves time)

```q
select from trade where date=20121.05.29, sym=`A
```

date | time | sym |price | size | cond
-|-|-|-|-|-
2021-05-29|	09:30:02.758|	A|	100.35004081670195 |	50300|	B
2021-05-29|	09:30:17.997|	A |	57.81544134486467 |	65600	|C
2021-05-29|	09:30:21.507|	A	|97.85912833176553 |	51800|	B

```q
select price from trade where date=2021.05.29, sym=`A
```

price|
-|
100.3 |
57.8 |
97.8 |

```q
select max price from trade where date=2021.05.29, sym=`A
```

price |
-|
109.99|

```q
count select from trade where cond="A"
```
211597

```q
select by sym from trade where date=.z.d
```
* by sym = will set sym as the key and agg all dates with the same sym
* since select + blank , KDB will auto select last entry in column

sym|date|time|price|size|cond
-|-|-|-|-|-|
A	|2021-06-02	|17:29:57.306	|87.54 |	49100 |	B
AA|	2021-06-02|	17:29:58.789 |	68.09 |	88100	|A
AAPL|	2021-06-02|	17:29:58.262 |	76.18	|22500	|A

(sym is a keyed col)

<a name="select_by"></a>
### Select By

```q
select first price, first time by date from trade where sym=`AAPL
```
* select = return column of values
* by date = sets date as the key column


date|price|time
-|-|-
2021-05-29|	78.6 |	09:30:03.025
2021-05-30|	60.8 |	09:30:02.686
2021-05-31|	55.1 | 09:30:18.274

(date is a keyed col)

```q
select open:first price, high:max price, low:min price, close:last price by date from trade where sym=`AAPL
```
* open: renames the column

date|open|high|low|close
-|-|-|-|-
2021-05-29|	78.66|	109.91 |	50.5 |	68.01
2021-05-30|	60.88	|109.98	| 50.0	| 90.49

(date is a keyed col )


<a name="select_count"></a>
### Select Count 

```q
select count i, max prirce by date, time.hh from trade where sym=`RBS
```
date|hh|x|prrice
-|-|-|-
2021-05-29|	9|	645 |	50.5 
2021-05-30|	10	|154	| 50.0

* i is a virtual column that returns the number of rows (as column x)


<a name="using_ops_functions"></a>
### Using Operations and Functions 

```q
select price by date from trade where sym=`AAPL, price < avg price
```
* finds all AAPL prices that are less than the avg price grouped by date

date|price
-|-
2021-05-29| 100 99 22 33
2021-05-30| 23 199 44 12

(date is a keyed column)

```q
select price by date=.z.d from trade where sym=`AAPL, price < avg price
```
* retrieve prices, keyed by TODAY, where AAPL's price is less than the avg price
* grouped by today; 0 = false, 1 = true

d | price
-|-
0 | 23 52 63
1 | 23 66 12

(d is a keyed column)

```q
select {x % max x} price by date = .z.d from trade where sym=`AApl, price < avg price
```
* retrieve price / max price, keyed by today, where the price is less than the avg price

d | price
-|-
0b | 0.98 0.7 0.8
1b | 0.12 0.43 0.32

(d is a keyed column)

<a name="in_function"></a>
### In Function

```q
select from trade where sym in `AAPL`RBS
```
* in function checks if every LHS argument occurs anywhere in RHS argument (AAPL or RBS)
* a faster way of checking "or" arguments

date|time|sym|price|size|cond
-|-|-|-|-|-
2021-05-30|	09:30:02.743 |	RBS |	97.113	| 80700 |	C
2021-05-30|	09:30:03.025 |	AAPL |	78.66 |	19000	| A

<a name="within_function"></a>
### Within Function

```q
select from trade where sym=`RBS, price within 95 100
```
* checks if LHS argument is within the range on RHS argument
* has to have lower + upper bind

date|time|sym|price|size|cond
-|-|-|-|-|-
2021-05-30|	09:30:02.743 |	RBS |	97.113	| 80700 |	C
2021-05-30|	09:30:03.025 |	AAPL |	98.66 |	19000	| A

```q
select from trade where sym=`RBS, price within 95 100, time within 11:30 12:00
```
* 2 within filters, price and time

date|time|sym|price|size|cond
-|-|-|-|-|-
2021-05-30|	11:40:02.743 |	RBS |	97.113	| 80700 |	C
2021-05-30|	11:44:03.025 |	AAPL |	98.66 |	19000	| A

<a name="xbar_function"></a>
### Xbar Function
* xbar allows for custom sized boundaries

```q
select count i, max price by date, xbar [15*60*1000;time] from trade where sym=`RBS
```
* retrieve number of trades (count) and max price, keyed by date and time 
* 15 mins x 60 sec x 1000 ms to get to milliseconds
* xbar rounds its 2nd argument to nearest multiple of first argument (so rounds time to 15 mins)

date|time|x|price
-|-|-|-
2021-05-30|	11:40:02.743 |	100 |	97.113
2021-05-30|	11:44:03.025 |	123 |	98.66 

(date and time are keyed columns)

<a name="qsql_problem_set"></a>
# q-SQL Problem Set
[Top](#top)

**1. Extract from trade table, trades for MS greater than 1,000 in size**

```q
select from trade where sym=`MS, size >1000
```

dt|sym|price|size
-|-|-|-
2021.01.01 | MS |225 | 200
2021.01.01 | MS |234 | 400

* multiple where expressions separated by commas
* sym has to be back tick MS
<hr>

**2. From the trade table, find the total size of all trades and the average price paid per sym**

```q
select total: sum size, avg price by sym from trade
```

sym|total | price
-|-|-
AAPL | 320 | 1015
C | 310 | 100
MS | 740 | 234

* "price paid per sym" = we need to set sym as a keyed colummn (by sym)
* select + conditions = columns retrieved
* total: renames column, sum size = sums sizes together
* avg price = retains the price column header, just averages prices

<hr>

**3. From the trade table, find the trade that was largest size for each sym**

```q
select from (update mx:max size by sym from trade) where size = mx
```

date|time|sym|price|size|cond|mx
-|-|-|-|-|-|-
2021-05-30|	09:30:21.256|	B	|100.04|	99900	| 	|99900
2021-05-30|	09:31:20.975	|AA|	67.30|	99900|	C|	99900
2021-05-30|	09:43:47.816	|GOOG|	72.42|	99900|	A|	99900

* add new column mx which is the max size by sym
* where size = filter size to max size
* this is using a nested query to filter only the max size for their sym

Alternative solution

```q
select from trade where size=(max;size) fby sym
```

date|time|sym|price|size|cond
-|-|-|-|-|-
2021-05-30|	09:30:21.256|	B|	100.04 |	99900|	 
2021-05-30|	09:31:20.975|	AA|	67.30	|99900|	C
2021-05-30|	09:43:47.816|	GOOG|	72.42	|99900|	A
2021-05-30|	09:46:44.690|	F	|73.22	|99900|	B

* fby = allows performing filters on agg queries
* fby has to go at the end of your query

<hr>

**4. From the trade table, select the latest trade for each sym, and include all details**

```q
select last date, last price, last size by sym from trade
```
sym|date|price|size
-|-|-|-
A|	2021-06-03|	87.54| 49100
AA|	2021-06-03|	68.09| 88100


Alternative Solution

```q
select by sym from trade
```
sym|date|price|size|cond
-|-|-|-|-
AMZN|	2021-06-03|	87.54| 49100 | B
AAPL|	2021-06-03|	87.54| 49100 | C

* table is already sorted by time, KDB is based on ordered lists

<hr>

**5. Find all trades that have sym GOOG**

```q
select from trade where sym=`GOOG
```
sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	87.54| 49100 | B
GOOG|	2021-06-03|	87.54| 49100 | C

<hr>

**6. Find all trades that have sym GOOG or RBS or A**

```q
select from trade where sym in `GOOG`RBS`A
```
sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	87.54| 49100 | B
RBS|	2021-06-03|	87.54| 49100 | C
A|	2021-06-03|	87.54| 49100 | C

<hr>

**7. Find all trades for google that had a price between 70 and 80**

```q
select from trade where sym=`GOOG, price within 70 80
```

sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	72 | 49100 | B
GOOG|	2021-06-03|	75| 49100 | C
GOOG|	2021-06-03|	78 | 49100 | C

<hr>

**8. Count the number of trades and total size of trades per hour for sym RBS**

```q
select NumberTrades: count i, totalSize: sum size by time.hh from trade where sym=`RBS
```
hh|NumberTrades|totalSize
-|-|-
9|	3186|	159063500
10|	6544|	321195100
11|	6280|	315284200

* NumberTrades + TotalSize = new column names
* count i = virtual column. Counts agg number of horizontal rows
* by time.hh = sets hour as the key column and groups results by hour
* sum size = gives you total size

<hr>

**9. Select the number of trades and total size of trades every 30 mins for the sym RBS**

```q
select numbertrades: count i, totalsize: sum size by 30 xbar time.minute from trade where sym=`RBS
```

minute|numbertrades|totalsize
-|-|-
09:30|	3186|	159063500
10:00|	3271|	162197000
10:30|	3273|	158998100

* 30 xbar time.minute = rounds minutes by 30; groups together and is set as key

