# Allen's Notes for KDB+ / Q

### q-SQL
1. [Select from where](#select_from_where)
2. [Select parameters](#select_parameters)
3. [Using operations and functions](#select_from_where)
4. [In function](#select_from_where)
5. [Within function](#select_from_where)
6. [xbar group by time](#select_from_where)
7. [xbar function](#select_from_where)

<a name="select_from_where"></a>
# Select from where

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


<a name="select_parameters"></a>
# Select Parameters

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




