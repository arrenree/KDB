# Allen's Notes for KDB+ / Q
<a name="top"></a>


## [Tables](#tables_header)
1. [Flipping Dictionary to Table](#dict_to_table)
2. [Simple Table](#simple_table)
3. [Single Row Table](#single_row_table)
4. [Mixed Table](#mixed_table)
5. [Meta / Data Type Table](#meta_datatypes_table)
6. [Count Row Table](#countrowsimple_table)
7. [Rename Column Table](#rename_column_table)
8. [Add Column Table](#add_column_table)
9. [Sort Column Table](#sort_column_table)
10. [Union Table](#union_table)
11. [Except Table](#except_table)
12. [Inter Table](#inter_table)
13. [Distinct Table](#distinct_table)
14. [Retrieve From Table](#retrieve_table)
15. [Insert Table](#insert_table)

## [Tables Problem Set](#tables_problem_set)

## [Keyed Tables](#keyed_tables)
1. [Single Keyed Table](#single_keyed_table)
2. [Multi_Keyed_Table](#multi_keyed_table)
3. [Retrieving Keys/Values](#retrieving_keysvalues)
4. [Changing Keys](#changing_keys)
5. [Adding Keys](#adding_keys)
6. [Removing Keys](#removing_keys)
7. [Upsert Keys](#upsert_keys)
8. [Upsert Multi Row/Keys](#upsert_multi_rowkeys)
9. [Retrieving Values from Keyed Table](#retrieve_value_keys)

## [Keyed Table Problem Set](#keyed_table_problem_set)

## [qSQL](#qsql_header)
1. [Select from where](#select_from_where)
2. [Select by](#select_by)
3. [Select count](#select_count)
4. [Using operations and functions](#using_ops_functions)
5. [In function](#in_function)
6. [Within function](#within_function)
7. [xbar function](#xbar_function)
8. [Exec query](#exec)
9. [Update](#update_statement)
10. [Delete columns](#delete_columns)
11. [Delete rows](#delete_rows)
12. [Sort Ascending / Descending](#sort_asc_desc)
13. [Renaming / Reordering Columns](#rename_reorder_columns)

## [q-SQL Problem Set](#qsql_problem_set)





<hr>

<a name="tables_header"></a>
## Tables
[Top](#top)

<a name="dict_to_table"></a>
### Flipping Dictionary to Table

```q
d: `company`employees`! (`ford`bmw; 300 100)
```
key|Value
-|-
company	|`ford`bmw
employees|	300 100

* dictionary d

```q
flip d
```
company | employees
-|-
ford |	300
bmw	| 100

* when you flip a dictionary, you get a table

<a name="simple_table"></a>
### Simple Table

```q
( [] company: `ford`bmw; employees: 300 100)
```
company | employees
-|-
ford |	300
bmw	| 100

* have to define a table within parathesis ( )
* tables must have [] which are for key columns
* semi colon ; separates next column

<a name="single_row_table"></a>
### Single Row Table

```q
( [] company: enlist `ford; employees: enlist 300)
```
company | employees
-|-
ford |	300

* have to use enlist for atoms and single row tables

<a name="mixed_table"></a>
### Mixed Table

```q
( [] syms:`a`b`c; floats: 1.1 2.2 3.3; strings: ("bob"; "jim"; "john"))
```
syms|floats|strings
-|-|-
a|	1.1 |	bob
b|	2.2	|jim
c|	3.3	|john

* syms have to have backtick+sym
* strings have to enclose within (" ")

<a name="meta_datatypes_table"></a>
### Meta / Data Type Table

* meta returns a table where each row is a column

```q
( [] company:(); employees:() )
meta t
```
c|t|f|a
-|-|-|-
company|	|	|
employees|	|	|

* create empty table with no types
* t = type (s = symbol, j = long)
* f = foreign key
* a = attributes

```q
( [] company: `symbol$(); employees: `int$())
```
c|t|f|a
-|-|-|-
company|	s	|	|
employees|	j	|	|

* changed type to s symbol and i integer

<a name="countrowsimple_table"></a>
### Count Row Table

Given:

company | employees
-|-
ford |	300
bmw	| 100

```q
count t
```
2

* returns number of rows in table

```q
cols t
```
`company`employee

* returns symbol list of columns

<a name="rename_column_table"></a>
### Rename Column Table xcol

```q
`a`b xcol t
```

a | b
-|-
ford |	300
bmw	| 100

<a name="add_column_table"></a>
### Add Column Table

```q
select company, employees, newval: 101 from t
```
company | employees | newval
-|-|-
ford |	300 | 101
bmw	| 100 | 101

* select will retrieve columns as values
* if you select a column that doesnt exist, it will add it (newval)

<a name="sort_column_table"></a>
### Sort Column Table (xasc)

```q
`employees xasc t
```
company | employees | newval
-|-|-
bmw	| 100 | 101
ford |	300 | 101

* will sort ascending by employees

<a name="union_table"></a>
### Union Table

Given

table t

company | employees
-|-
ferrari| 100
ford |	100 
rover| 100

table t

company | employees
-|-
ferrari| 100
bmw |	5 
ford| 5

```q
t union u
```
company | employees
-|-
ferrari| 100
ford | 100 
rover| 100
bmw |	5 
ford| 5

* returns values that are same (ferrari 100). does not dupe same values.
* any values that do NOT equal, adds as new row

<a name="except_table"></a>
### Except Table

```q
t except u
```
company | employees
-|-
ford| 100
rover | 100 

* checks for any matches, and removes them (ferrari 100)
* returns remaining rows in table t

<a name="inter_table"></a>
### Inter Table

```q
t inter u
```
company | employees
-|-
ferrari| 100

* only returns rows that match

<a name="distinct_table"></a>
### Distinct Table

```q
([] a: 1 1 2; b: 1 1 3)
```
a|b
-|-
1|	1
1	|1
2	|3

```q
distinct ([] a: 1 1 2; b: 1 1 3)
```
a|b
-|-
1|	1
2	|3

* will return distinct values per row

<a name="retrieve_table"></a>
### Retrieve From Table

Given

company | employees
-|-
ferrari| 100
ford | 100 
rover| 100
bmw |	5 
ford| 5

```q
select from t
```
company | employees
-|-
ferrari| 100
ford | 100 
rover| 100
bmw |	5 
ford| 5

* retrieves all columns from table t

```q
select company from t
```

company | 
-|
ferrari| 
ford |  
rover| 
bmw |	 
ford| 

* only retrieves the company column

```q
select from t where company = `ford
```

company | employees
-|-
ford | 100 

* retrieves rows that meet the specific where requirement (ford)

```q
t [`employees]
```
100 100 100 5 5 

* retrieves column= employee as a row

```q
t [`employees] - : 100
```
company | employees
-|-
ferrari| 0
ford | 0 
rover| 0
bmw |	-105 
ford| -105

* you can manipulate all the values in a column (employees)

```q
t [ 0 1]
```
company | employees
-|-
ferrari| 0
ford | 0 

* returns first 2 rows

alternatively

```q
2#t
```

```q
-3#t
```

company | employees
-|-
rover| 0
bmw |	-105 
ford| -105

* returns last 3 rows 

```q
2 ? t
```

company | employees
-|-
rover| 0
ford| -105

* randomly select 2 from table

<a name="insert_table"></a>
### Insert Table

```q
t: ( [] company: (); employees: () )
```
company|employees
-|-

* empty table

```q
insert [`t; (`Ferrari; 8)]
```
company|employees
-|-
Ferrari | 8

* backtick t to update underlying table
* first argument is table name, second argument are the values to be inserted
* semi colon separate columns for the values

```q
insert [`t; (Ferrari`bmw; 9 7)]
```
company|employees
-|-
Ferrari | 8
Ferrari | 9
bmw | 7

* insert will append to the table each time (ferrari repeated)

```q
x: ( [] company: `Subaru`Hyundai; employees: 55 56)
```
company|employees
-|-
Subaru | 55
Hyundai | 56

```q
`t insert x
```
company|employees
-|-
Ferrari | 8
Ferrari | 9
bmw | 7
Subaru | 8
Hyundai | 56

* table x inserted into table t

alternatively:
```q
t:t,x
```
<hr>

<a name="tables_problem_set"></a>
# Tables Problem Set
[Top](#top)

**1. Given:**

```q
stock: ( [] sym: `MS`C`AAPL; sector:`Financial`Financial`Tech; employees: 100 100 100)
```
sym|sector|employees
-|-|-
MS	|Financial|	100
C	|Financial	|100
AAPL|	Tech	|100

**1. Extract the employees numbers (without the header)**

```q
stock [ ; `employees]
```

```q
stock[`employees]
```

```q
stock.employees
```

```q
stock`employees
```
100

<hr>

**2. Key the first column in stock table (above)**

```q
1!stock
```

sym|sector|employees
-|-|-
MS	|Financial|	100
C	|Financial	|100
AAPL|	Tech	|100

* you can't tell cuz of formatting, but sym is now keyed

<hr>

**3. Display only the first and second rows of the stock table**

```q
2#stock
```
or

```q
stock [0 1]
```
sym|sector|employees
-|-|-
MS	|Financial|	100
C	|Financial	|100

<hr>

**4. Select the last row of stock table as a dictionary**

```q
last stock
```
key |value
-|-
sym |`AAPL
sector | `Tech
employees | 100

<hr>

**5. Insert GOOG in the tech sector with 100 employees**

```q
insert [`stock; ([] sym: enlist `GOOG; sector: enlist `tech; employees: enlist 100)]
```
sym|sector|employees
-|-|-
MS	|Financial|	100
C	|Financial	|100
AAPL|	Tech	|100
GOOG | Tech | 100

* syntax is insert + [table name; table with corresponding columns]
* must use enlist when adding single row!!

<hr>

**6. Given:**

```q
boss: ( [] name:`bob`bill`belinda; height: 188 186 174)
employees: ( [] name:`jim`jane`john; height: 180 160 170)
```
boss:
name|height
-|-
bob|	188
bill |	186
belinda |174

employees:

name|height
-|-
jim|	180
jane|	160
john|	170

**6. Find the average height of the bosses, the employees, and both the bosses and employees**

```q
avg boss `height
```
182.667

```q
avg employees `height
```
170f

```q
avg (employees, boss) `height
```
176.33

* joins the 2 tables together
* calculate the average height from joined table

<hr>

**7. Find the 2 tallest employees**
```q
2#`height xdesc employees
```
name|height
-|-
jim	|180
john|	170

* take 2 from employees table, sorted descending by height

<hr>

**8. Given the 2 tables:**

```q
stock: ( [sym:`MS`C`AAPL] sector:`Fin`Fin`Tech; employees: 100 100 100)
trade: ( [] dt: 2021.01.01+til 5; sym:`C`C`MS`C`AAPL; price: 10 20 30 40 50; size: 100 200 300 400 500)
```
stock:
sym|sector|employees
-|-|-
MS|	Fin|	100
C	|Fin	|100
AAPL	|Tech|	100

trade:
dt|sym|price|size
-|-|-|-
2021-01-01|	C	|10	|100
2021-01-02|	C	|20	|200
2021-01-03|	MS|	30|	300
2021-01-04|	C	|40	|400
2021-01-05|	AAPL	|50|	500

**8. Insert the following rows into trade table**
dt|sym|price|size
-|-|-|-
2021-11-01|	JPM	|1	|100
2021-11-02|	UBS	|2	|200

```q
`trade insert( [] dt:2021.11.01+1 ; sym:`JPM`UBS; price:1 2; size: 100 200) 
```
or
```q
insert [`trade; ([] dt:2021.11.01+1 ; sym:`JPM`UBS; price:1 2; size: 100 200)]
```
dt|sym|price|size
-|-|-|-
2021-01-01|	C	|10	|100
2021-01-02|	C	|20	|200
2021-01-03|	MS|	30|	300
2021-01-04|	C	|40	|400
2021-01-05|	AAPL	|50|	500
2021-11-01|	JPM	|1	|100
2021-11-02|	UBS	|2	|200

* have to use backtick table in order to amend the underly table

<hr>

**9. Insert the following record into stock**
sym|sector|employees
-|-|-
FB|	Tech|	100

```q
`stock insert [`FB; `Tech; 100]
```
sym|sector|employees
-|-|-
MS|	Fin|	100
C	|Fin	|100
AAPL	|Tech|	100
FB | Tech | 100

* table name + insert (value1, value 2, value 3)

<hr>

**10. In the stock table, change the number of employees for C to 300**

```q
stock upsert (`C;`Fin;300)
```
or
```q
stock upsert ([sym: enlist`C] employees: enlist 300)
```
sym|sector|employees
-|-|-
C	|Fin	|300

* have to use enlist to create a vector for an atom

**11. Sort the stock table by sym**

```q
`sym xasc `stock
```
sym|sector|employees
-|-|-
AAPL|	Tech|	100
C	|Fin|	100
MS|	Fin|	100

* `column name + xasc + `table name

<hr>

<a name="keyed_tables"></a>
## Keyed Tables
[Top](#top)

<a name="single_keyed_table"></a>
### Single Keyed Table

```q
( [id: `a`b`c`e] name:`jane`jim`kim`john; employer:`citi`citi`ms`ts; age: 11 22 33 44)
```
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	john|	ts|	15

* the [ ] square bracket holds the key columns

<a name="multi_keyed_table"></a>
### Multi Keyed Table

```q
kt: ( [id:`a`b`c`d; name:`jane`jim`kim`john] employer:`citi`citi`ms`ts; age: 11 22 33 44)
```

id|name|employer|age
-|-|-|-
`a`|	`jane`|	citi|	11
`b`|	`jim`|	citi|	22
`c`|	`kim`|	ms|	13
`e`|	`john`|	ts|	15

<a name="retrieving_keysvalues"></a>
### Retrieving Keys/Values
```q
key kt
```
id|name
-|-
a	|jane
b	|jim
c	|kim
d	|john

*retrieves key columns

```q
value kt
```
employer|age
-|-
citi|	11
citi|	22
ms|	33
ts|	44

<a name="changing_keys"></a>
### Changing Keys
Table kt
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	john|	ts|	15

* id column is keyed

```q
`id`name xkey `kt
```
id|name|employer|age
-|-|-|-
`a`|	`jane`|	citi|	11
`b`|	`jim`|	citi|	22
`c`|	`kim`|	ms|	13
`e`|	`john`|	ts|	15

* changed key columns to both id and name
* use backtick kt to change underlying table

<a name="adding_keys"></a>
### Adding Keys
```q
1!kt
```
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	john|	ts|	15

<a name="removing_keys"></a>
### Removing Keys
```q
() xkey `kt
```
or
```q
0!kt
```
id|name|employer|age
-|-|-|-
a|	jane|	citi|	11
b|	jim|	citi|	22
c|	kim|	ms|	13
e|	john|	ts|	15

<a name="upsert_keys"></a>
### Upserting Keys
Given
```q
nd: ( [id:`e`f] name:`dan`kate; employer:`walmart`walmart; age:200 200)
```
id|name|employer|age
-|-|-|-
`e`|	dan|	walmart|	200
`f`|	kate|	walmart|	200

```q
upsert[`kt;nd]
```
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	dan|	walmart|	200
`f`|	kate|	walmart|	200

* if key exists and matches, updates value
* if new key, adds new row
* since key e already exists, overrides values for name, employer, age
* must make sure underlying keyed columns match, otherwise error. (1 keyed col vs 2 keyed col)

```q
upsert [`kt; ( [id:`f`g] name:`ron`allen)]
```
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	dan|	walmart|	200
`f`|	ron|	walmart|	200
`g`|	allen|	|	

* f was updated to ron, and since no employer or age info, pulled from existing kt table (kate's old row)
* g is new key, so adds new row. since no info, returns null

<a name="upsert_multi_rowkeys"></a>
### Upserting Multi Rows/Keys
Given:
```q
et: ([employer:`kx`ms`ms; loc:`NY`NY`HK] size: 10 20 30; area: 1 2 3)
```
employer|loc|size|area
-|-|-|-
`kx`|	`NY`|	10|	1
`ms`|	`NY`|	20|	2
`ms`|	`HK`|	30|	3

```q
upsert [et; ([employer:`kx`ms; loc:`NY`SG] size: 9 10)]
```
employer|loc|size|area
-|-|-|-
`kx`|	`NY`|	9|	1
`ms`|	`NY`|	20|	2
`ms`|	`HK`|	30|	3
`ms`|	`SG`|	10|	

* updated kx, NY to 9 (overrides prev value)
* since there was no ms, SG, adds new row 

<a name="retrieve_value_keys"></a>
### Retrieving Values from Keyed Table
Given:
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	33
`d`|	john|	ts|	44
`e`|	dan|	walmart|	200

```q
kt ( [] id:`a`b)
```
name|employer|age
-|-|-
jane|	citi|	11
jim|	citi|	22

* retrieves rows based on the values in column id (a and b)
or
```q
( [] id:`a`b) # kt)
```
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22

* uses the #take function to lookup values in column id
* notice it also returns the key column (id)

Given:
Table et
employer|loc|size|area
-|-|-|-
`kx`|	`NY`|	10|	1
`ms`|	`NY`|	20|	2
`ms`|	`HK`|	30|	3

```q
et`ms`HK
```
key|value
-|-
size|30
area|3

* will lookup the keys ms and HK and return the values

```q
et(`ms`HK; `kx`NY)
```

size|area 
-|-
30|3
10|1

* looks up values for both ms+HK (returns 30 and 3) and kx+NY (returns 10 and 1)

<hr>

<a name="keyed_table_problem_set"></a>
## Keyed Tables Problem Set
[Top](#top)







<hr>

<a name="qsql_header"></a>
## qSQL
[Top](#top)

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
`A`	|2021-06-02	|17:29:57.306	|87.54 |	49100 |	B
`AA`|	2021-06-02|	17:29:58.789 |	68.09 |	88100	|A
`AAPL`|	2021-06-02|	17:29:58.262 |	76.18	|22500	|A

<a name="select_by"></a>
### Select By

```q
select first price, first time by date from trade where sym=`AAPL
```
* select = return column of values
* by date = sets date as the key column


date|price|time
-|-|-
`2021-05-29`|	78.6 |	09:30:03.025
`2021-05-30`|	60.8 |	09:30:02.686
`2021-05-31`|	55.1 | 09:30:18.274

```q
select open:first price, high:max price, low:min price, close:last price by date from trade where sym=`AAPL
```
* open: renames the column

date|open|high|low|close
-|-|-|-|-
`2021-05-29`|	78.66|	109.91 |	50.5 |	68.01
`2021-05-30`|	60.88	|109.98	| 50.0	| 90.49

<a name="select_count"></a>
### Select Count 

```q
select count i, max prirce by date, time.hh from trade where sym=`RBS
```
date|hh|x|prrice
-|-|-|-
`2021-05-29`|	`9`|	645 |	50.5 
`2021-05-30`|	`10`	|154	| 50.0

* i is a virtual column that returns the number of rows (as column x)

<a name="using_ops_functions"></a>
### Using Operations and Functions 

```q
select price by date from trade where sym=`AAPL, price < avg price
```
* finds all AAPL prices that are less than the avg price grouped by date

date|price
-|-
`2021-05-29`| 100 99 22 33
`2021-05-30`| 23 199 44 12

```q
select price by date=.z.d from trade where sym=`AAPL, price < avg price
```
* retrieve prices, keyed by TODAY, where AAPL's price is less than the avg price
* grouped by today; 0 = false, 1 = true

d | price
-|-
`0` | 23 52 63
`1`| 23 66 12

```q
select {x % max x} price by date = .z.d from trade where sym=`AApl, price < avg price
```
* retrieve price / max price, keyed by today, where the price is less than the avg price

d | price
-|-
`0b` | 0.98 0.7 0.8
`1b` | 0.12 0.43 0.32

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
`2021-05-30`|	`11:40:02.743` |	100 |	97.113
`2021-05-30`|	`11:44:03.025` |	123 |	98.66 

<a name="exec"></a>
### Exec Query

```q
exec price from trade where date=.z.d, sym=`AAPL
```
62 59 13

* exec = single list returned

```q
select price from trade where date=.z.d, sym=`AAPL
```
price|
-|
62|
59|
13|

* select = single column returned

```q
exec first price from trade where date=.z.d, sym=`AAPL
```
62

```q
exec price by sym from trade where date=.z.d, sym=`AAPL
```
AAPL | 62 59 13

* retrieve price as values and specify the where expressions (date and sym)
* sets sym as keys

```q
exec price by sym from trade where date=.z.d
```
sym| price
-|-
`A` | 108 77 88
`AA`| 33 45 23
`AAPL`| 34 56 23

```q
exec first price by sym, cond from trade where date=.z.d, sym in `KX`AAPL
```

sym | cond | price
-|-|-
`AAPL` |` `| 95
`AAPL` | `A` | 43
`KX` | `C` | 32

<a name="update_statement"></a>
### Update

```q
tt:100?trade
```
date|time|sym|price|size | cond
-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 422| B
2021.03.01 | 15:09:01| JPM | 74| 412| C

* randomly select 100 rows

```q
update cond: "D" from tt
```
date|time|sym|price|size | cond
-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 422| D
2021.03.01 | 15:09:01| JPM | 74| 412| D
2021.03.01 | 15:09:01| UBS | 41| 312| D

* updates cond to "D"

```q
update size%100 from tt
```
date|time|sym|price|size | cond
-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 42.2| D
2021.03.01 | 15:09:01| JPM | 74| 41.2| D
2021.03.01 | 15:09:01| UBS | 41| 31.2| D

* can perform function on entire column. size divided by 100

```q
update advice:`sell from tt
```
date|time|sym|price|size | cond| advice
-|-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 42.2| D | sell
2021.03.01 | 15:09:01| JPM | 74| 41.2| D | sell
2021.03.01 | 15:09:01| UBS | 41| 31.2| D | sell

* if you update a column that doesnt exist, it will add the column
* new column added called advice and populates with sell
* notice it has to be backtick sell

```q
update advice: `buy from tt where price < 70
```
date|time|sym|price|size | cond| advice
-|-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 42.2| D | 
2021.03.01 | 15:09:01| JPM | 74| 41.2| D | 
2021.03.01 | 15:09:01| UBS | 41| 31.2| D | buy

* if price less than 70, advice becomes buy
* if not, then null value returned

```q
update maxprice: max price by sym from tt
```
date|time|sym|price|size | cond| maxprice
-|-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 42.2| D | 104
2021.03.01 | 15:09:01| JPM | 74| 41.2| D | 102
2021.03.01 | 15:09:01| UBS | 41| 31.2| D | 91

* adds new column max price

<a name="delete_columns"></a>
### Delete Columns
* cannot have by or where clause

Given table tt

date|time|sym|price|size | cond| maxprice
-|-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 42.2| D | 104
2021.03.01 | 15:09:01| JPM | 74| 41.2| D | 102
2021.03.01 | 15:09:01| UBS | 41| 31.2| D | 91

```q
delete maxprice from tt
```
date|time|sym|price|size | cond
-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 42.2| D
2021.03.01 | 15:09:01| JPM | 74| 41.2| D
2021.03.01 | 15:09:01| UBS | 41| 31.2| D

* removes maxprice column

```q
delete date, time from tt
```
sym|price|size | cond
-|-|-|-
BAC | 70| 42.2| D
JPM | 74| 41.2| D
UBS | 41| 31.2| D

* deletes multiple columns from the table

<a name="delete_rows"></a>
### Delete Rows
Given table tt

date|time|sym|price|size | cond| maxprice
-|-|-|-|-|-|-
2021.01.01 | 15:10:01| BAC | 70| 42.2| A | 104
2021.03.01 | 15:09:01| JPM | 74| 41.2| B | 102
2021.03.01 | 15:09:01| UBS | 41| 31.2| C | 91

```q
delete from tt where cond="A"
```
date|time|sym|price|size | cond| maxprice
-|-|-|-|-|-|-
2021.03.01 | 15:09:01| JPM | 74| 41.2| B | 102
2021.03.01 | 15:09:01| UBS | 41| 31.2| C | 91

* deletes row where cond=A

```q
delete from tt
```
date|time|sym|price|size | cond| maxprice
-|-|-|-|-|-|-

* deletes all rows

<a name="sort_asc_desc"></a>
### Sort Ascending / Descending 

```q
`sym`price xasc tt
```
date|time|sym|price|size | cond
-|-|-|-|-|-
2021.01.01 | 15:10:01| A | 70| 42.2| D
2021.03.01 | 15:09:01| B | 73| 41.2| E
2021.03.01 | 15:09:01| C | 79| 31.2| F

* first sorts ascending by sym, then by price

```q
`sym`price xdesc tt
```
date|time|sym|price|size | cond
-|-|-|-|-|-
2021.01.01 | 15:10:01| C | 79| 42.2| D
2021.03.01 | 15:09:01| B | 73| 41.2| E
2021.03.01 | 15:09:01| A | 70| 31.2| F

* first sorts descending by sym, then by price

<a name="rename_reorder_columns"></a>
### Renaming / Reordering Columns

```q
`new1`new2 xcol tt
```
new1|new2|sym|price|size | cond
-|-|-|-|-|-
2021.01.01 | 15:10:01| C | 79| 42.2| D
2021.03.01 | 15:09:01| B | 73| 41.2| E
2021.03.01 | 15:09:01| A | 70| 31.2| F

* renames first 2 columns to new1 and new 2

```q
`cond`size xcols tt
```
cond|size|date|time|sym|price
-|-|-|-|-|-
D| 79| 2021.01.01 | 15:10:01| C | 42.2
E| 73| 2021.03.01 | 15:09:01| B | 41.2
F| 70| 2021.03.01 | 15:09:01| A | 31.2

* reorders columns cond and size to beginning

```q
`sym xgroup tt
```
sym| date
-|-
`BAC` | 2021.01.01
`RBS` | 2021.01.23

* group by column sym

```q
`date`sym xgroup tt
```
date| sym| time
-|-|-
`2021.01.01` | `BAC` | 1:12
`2021.01.02` | `JPM` | 1:45

* group and key by 2 columns (date and sym)

```q
`date`sym xkey tt
```
date| sym| time | price | size | cond
-|-|-|-|-|-
`2021.01.01` | `BAC` | 1:12 | 83 | 834 | B
`2021.01.02` | `JPM` | 1:45 | 34 | 342 | A

* make date and sym key columns

<a name="qsql_problem_set"></a>
## q-SQL Problem Set
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
`AAPL` | 320 | 1015
`C` | 310 | 100
`MS` | 740 | 234

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
`A`|	2021-06-03|	87.54| 49100
`AA`|	2021-06-03|	68.09| 88100


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
`9`|	3186|	159063500
`10`|	6544|	321195100
`11`|	6280|	315284200

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
`09:30`|	3186|	159063500
`10:00`|	3271|	162197000
`10:30`|	3273|	158998100

* 30 xbar time.minute = rounds minutes by 30; groups together and is set as key

<hr>

**10. Find all trades for `A where the price was cheaper than the average for that day**

```q
a: update avgPrice: avg price by date from select from trade where sym=`A
```
