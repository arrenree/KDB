# Allen's Notes for KDB+ / Q
<a name="top"></a>


## [Functions](#functions_header)
1. [Defining & Calling Functions](#define_func)
2. [Anonymous Function](#anon_function)
3. [Implicit Argument](#implicit_argu)
4. [Local vs Global Variables](#local_global_variables)
5. [Projected Functions](#projected_func)

## [Functions Problem Set](#func_problem_set)

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

<hr>

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

<hr>

## [Keyed Table Problem Set](#keyed_table_problem_set)

## [Table Attributes](#table_attributes)
1. [Setting Attributes During Creation](#set_attribute_creation)
2. [Applying Attribute to Existing Data](#apply_attribute_data)
3. [Updating Attribute to Existing Data](#update_attribute_data)
4. [Clear Attributes](#clear_attribute)
5. [Attributes Benefits](#fast_attribute)
6. [Sorted Attribute](#sort_attribute)
7. [Unique Attribute](#unique_attribute)
8. [Grouped Attribute](#group_attribute)
9. [Parted Attribute](#parted_attribute)

<hr>

## [Foreign Key Restrictions](#fkey_restrictions)
1. [Single Foreign Keys](#single_fkey)
2. [Checking Foreign Keys](#check_fkey)
3. [Upserting with Foriegn Keys](#upsert_fkey)
4. [Retrieving Custom Columns via fkey](#retrieve_fkey)
5. [Multiple Foreign Keys](#multi_fkey)

## [Foreign Key Problem Set](#fkey_problemset)

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

<hr>

## [qSQL Problem Set](#qsql_problem_set)

## [qSQL Joins](#qsql_joins)
1. [Left Join](#left_join)
2. [Plus Join](#plus_join)
3. [Inner Join](#inner_join)
4. [Union Join](#union_join)

<hr>

## [qSQL Joins Problem Set](#qsqljoins_problem_set)

<hr>





<a name="functions_header"></a>
## Functions
[Top](#top)

<a name="define_func"></a>
### Defining & Calling Functions
* functions are encased in { }
```q
f: { [a] a * a}
```
```q
f [3]
```
or
```q
f @ 3
```
9
* [a] defines the argument
* f[3] or f@3  calls the function with a=3

```q
add: { [a;b] a+ b}
```
```q
add [3;5]
```
8
* multi argument function
* [a;b] = defines first, second argument
* a+b = statement

<a name="anon_function"></a>
### Anonymous Functions
```q
{[a] a*a}6
```
36
* you dont assign variable 
* simply call the argument outside the function { } 

<a name="implicit_argu"></a>
### Implicit Argument
```q
{x*x}5
```
25
* omit [x], q implicitly understands x is an argument

```q
{x+y+z}[1;2;3]
```
6
* q has x, y, z as implicit arguments

```q
{x+z}[1;2]
```
* error because you can't skip the y. if only 2 implicit arguments, need to use x, y

<a name="local_global_variables"></a>
### Local vs Global Variables
```q
{a:1; b:2; a+b*x} [12]
```
25
* = (12x2) + 1
* a and b are locally defined variables within the function
* will NOT work if you try to recall variable a or b outside the function
* 12 = implicit argument x

```q
d:10
f:{d+x}
f 1
```
11
* assign global variable D to 10 (outside the function)
* functions pulls in 10 (global variable) for d and 1 for x (implicit argument)

```q
g: {d:20; d+x}
g 1
```
21
* local variable d:20 takes priority over global variable of 10

<a name="projected_func"></a>
### Projected Functions
```q
raise: {x xexp y}
raise [10; 2 3 4]
```
100 1000 1000f
* calls x = 10; y = 2 3 4

```q
g: raise [10; ]
g 1 2 3
```
10 100 1000
* creates a projection of the original raise function

<hr>

<a name="func_problem_set"></a>
## Functions Problem Set
[Top](#top)

**1. Create a function volc that accepts 2 arguments (r and h), that returns the volume of the given volc [2;3]** \
vol of cone = 1/3 * pi * r^2 * h \
pi = -4 * atan -1**

```q
volc: {[r;h] pi:-4*atan -1; pi*r*r*h%3}
volc[2;3]
```
12.57
* define arguments [r;h] first
* define variable pi
* must have space after atan and before -1
* no space for volc[2;3]

<hr>

**2. Write function sph that takes radius and returns the area and volume**\
v = 4/3 * pi * r^3 \
a = 4 * pi * r^2

```q
sph: { [r] pi:-4*atan -1; a:(4%3)*pi*r xexp 3; v:4*pi*r xexp 2; `area`volume ! (a;v)}
```
```q
sph[1]
```
key|value
-|-
area	|4.18
volume |	12.56

* define argument [r]
* define variable pi with formula
* define variable a with formula
* define variable v with formula
* show dictionary with symbols `area `volume against values a and v

<hr>

**3. Create function setc that takes one argument and sets the global value c to that argument**
```q
setc: {c::x}
setc[10]
c
```
10
* setc 10 = setting x = 10 (implicit variable)
* since x = 10, and you've set c as the global variable to x, then c = 10

```q
setc `hi
c
```
`hi
* you set setc = `hi, so c = x = `hi

<hr>

**4. Given raise:{x xexp y}, create function that is projection of the raise. Ex, root[9] = 3**
```q
raise: {x xexp y}
root: raise[ ; 0.5]
root[9]
```
3
* an embedded function is a function within another function
* root function sets y as 0.5
* so root 9 =x

<hr>

**5. Convert all entries of list L to a string**
* list of long, sym, and boolean
```q
l: (100;`price;1b)
string l
```
"100"
"price"
"1b"

* remember, mixed lists have to be contained in parathesis ( )

<hr>

**6. Given the string, find and replace "cow" with "kangaroo"**

```q
st: "the cow jumped over the moon"
ssr [st; "cow";"kangaroo"]
```
"the kangaroo jumped over the moon"
* ssr = string search replace.
* syntax = ssr [listname + find this + replace with this]

<hr>

**7. Create function sayHi that takes 2 arguments, first one name, second one age and behaves as follows:**

sayHi("joe";90] \
"hello 90 year old joe"

```q
sayHi:{[name;age] "hello ", string[age]," year old ", name}
sayHi["joe";90]
```
hello 90 year old joe
* name and age are your arguments
* "hello" and "year old" are simply lists of characters
* you have to convert raw data values into strings, use , to concatenate the strings together
* need to convert [age] to string
* when you define argument "joe" have to use parathesis otherwise wont work

<hr>

**8. I have a box of 7 eggs, find the median and average weight**

eggs: 10 20 30 40 50 60 70

```q
med eggs
```
40
```q
avg eggs
```
40

<hr>

**9. I sold 2 boxes of eggs. 1 box had 10 eggs and i sold it for 50 each. the other box had 20 eggs and sold it for 100 each. find the average price paid per egg**

```q
10 20 wavg 50 100
```
83.3
* wavg = weight average function

<hr>

**10. Generate list k of 10 random integers. Find the moving average with window size of 3**
```
k: 10?10
mavg[3;k]
```
8 4.5 6 5 6 5 5.33 4.33 5 4.67

**Find the 3 largest numbers in list k**

```q
3#desc k
```
9 8 8 
* take 3 of the largest from k, sort by desc

**Find the difference between the successive elements of k**

```q
deltas k
```
8 -7 8 -4 -1 2 0 -5 7 -3

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
( [] id:`a`b) # kt
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

**1. Create the following keyed table**

table p
`book` | `ticker`|size
-|-|-
`A`| `MS`| 100
`B`| `AAPL`| 200
`B`| `MS`| 300
`C`| `C`| 400

```Q
p: ( [book:`A`B`B`C; ticker:`MS`AAPL`MS`C] size:100 200 300 400)
```
* book and ticker are keys
* must use backtick for values
* no ; after the []
* no commas between values

<hr>

**2. Retrieve entries where book is B, using select**
```q
select from p where book=`B
```
book | ticker|size
-|-|-
`B`| `AAPL`| 200
`B`| `MS`| 300

<hr>

**3. Retrieve entries where book is C and ticker is c, using take**
```q
( [book:enlist`C; ticker:enlist`C]) # p
```
book | ticker|size
-|-|-
`C`| `C`| 400

* underlying table p has 2 keyed columns (book and ticker)
* you cannot retrieve 2 keyed columns if underlying table only has 1 key column

**4. Upsert the following values**

table p

`book` | `ticker`|size
-|-|-
`A`| `MS`| 100
`B`| `AAPL`| 200
`B`| `MS`| 300
`C`| `C`| **400**
**`D`**|**`MS`**|**500**

```q
upsert [p; ([book:`C`D; ticker:`C`MS]size:400 500)]
```
`book` | `ticker`|size
-|-|-
`A`| `MS`| 100
`B`| `AAPL`| 200
`B`| `MS`| 300
`C`| `C`| 400
`D`|`MS`|500

<hr>

<a name="table_attributes"></a>
## Table Attributes
[Top](#top)

<a name="set_attribute_creation"></a>
### Setting Attributes During Creation
```q
l:`s# 1 2 3 4 5 
```
1 2 3 4 5
* applies the sorted attribute during creation of the list

```q
attr l
```
's

* checks what attributes are applied to list l
* 's means sorted attribute applied

<a name="apply_attribute_data"></a>
### Applying Attribute to Existing Data
```q
k: 1 2 3 4 5
```
```q
@ [ `.; `k;`s#]
```
* @ = apply
* `. = within the default name space
* within the default name space, apply the sorted attribute to list k

```q
attr k
```
`s
* confirms list k now has the `s# sorted attribute

<a name="update_attribute_data"></a>
### Updating Attribute to Existing Data

Given:

table t

time|name|val
-|-|-
08:00:00.000 |	joe|	10
08:30:00.000|	jim|	20
09:10:00.000|	bob|	30

```q
meta t
```
c|t|f|a
-|-|-|-
time|	t	|	
name|	s|		
val	|j|		

* a = attributes = currently nothing

```q
update `s#time from `t
```
* update column time from table t with the sorted attribute

c|t|f|a
-|-|-|-
time|	t	|	|a
name|	s|		
val	|j|		

* under attributes for column time, s sorted has been applied

<a name="clear_attribute"></a>
### Clear Attributes
```q
@ [`.;`k;`#]
```

```q
attr k
```
`
<a name="fast_attribute"></a>
### Attribute Benefits
Given:
```q
k: til 1000000
```
0 1 2 3...999,999

```q
\t do[1000; k?500000]
```
* time 1,000 lookups for the number 500,000 in list k
130
* it took 130 miliseconds

```q
`s#k
```
* appy the sorted attribute to list k

```q
\t do[1000; k?500000]
```
0
* after applying sort attribute, only took 0 miliseconds
* applying sort applies a binary search. start in the middle, (ex 5), less than that, so checks mid (ex 3), more, so 4

<a name="sort_attribute"></a>
### Sorted Attribute
* sorted attribute applied to list or column to specify data is sorted in ascending order
* the underlying list must already be in ascending order, otherwise error
* `s# attribute only maintained during append that maintain the sort requirement, otherwise lost

```q
list: 1 2 3 4 5
```
```q
`s#list
```
* apply sorted attribute to list
```q
attr list
```
* checks what attributes are applied to list; confirms sorted attributed applied
`s
```q
list,: 6
```
* add 6 to list
```q
attr list
```
* checks attributes for list
* the sort attribute maintained since 6 is in ascending order to list
`s

```q
list,:3
```
* adds 3 to list

```q
attr list
```
* sort attribute LOST because 3 is not ascending to existing list

```q
`s#list
```
* cannot apply sort attribute because underlying list is NOT ascending
s-fail

<a name="unique_attribute"></a>
### Unique Attribute
* unique attribute applied to a list where all values must be unique (no same values)

```q
lu:`u#1 2 3 4 5
```
`u

```q
lu,:7
```
* appends 7 to list lu

```q
attr lu
```
`u
* lu still has unique attribute

```q
lu,:4
```
* adds 4 to list lu

```q
attr lu
```
`
* loses unique attribute since 4 already exists

<a name="group_attribute"></a>
### Grouped Attribute
* groups same identifiers together for faster searches

```q
lg: 1 3 2 3 2 1 2 3
```
```q
@ [`.;`lg;`g#]
```
* @ = apply
* `. = within the default name space
* g# = group attribute
* within the default name space, apply the group attribute to list lg

```q
attr lg
```
`g
* confirms group attribute applied to list lg

```q
group lg
```
key|value
-|-
1|	0 5
3|	1 3 7
2|	2 4 6

* stores lookup table from values to indices where they occur

<a name="parted_attribute"></a>
### Parted Attribute
* parted attribute marks a list of having same value occuring in sequential block
* enables faster searches

```q
lp:`p#`a`a`a`b`b`b`c`c`c
```
* applied parted attribute to list lp

```q
attr lp
```
`p

* confirms parted attribtue applied to list lp

```q
lp,:`a
```
* appends a to list

```q
attr lp
```
`
* loses group attribute since a now isnt in sequential block

<hr>

<a name="fkey_restrictions"></a>
## Foreign Key Restrictions
[Top](#top)

* Foreign keys restrict the values that are allowed in a column

<a name="single_fkey"></a>
### Single Foreign Keys

Given:

```q
company:([sym:`TS`KX`C`AAPL`GOOG`MS] advice: 6?`HOLD`BUY`SELL; level: 6?100)
```

company table

sym | advice | level
-|-|-
`TS`|HOLD |40
`KX` |HOLD |51
`C` | SELL | 55
`AAPL`|	BUY|	90
`GOOG`|	SELL|	73
`MS`|	SELL|	90

```q
employee:( [] name:`ryan`charlie`arthur`greg; employer:`TS`KX`KX`MS)
```

employer table

name|employer
-|-
ryan|TS
charlie|KX
arthur | KX
greg | MS

```q
update `company$employer from `employee
```
* similar to casting, you limit the employer column to the domain in company table (keyed column)
* limits the **employer** column from **employee table** to the domain (keyed column = **sym**) in the **company table**
* the domain table HAS to be keyed
* the values in column employee must exist in domain company table

<a name="check_fkey"></a>
### Checking Foreign Keys

```q
meta employee
```
c|t|f|a
-|-|-|-
name|	s| |		
employer|	s|	company| |	

* c = column
* f = foreign key
* confirms the employer column is linked to the company table

```q
fkeys employee
```

key|value
-|-
employer|company

<a name="upsert_fkey"></a>
### Upserting with Foreign Keys
```q
upsert[employee; ( [] name:`james`claire; employer:`RBS`RBS)]
```
`cast
* prev set **employer column** from **employee table** as fkey to **company table** domain (**sym**)
* error because RBS is NOT a sym in the company table
* fkey restricts us from adding what's not in the domain  

```q
insert[`company; ([sym:enlist `RBS] advice:enlist `SELL; level: enlist 20)]
```
* need to first add RBS into the company domain (as a keyed sym)
* remember  need to use enlist when adding single rows

sym|advice|level
-|-|-
`TS`|HOLD |40
`KX` |HOLD |51
`C` | SELL | 55
`AAPL`|	BUY|	90
`GOOG`|	SELL|	73
`MS`|	SELL|	90
`RBS|SELL |20

```q
upsert[employee; ( [] name:`james`claire; employer:`RBS`RBS)]
```

name|employer
-|-
ryan|TS
charlie|KX
arthur | KX
greg | MS
james|RBS
claire | RBS

* now you can append james and claire

<a name="retrieve_fkey"></a>
### Retrieving Columns via fkey
company table

sym | advice | level
-|-|-
`TS`|HOLD |40
`KX` |HOLD |51
`C` | SELL | 55
`AAPL`|	BUY|	90
`GOOG`|	SELL|	73
`MS`|	SELL|	90

employer table

name|employer
-|-
ryan|TS
charlie|KX
arthur | KX
greg | MS

```q
update employer.advice, employer.level from employee
```
* prev you keyed the employer column to domain of company table (linking the 2 tables)
* from the employee table, retrieve the value linked from **employer column** to **company table**
* pulls in **advice** and **level** from the **company table**

name|employer|advice|level
-|-|-|-
ryan|	TS	|SELL|	12
charlie|	KX	|BUY	|10
arthur|	KX|	BUY|	10
greg|	MS|	SELL|	90

<a name="multi_fkey"></a>
### Multiple Foreign Keys
```q
office: ([sym:`TS`KX`C; loc:`LDN`NY`LDN] employees:10+3?1000)
```
office

sym|loc|employees
-|-|-
`TS`|	`LDN`|	875
`KX`|	`NY`|	354
`C`	|`LDN`|	1007

```q
employee: ([] name:`ryan`charlie`arthur; employer:`TS`KX`KX; city:`LDN`NY`NY)
```
employee

name|employer|city
-|-|-
ryan|	TS|	LDN
charlie|	KX|	NY
arthur|	KX|	NY

```q
exec `office$flip (employer;city) from employee
```
0 1 1

* since the office table has 2 keyed columns, you have to "cast" 2 columns as fkey
* ignore the flip syntax - youre settingn fkey by linking columns **employer** and **city** from the employee table to the domain of the **company table** (keyed columns)
* ryan, look for TS and LDN in office table, found on row 0
* charlie, look for KX and NY in office table, found on row 1
* arthur, look for KX and NY in office table, found on row 1

```q
update empOffice:`office$flip(employer;city) from `employee
```
name|employer|city|empOffice
-|-|-|-
ryan|	TS|	LDN|	0
charlie|	KX|	NY|	1
arthur|	KX|	NY|	1

* adds new column **empOffice**, which retrieves linked values from office table
* sets column **empOffice** as the foreign key

```q
meta employee
```
c|t|f|a
-|-|-|-
name|	s|	|	
employer|	s	|	|
city|	s|	|	|
empOffice|	j|	office|	|

* meta shows us empOffice has an foreign key referencing the office table

```q
update empOffice.sym, empOffice.loc from employee
```
name|employer|city|empOffice|sym|loc
-|-|-|-|-|-
ryan	|TS|	LDN|	0	TS|	LDN
charlie|	KX|	NY	|1	KX|	NY
arthur|	KX|	NY	|1|	KX|	NY

* employee table doesnt have columns for sym or loc
* but since you set the empOffice as foreign key, it pulls in the values from the company table

<hr>

<a name="fkey_problemset"></a>
## Foreign Key Problem Set
[Top](#top)

**1. Given the following table**

book table

id|name
-|-
fmgoh|jim
fddig|allen
lefhe|bob
bfjnf|sherman

trade table

date|time|sym|price|size|cond|bookId
-|-|-|-|-|-|-
2021.01.01 | 09:00|D| 109|100| |fmgoh
2021.01.01|09:00|AA|93|100| B | fddig
2021.01.01|09:00|UPS|34|100| A| lefhe
2021.01.01|09:00|A|56|100| C| bfjnf

**1. Insert a foreign key column into the trade table called owner, linking trade and book table, using bookID**
```q
update owner: `book$bookId from `trade
```
* from trade table, insert a new column **owner**, take column **bookId** and limit to domain in book table

date|time|sym|price|size|cond|bookId | owner
-|-|-|-|-|-|-|-
2021.01.01 | 09:00|D| 109|100| |fmgoh|fmgoh 
2021.01.01|09:00|AA|93|100| B | fddig| fddig
2021.01.01|09:00|UPS|34|100| A| lefhe| lefhe
2021.01.01|09:00|A|56|100| C| bfjnf| bfjnf

```q
meta trade
```
c | t|f|a
-|-|-|-
owner | | book|

**2. Join the book table onto the trade table and add the name of person who did trade**
```q
update owner.name from trade
```
date|time|sym|price|size|cond|bookId | owner|name
-|-|-|-|-|-|-|-|-
2021.01.01 | 09:00|D| 109|100| |fmgoh|fmgoh |jim
2021.01.01|09:00|AA|93|100| B | fddig| fddig|allen
2021.01.01|09:00|UPS|34|100| A| lefhe| lefhe|bob
2021.01.01|09:00|A|56|100| C| bfjnf| bfjnf|sherman

* the book table only has id and name columns, so you are really only joining the name column onto trade
* since owner is linked to book table, you can use that as a link to reference the name colum* 

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
* 
<hr>

<a name="qsql_problem_set"></a>
## qSQL Problem Set
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

<hr>

<a name="qsql_joins"></a>
## qSQL Joins
[Top](#top)

<a name="left_join"></a>
### qSQL Join Left 

* syntax = **source table** lj **lookup table** (must be keyed)
* for each row in **source**, find corresponding values in **lookup** (keyed)
* no match = nulls
* column names must match
* will always return same number of rows as **source** table

trade table

x|date |      time |        sym|  price|    size  
-|-----|-----------|-----------|---------|------
1|2021.06.03| 09:30:02.553| C   | 107.2018| 63500
2|2021.06.03| 09:30:02.701| MSFT |96.87488| 1700
3|2021.06.03| 09:30:02.743| RBS  |97.11338| 80700
4|2021.06.03| 09:30:02.758| A    |100.35  | 50300
5|4021.06.03| 09:30:03.044| F    |79.48574| 54100

stock table

x|`sym`| sector | employees
-|---|--------|----------
1|`C`    |Tech      |862      
2|`MSFT` |Tech      |765      
3|`RBS`  |Tech      |377      
4|`A`    |Financial |167      
5|`F`    |Financial | 615     

```q
trade lj stock
```

x|date |      time |        sym|  price|    size|  cond| sector |   employees
-|-----|------------|------------|--------|----------|------|----------|-----
1|2021.06.03| 09:30:02.553| C   | 107.2018| 63500| B |  Tech      |862      
2|2021.06.03| 09:30:02.701| MSFT| 96.87488| 1700 | B |  Tech      |765      
3|2021.06.03| 09:30:02.743| RBS | 97.11338| 80700| C |  Tech      |377      
4|2021.06.03| 09:30:02.758| A   | 100.35  | 50300| B |  Financial |167      
5|2021.06.03| 09:30:03.044| F   | 79.48574| 54100| A |  Financial |615      

* all column names must match
* **stock** table has **sector** and **employees**, which **trade** does not
* **trade** = source table
* **stock** = lookup table (keyed by sym)
* takes trade table, for each sym, pulls in **sector** and **employees** columns
* will always be same number of rows as source table (5)

<a name="plus_join"></a>
### qSQL Plus Join 

* finds the same value across 2 tables, adds their values

stock table

x|`sym`| sector | employees
-|---|--------|----------
1|`C`    |Tech      |100      
2|`MSFT` |Tech      |100      
3|`RBS`  |Tech      |100      

trade table

x|`sym`| sector | employees
-|---|--------|----------
1|`C`    |Tech      |100      
2|`MSFT` |Tech      |-100      

```q
stock pj trade
```
or
```q
stock pj [ (sym:`C`MSFT] employees: 100 -100)
```

* stock = source table
* trade = lookup table

x|`sym`| sector | employees
-|---|--------|----------
1|`C`    |Tech      |200      
2|`MSFT` |Tech      |0      
3|`RBS`  |Tech      |100    

* from stock table, find the corresponding syms, add values together
* if value doesnt exist (RBS) just leave as is

<a name="inner_join"></a>
### qSQL Inner Join 

* similar to left join, but **only returns rows where matches occur**

trade table

x|date |        sym|  price|    size  
-|-----|-----------|---------|------
1|2021.06.03| C   | 107.2018| 63500
2|2021.06.03| MSFT |96.87488| 1700
3|2021.06.03| UBS    |100.35  | 50300

stock table

x|`sym`| sector | employees
-|---|--------|----------
1|`C`    |Tech      |100      
2|`MSFT` |Tech      |100      

```q
trade pj stock
```
* adds columns where the key matches (sym), otherwise remove

x|date |        sym|  price|    size  | sector | employees
-|-----|-----------|---------|------| -|-
1|2021.06.03| C   | 107.2018| 63500| Tech | 100
2|2021.06.03| MSFT |96.87488| 1700| Tech | 100

* removes row UBS since no match

<a name="union_join"></a>
### qSQL Union Join 

* adds ALL rows/columns together
* if key matches, will upsert (update or insert)
* if no match, just append as new entry

trade table

x|date |        sym|  price|    size  
-|-----|-----------|---------|------
1|2021.06.03| C   | 107.2018| 10
2|2021.06.03| MSFT |96.87488| 10
3|2021.06.03| UBS    |100.35  | 10

stock table

x|`sym`| sector | size | book
-|---|--------|---------|-
1|`FB`    |Tech      |100| A      
2|`GOOG` |Tech      |100 | B

```q
trade uj stock
```
x|date |        sym|  price|    size | book 
-|-----|-----------|---------|------|--
1|2021.06.03| C   | 107.2018| 10 | 
2|2021.06.03| MSFT |96.87488| 10 |
3|2021.06.03| UBS    |100.35  | 10 |
4| | FB |  |100 |A
5| | GOOG |  |100 | A

* no key match for FB or GOOG, so appends new row
* adds new column book; blank for existing, pulls in value from new

<hr>

<a name="qsqljoins_problem_set"></a>
## qSQL Joins Problem Set
[Top](#top)

```q
\l ex-joins.q
```
```q
\a
```
* **fbTrades** (headers = dt, sym, size, book) \
* **newsItems** (headers = ndate, ticker, title) \
* **quote** (headers = date, time, sym, size, cond, bid, ask, asize, bside)\
* **stock** (headers = sym, sector, employees)\
* **trade** (headers = dt, sym, price, size)

**1. Find the total value of trades by sector, include those who's sector is unknown (totalvalue = price x size)**

* the columns you need are price x size (trade table) and sector (stock table) 
* need to use left join because you want to keep the same number of rows, and add in the relevant columns

```q
trade lj stock
```
dt|sym|price|size|sector|employees
-|-|-|-|-|-
2015-01-01|	C|	10.0|	10|	Financial|	262000
2015-01-02|	C	|10.5	|100	|Financial|	262000
2015-01-04|	DBK|	35.6|	55|	|	

* joins tables together, but does not calculate totalValue

```q
select totalValue:sum price*size by sector from trade lj stock
```

sector | totalValue
-|-
null	|1958.0
Financial|	159850.0
Tech	|326200.0

```q
select totalValue:sum price*size by `unknown^sector from trade lj stock
```
sector |totalValue
-|-
Financial|	159850.0
Tech|	326200.0
unknown|	1958.0

* use `unknown^sector to rename the null sectors (visually more appeasing)
* price * size will get you all the individual prices, but you want an aggregate figure. so need to use sum price
* you want the new values by sector, so this becomes your key

<hr>

**2. Combine trades from trade and fbTrades Table into a table t2, sorted by date. Include all columns**

* include all columns, so we use union join

```q
t2: trade uj fbTrades
```
dt|sym|price|size|book
-|-|-|-|-
2015-01-06|	AAPL	|1020.0|	300|	
2015-01-07|	MS	|254.0|	400|	
2015-01-02|	FB	|	1000|	A
2015-01-03|	FB	|	1000|	B
2015-01-05|	FB	|	1000|	A

* joins tables together, but doesnt sort by date

```q
t2:`dt xasc trade uj fbTrades
```
dt|sym|price|size|book
-|-|-|-|-
2015-01-02|	FB	|	1000|	A
2015-01-03|	FB	|	1000|	B
2015-01-05|	FB	|	1000|	A
2015-01-06|	AAPL	|1020.0|	300|	
2015-01-07|	MS	|254.0|	400|	

* `dt xasc sorts dates by ascending
* since you are joining table together, no select query

<hr>

**3. Find the highest and lowest price in the trade table for each sym**

```q
select max price by sym from trade
```
sym|price
-|-
AAPL|	1020.0
C|	11.0
DBK|	35.6
MS|	260.0

```q
select min price by sym from trade
```
sym|price
-|-
AAPL|	1010.0
C|	10.0
DBK|	35.6
MS|	254.0

<hr>

**4. Find the 2 highest trade prices for each sym**

```q
ungroup select 2 sublist desc price by sym from trade
```
* sublist creates a subset of a list
* select 2 = you want 2 highest
* sort by descending 
* ungroup = ungroups everything

sym | price
-|-
AAPL|	1010.0
C	|10.0
DBK|	35.6
MS	|254.0

```q
select 2 sublist desc price by sym from trade
```
sym | price
-|-
AAPL|	1,020 1,010f
C	|11 10.5
DBK|	,35.6
MS|	260 255f

* if you dont ungroup, it groups together by sym

<hr>

**5. Find the average daily price for each sym in trade table. Join the newsItems table to show only those items where the sym had a newsItem on that date**

* from trade table, find avg price. then join the newsItem table where matches date and sym
* so date and sym need to be keys in the newsItems table
* **newsItems** (headers = ndate, ticker, title) \
* **trade** (headers = dt, sym, price, size)

```q
select avg price by dt, sym from trade
```
* first step is calc the avg price grouped by dt, sym from **trade** table

dt|sym|price
-|-|-
2015-01-01|	C|	10.0
2015-01-02|	C	|10.5
2015-01-03|	MS|	260.0
2015-01-04|	C	|11.0
2015-01-04|	DBK|	35.6
2015-01-05|	AAPL|	1010.0
2015-01-06|	AAPL	|1020.0
2015-01-07 |	MS	|254.5

```q
(select avg price by dt, sym from trade) ij 2!`dt`sym xcol newsItems
```
* `dt`sym xcol newwsItems = **renaming columns** in newsItems from **ndate to dt** and **ticker to sym**
* then use 2! to set those 2 columns as keys
* then inner join so only those rows with matches will be returned
* 2! sets first 2 columns as keys in newsItems table

dt| sym| price|title
-|-|-|-
2015-01-04|	C|	11.0|	regulators| investigating

<hr>

**6. Take the newsItems table and join the trade table to bring in the latest price for each ticker**

```q
aj [`ticker`ndate;newsItems; `ndate`ticker xcol trade]
```
* from newsItems table, retrieve ticker and ndate
* from trade table, rename dt to ndate and sym to ticker
* aj = as of join

ndate|ticker|title|price|size
-|-|-|-|-
2015-01-06|	MS|	traders did it!|	260.0|	15
2015-01-04|	C|	regulators investigating|	11.0|	200

```q
delete size from aj [`ticker`ndate;newsItems; `ndate`ticker xcol trade]
```

ndate|ticker|title|price
-|-|-|-
2015-01-06|	MS|	traders did it!|	260.0
2015-01-04|	C|	regulators investigating|	11.0

* deletes the size column

<hr>


[Top](#top)

