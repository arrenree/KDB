# Allen's Notes for KDB+
<a name="top"></a>
[bottom](#bottom)

## 1. [KDB Basics](#kdbintro_header)
1. [Assigning Values to Variable](#assign_intro)
2. [Expressions](#expression_intro)
3. [Division](#division_intro)
4. [Loading Scripts](#load_intro)
5. [Floats](#float_intro)
6. [Til](#til_intro)
7. [Booleans](#boolean_intro)
8. [Over](#over_intro)
9. [Scan](#scan_intro)
10. [Count](#count_intro)
11. [Take](#take_intro)
12. [Drop](#drop_intro)
13. [Larger](#larger_intro)
14. [Smaller](#smaller_intro)
15. [+:](#pluscolon)
16. [Multi-line Comment](#multilinecomment)
17. [Signum](#signum)
18. [Cross](#cross_operator)

## 2. [Data Types & Casting & Enumeration](#casting_header)
1. [Datatype Table](#datatype_table)
2. [Date](#date_type)
3. [Time](#time_type)
4. [Casting](#cast_type)
5. [Enumeration](#enu_cast)

## 3. [Data Types & Casting & Enumeration Problem Set](#casting_problemset)

## 4. [Lists](#lists_header)
1. [Simple Lists](#simple_list)
2. [Mixed Lists](#mixed_list)
3. [Empty Lists](#empty_list)
4. [Single Item Lists](#atom_list)
5. [Joining Lists](#join_lists)
6. [Retrieving from Lists](#retrieve_list)
7. [Update List Values](#update_list)
8. [Nested Lists](#nest_list)
9. [Matrix](#matrix_list)
10. [Sublist](#sublist_list)
11. [Find Operator](#find_list)
12. [Random Operator](#random_list)
13. [Count Operator](#count_list)
14. [Raze](#raze_intro)
15. [Union - Lists](#union_list)
16. [Where Clause - Lists](#where_lists)
17. [Contain](#contain_ops)
18. [Except](#except_ops)
19. [Inter](#inter_ops)
20. [Distinct](#distinct_ops)

## 5. [Lists Problem Set](#list_problemset)

## 6. [Primitive Operations](#primitive_header)
1. [Addition](#add_list)
2. [Comparing Lists](#compare_lists)
3. [Equal and Match Differences](#match_diff)
4. [Basic Operations](#basic_operations)
5. [Division Remainders Mod](#mod_operations)
6. [Running Sums/Moving Windows](#running_sums)
7. [Reverse](#reverse_ops)
8. [Upper/Lowercase](#uppercase_ops)

## 7. [Primitive Operations Problem Set](#primitive_problemset)

## 8. [Dictionary](#dict_header)
1. [Ways to Construct Dictionaries](#dict_from_list)
2. [Retrieving values](#retrieve_dict)
3. [Index Retrieve](#index_retrieve_dict)
4. [Take](#take_dict)
5. [Drop](#drop_dict)
6. [Upsert](#upsert_dict)
7. [Multi Key Dictionaries](#multi_key_dict)
8. [Repeat Keys](#repeat_key_dict)
9. [Find Operator](#find_dict)
10. [Dictionary Operators](#dict_opt)
11. [Adding / Joining Dictionaries](#dict_adding)
12. [Boolean Comparisons](#dict_boo)

## 9. [Dictionary Problem Set](#dict_problemset)

## 10. [Functions](#functions_header)
1. [Defining & Calling Functions](#define_func)
2. [Anonymous Function](#anon_function)
3. [Implicit Argument](#implicit_argu)
4. [Local vs Global Variables](#local_global_variables)
5. [Projected Functions](#projected_func)
6. [If True Statements](#iftrue_state)
7. [If True/Else Statements](#iftrue_else_state)
8. [Adding Conditional Branch Pair](#add_cond_branch)
9. [Do Loops](#do_loop)
10. [While_Loops](#while_loop)
11. [Multi Condition While Loops](#multi_cond_while_loop)
12. [Prime Numbers Function Case Study](#prime_func)
13. [Function within a Function Lambda](#func_lambda)

## 11. [Functions Problem Set](#func_problem_set)

## 12. [Tables](#tables_header)
1. [Flipping Dictionary to Table](#dict_to_table)
2. [Simple Table](#simple_table)
3. [Single Row Table](#single_row_table)
4. [Mixed Table](#mixed_table)
5. [Meta / Data Type Table](#meta_datatypes_table)
6. [Count Row Table](#countrowsimple_table)
7. [Rename, Reorder Columns (xcol, xcols)](#rename_column_table)
8. [Add Column Table](#add_column_table)
9. [Sort Columns (xasc, xdesc)](#sort_column_table)
10. [Union Table](#union_table)
11. [Except Table](#except_table)
12. [Inter Table](#inter_table)
13. [Distinct Table](#distinct_table)
14. [Retrieve From Table](#retrieve_table)
15. [Insert Rows Table](#insert_table)
16. [Upsert Rows Table](#upsert_table)
17. [Operations on Tables](#operations_table)
18. [Joins on Tables](#joins_table)
19. [Find on Tables](#find_table)

## 13. [Tables Problem Set](#tables_problem_set)

## 14. [Keyed Tables](#keyed_tables)
1. [Single Keyed Table](#single_keyed_table)
2. [Multi_Keyed_Table](#multi_keyed_table)
3. [Retrieving Keys/Values](#retrieving_keysvalues)
4. [Changing Keys](#changing_keys)
5. [Adding Keys](#adding_keys)
6. [Removing Keys](#removing_keys)
7. [Upsert Keys](#upsert_keys)
8. [Upsert Multi Row/Keys](#upsert_multi_rowkeys)
9. [Retrieving Values from SINGLE Keyed Table](#retrieve_single_value_keys)
10. [Retrieve SINGLE ROW as a DICTIONARY](#ret1)
11. [Retrieve MULTI ROWS as a DICTIONARY](#ret2)
12. [Retrieve SINGLE ROW as a TABLE](#ret3)
13. [Retrieve MULTI ROWS as a TABLE](#ret4)
14. [Retrieving Values from MULTI Keyed Table](#retrieve_multi_value_keys)
15. [Retrieve SINGLE ROW as a DICTIONARY](#ret5)
16. [Retrieve MULTI ROWS as a DICTIONARY](ret6)
17. [Retrieve SINGLE ROW as a TABLE](#ret7)
18. [Retrieve MULTI ROWS as a TABLE](#ret8)

## 15. [Keyed Table Problem Set](#keyed_table_problem_set)

## 16. [Table Attributes](#table_attributes)
1. [Setting Attributes During Creation](#set_attribute_creation)
2. [Applying Attribute to Existing Data](#apply_attribute_data)
3. [Updating Attribute to Existing Data](#update_attribute_data)
4. [Clear Attributes](#clear_attribute)
5. [Attributes Benefits](#fast_attribute)
6. [Sorted Attribute](#sort_attribute)
7. [Unique Attribute](#unique_attribute)
8. [Grouped Attribute](#group_attribute)
9. [Parted Attribute](#parted_attribute)

## 17. [Foreign Key Restrictions](#fkey_restrictions)
1. [Single Foreign Keys](#single_fkey)
2. [Checking Foreign Keys](#check_fkey)
3. [Upserting with Foriegn Keys](#upsert_fkey)
4. [Retrieving Custom Columns via fkey](#retrieve_fkey)
5. [Multiple Foreign Keys](#multi_fkey)

## 18. [Foreign Key Problem Set](#fkey_problemset)

## 19. [qSQL](#qsql_header)
1. [Select Template](#select_template)
2. [Adding a new column using Select](#selectadd_template)
3. [Virtual Column i](#qsqlvirtuali_template)
4. [Select using [ ] ](#qsqlselectmaxmin_template)
5. [Where Clause](#select_from_where)
6. [By Clause](#select_by)
7. [Select count](#select_count)
8. [Using operations and functions](#using_ops_functions)
9. [In function](#in_function)
10. [Within function](#within_function)
11. [xbar function](#xbar_function)
12. [Exec query](#exec)
13. [Update](#update_statement)
14. [Delete columns](#delete_columns)
15. [Delete rows](#delete_rows)
16. [Sort Ascending / Descending](#sort_asc_desc)
17. [Renaming / Reordering Columns](#rename_reorder_columns)
18. [Filter By fby](#fby_sql)
19. [xgroup](#xgroup_sql)
20. [Differ](#differ_sql)
21. [Deltas](#deltas_sql)
22. [Next/Prev](#nextprev_sql)
23. [^ Carrot](#carrot_sql)
24. [iasc/idesc](#iasc_sql) 
25. [xrank](#xrank_sql)

## 20. [qSQL Problem Set](#qsql_problem_set)

## 21. [qSQL Joins](#qsql_joins)
1. [Left Join](#left_join)
2. [Plus Join](#plus_join)
3. [Inner Join](#inner_join)
4. [Union Join](#union_join)

## 22. [qSQL Joins Problem Set](#qsqljoins_problem_set)

## 23. [Timeseries Tables Joins](#timeseries_joins)
1. [Asof Time Join](#asof_join)
2. [Union Time Join](#uniontime_join)
3. [Window Time Join](#windowtime_join)

## 24. [Adverbs](#adverbs_header)
1. [Each Both](#eachboth_adverbs)
2. [Each Monadic](#each_monadic)
3. [Each Right / Each Left](#eachright_eachleft)
4. [Scan](#scan_adverb)
5. [Over](#over_adverb)
6. [Each Previous](#eachprevious_adverb)

## 25. [Adverbs Problem Set](#adverbs_problemset)

## 26. [Saving and Loading Data](#importexport_header)
1. [Importing / Loading TXT Files](#txt_import)
2. [Exporting / Saving TXT Files](#txt_export)
3. [Exporting / Saving Tables as txt, csv, excel, and xml files](#tables_exportformat)
4. [Exporting / Saving Tables with New Name](#export_tablenewname)
5. [Importing CSV Files](#csv_import)
6. [Saving to Binary Files](#binaryfile_export)

## 27. [Functional Form](#functional_form)

## 28. [Flat Tables](#flat_tables)
1. [Saving Flat Tables](#flat_tables)
2. [Renaming Flat Tables when Saving](#rename_flatfiles)
3. [Loading Flat Files](#loading_flatfiles)

## 29. [Splayed Database Tables](#splayed_tables)
1. [Get Function - TS](#splay_getfuncTS)
2. [Enumerating Syms - TS](#splay_enusymTS)
3. [Saving Splayed Tables - AQ](#splay_savingAQ)
4. [Memory Considerations](#splay_memoryAQ)
5. [Rearranging Columns/Orders](#splay_arrangecolsAQ)
6. [Retrieving Values from Splayed Columns](#splay_retrievecolsAQ)
7. [Adding New Columns to Splayed Table](#splay_addcolsAQ)
8. [Adding New Row to Splayed Table](#splay_addrowAQ)
9. [Sorting Splayed Tables](#splay_sortAQ)
10. [Enumerating Syms for Splayed Tables](#splay_enusymAQ)

## 30. [Partitioned Database Tables](#partitioned_db)
1. [Saving Partitioned Tables](#savingpartition)
2. [Index Querying](#part_index)
3. [Fill Missing Tables](#part_fillmissing)
4. [Saving Splayed Table into Database Partition](#part_savingsplayed)
5. [Using Functions to Save - no sym](#part_functions)
6. [Using Functions to Save - sym](#part_functionssym)

## 31. [Debugging](#debugging)

## 32. [@ and . Operator](#atanddot_operator)
1. [Square Bracket Notation](#squarebracket_at)
2. [@ Operator](#operator_at)
3. [. Operator](#operator_dot)
4. [Amending List Items using @](#amending_at)
5. [Amending List Items using .](#amending_dot)
6. [Advance use @ Index](#advanced_at)
7. [Using . index with database tables](#advanced_at)
8. [. Zero Dimensional Amend](#zero_dot)
9. [@ Apply](#at_apply)
10. [. Apply](#dot_apply)

## 33. [Racking](#racking)
1. [Loading fakedb.q Script](#loadfakedb)
2. [Racking](#racking)
3. [Alignment](#alignment)

## 34. [Profiling](#profiling)
1. [Comparing Trading Vol vs Average Profile](#profile_one)
2. [Creating Functions for Comparing Profiles](#profiling_func)

## 35. [Trade Analysis](#tradeanalysis)

## 36. [Creating Tables with Random Data](#creatingrandomtable)


<hr>

<a name="kdbintro_header"></a>
## 🔴 1. KDB Basics
[Top](#top)

* KDB is a time series database built upon q
* q is an interpreted language, which means the code is evaluated immediately upon entering
* q is a declarative language, which means you say what you want, not how to do it
* in KDB, all operators are executed RIGHT to LEFT

<a name="assign_intro"></a>
### 🔵 1.1 Assigning Values to Varibles
```q
a: 7
a
```
7

<a name="expression_intro"></a>
### 🔵 1.2 Expressions
```q
6*7
```
42

You can also store an expression in a variable
```q
b: 6*7
b
```
42


<a name="division_intro"></a>
### 🔵 1.3 Division
* division in KDB is expressed as %
* always gives a float response

```q
4 % 2
```
2

<a name="load_intro"></a>
### 🔵 1.4 Loading Scripts
```q
\l scriptname.q
```
```q
/ to show all tables

tables []

```

```q
/ can force output to consol via "show"
/ or can also use '0N!'

/ 
can comment multiple lines
and finish with this
\
```
```q
/ creating script: function whitespace matters!

f:{[a;b;c]
   n:a*b;
   c+n}
f[1;2;3]

/ notice the indentation
```
```q
/ .z.x holds data in string form

\l script.q
.z.x

"sample"
"things"
"show"
"up"
```

<a name="float_intro"></a>
### 🔵 1.5 Floats
* a float is any number with a decimal point
* remember, division will always return a float response

<a name="til_intro"></a>
### 🔵 1.6 Til
* til generates integers until value
* always starts at 0; does NOT include value indicated

```q
til 4
```
0 1 2 3

```q
1+ til 4
```
1 2 3 4

<a name="boolean_intro"></a>
### 🔵 1.7 Booleans
* booleans are true/false statements
* 0b = false
* 1b = true

```q
101b
```
True, False, True

```q
42 = 6*7
```
1b (true)

```q
1 2 3 = 10 2 30
```
010b
* can compare 2 lists of equal length

<a name="over_intro"></a>
### 🔵 1.8 Over

```q
+/ [2 3 4] 
9

/ reduces 2, 3, 4 with +
/ returns SINGLE output 9
/ execuutes "over" entire list
```

```q
0 +/ 2 3 4
9

/ 0 + 9 = 9
```

```q
1 +/ 2 3 4
10

/ 1 + 9 = 10
```

```q
(*/) 2 # 5
25

/ 2#5= 5 5
/ (*/) means multiple over the list 5 x 5 = 25
/ notice you have to use ( ) to contain the (*/)


2 */ 2#5
50

/ notice no more parenthesis if you are multiplying 2 over
/ 2 * 5 * 5 = 50
```

<a name="scan_intro"></a>
### 🔵 1.9 Scan

```q
/ scan is similar to over /, but returns all values

(+\) 2 3 4
2 5 9

/ starts with 2
/ 2 + 3 = 5
/ 5 + 4 = 9
/ accumulates and adds next value
```

```q
(+\) 1 + 0 1 2 3
1 3 6 10

/ 1 2 3 4
/ 1
/ 1 + 2 = 3
/ 3 + 3 = 6
/ 6 + 4 = 10
```

<a name="larger_intro"></a>
### 🔵 1.10 Larger

```q
4 | 5
5

/ | is called style or bar
/ returns the larger of the two operants
```

```q
(|/) til 4
3

/ find the largest value over the list
/ 0 1 2 3 = list
/ compares each element, returns larger 
```

```q
max 10 20 30
30

/ return the largest value over the list
```

<a name="smaller_intro"></a>
### 🔵 1.11 Smaller

```q
10 & 2
2

/ the & is called amper
/ chooses the lesser of the 2
```

```q
(&/) til 4
0

/ return the smallest value over the list
```

```q
min 10 20 30
10

/ return the smallest value  in this list
```

<a name="count_intro"></a>
### 🔵 1.12 Count

```q
count (til 6; 10 20 30)
2

/ counted 2 items in list
```

```q
count each (til 6; 10 20 30)
6 3

/ counts the number of items in EACH nested list
```

<a name="take_intro"></a>
### 🔵 1.13 Take

```q
k: 1 2 3 4
2#k
1 2

/ take # will take the first 2 values of list k

-2#k
3 4

/ take last 2 values of list k

5 # 8
8 8 8 8 8 

/ take 5 values of 8

5 # 1 2 3
1 2 3 1 2

/ take 5 values from this list
/ notice take # wraps around until 5 elements are returned
/ sublist is similar, but wont wrap. 
```

<a name="drop_intro"></a>
### 🔵 1.14 Drop

```q
k: 1 2 3 4

2_k
3 4

/ drops the FIRST 2 values from list k

-2_k
1 2

/ - drops the LAST 2 values from list k

k_2
1 2 4

/ if order is list _ number, then it drops the element at that index position
/ 2nd index position = 3
```

### 🔵 1.14 Cut

```q
l: 1 2 3 4 5 6

2 cut l
(1 2; 3 4; 5 6)

/ cuts list into elements of 2
```
```q
3 cut l
(1 2 3; 4 5 6)

/ cuts list into elements of 3
```

```q
1 4 cut l
(2 3 4; 5 6)

/ 2nd element (4) = cut list by 4
/ first element (1) = AFTER cutting, then drop everything before this element (1) from output
```

```q
2 3 cut l
(3; 4 5 6)

/ drop all elements from 2 and before (1, 2)
/ cut after 3
```

<a name="pluscolon"></a>
### 🔵 1.15 +:

```q
x+:1

/ is the same as x:x+1
```

```q
x*:3

/ is the same as x:x*3
```

<a name="multilinecomment"></a>
### 🔵 1.16 Multi-line Comment

```q
/
to write a multi line comment
start with "/"
end with "\"
\
```

<a name="signum"></a>
### 🔵 1.17 Deltas

```q
prices: 3 2 2 1 5
deltas prices
3 -1 0 -1 4

/ deltas = difference between each element
```

<a name="signum"></a>
### 🔵 1.17 Signum

```q
/ signum conveys whether a value is positive, negative, or 0

signum -2 0 1 3
-1 0 1 1

/ neg, 0, pos pos
```

```q
deltas: 3 -1 0 -1 4
signum deltas
1 -1 0 -1 1

/ pos, neg, 0, neg, neg
```

<a name="cross_operator"></a>
### 🔵 1.18 Cross 

```q
x cross y

/ cross returns all possible combinations of x and y
/ note - does NOT multiply or add
```

```q
1 cross 3 4
1 3
1 4

/ x(1) to y(3)
/ x(1) to y(4)
```

```q
1 2 cross 3 4
1 3
1 4
2 3
2 4

/ x(1) to y(3)
/ x(1) to y(4)
/ x(2) to y(3)
/ x(2) to y(4)
```

```q
/ also works on lists + tables

s:`IBM`MSFT`AAPL
v: 1 2

s cross v
((`ibm;1);(`ibm;2);(`apple;1);(`apple;2);(`msft;1);(`msft;2))
```

```q
([]s) cross ([]v)

s    | v
---------
IBM  | 1
IBM  | 2
MSFT | 1
MSFT | 2
AAPL | 1
AAPL | 2

/ so takes every element of s (IBM, MSFT, AAPL) and combines with every element of v (1 2)
/ the ([] s) returns a table

```q
/ ([]s) returns a single column table

([]s)

s
----
IBM
MSFT
AAPL
```

```q
/ useful for building xbar timeseries

time: 09:00u 09:15u 09:30u 09:45u
sym: `GOOG`IBM

([] sym) cross ([] time)

sym  | time
------------
GOOG | 09:00
GOOG | 09:15
GOOG | 09:30
GOOG | 09:45
IBM  | 09:00
IBM  | 09:15
IBM  | 09:30
IBM  | 09:45
```

<hr>

<a name="casting_header"></a>
## 🔴 2. Data Types & Casting 
[Top](#top)

<a name="datatype_table"></a>
### 🔵 2.1 Datatype Table

type|	size|	char|	num|	notation|	Null Value|	Positive Infinity
-|-|-|-|-|-|-
Mixed List|	|	|	|0|	|	|	
boolean|	1|	b|	1|	1b|	0b|	
byte|	1|	x|	4|	0x26|	0x00|	
short|	2|	h|	5|	42h|	0Nh	|0Wh
int|	4|	i	|6	|42	|0N|	0W
long|	8|	j	|7|	42j|	0Nj|	0Wj
real	|4	|e	|8	|4.2e	|0Ne	|0We
float	|8|	f|	9|	4.2	|0n|	0w
char	|1	|c	|10	|"z"|	" "|	
symbol|	|	s|	11|	`zaphod|	`|	
timestamp|	8|	p	|12|	2011.07.08D21:48:48.703125000|	0Np	|0Wp
month|	4|	m|	13|	2006.07m	|0Nm	|0Wm
date|	4	|d|	14|	2006.07.21	|0Nd	|0Wd
datetime	|4	|z	|15|	2006.07.21T09:13:39	|0Nz	|0Wz
timespan	|8|	n	|16|	0D21:56:26.421875000	|0Nn	|0Wn
minute|	4	|u	|17|	12:11|	0Nu|	0Wu
second	|4|	v	|18|	12:11:17|	0Nv	|0Wv
time	|4	|t	|19	|09:01:02:042	|0Nt	|0Wt
enum	|4|	*|	20-77	|`u$v|	|
table|	|	|98	|([] c1:ab`c; c2:10 20 30) | 
dictionary	|	|	|99	|`a`b`c!!10 20 30 |

<a name="date_type"></a>

```q
Given:
d: 2011.02.22

d.year
d.mm
d.month
d.dd

2011i
2i
22i 
```

<a name="time_type"></a>
### 🔵 2.2 Time
```q

t: 11:02:58:000

t.hh
t.mm
t.minute
t.ss
t.second

11i
2i
11:02
58i
11:02:85 
```
```q
Current Time
.z.t

Current Date
.z.d

Current Timespan
.z.n

Current TimeStamp
.z.p
```

```q
/ Timestamp Examples

depth
time                       sym  price
-------------------------------------
2021-11-07T08:04:21.425000 YHOO 33.99
2021-11-07T08:14:59.215000 ORCL 35.16
2021-11-07T08:21:30.944000 NOK  42.01

meta depth

/ time column is datatype p = timestamp

c    |t|f|a
------------
time |p| |		
sym  |s| |g
price| |f|		

/ extract the timestamp column

select time from depth

time
--------------------------
2021-11-07T08:04:21.425000
2021-11-07T08:14:59.215000
2021-11-07T08:21:30.944000

/ extract the date from timestamp

select `date$time from depth

time
----------
2021-11-07
2021-11-07
2021-11-07

/ extract the time from timestamp

select time.time from depth
select `time$time from depth

time
------------
08:04:21.425
08:14:59.215
08:21:30.944
```


<a name="cast_type"></a>
### 🔵 2.3 Casting
```q
/ casting = changes one datatype to another type that's compatible
/ parsing = converting from a string to a native type
/ x $ y 
/ x = target type
/ y = source type
/ Casting y to x
```

Casting strings to sym

```q
"S" $ "a","b","c"
`abc

/ use capital "S" to cast to sym
/ or can also use `
```

Casting syms to strings 

```q
string `abc
"abc"

/ sym to string, simply use "string" function
```

Casting int to dates

```q
`date$2
2000-01-03d

/ 2nd day of the millennia
```

Casting int to time

```q
`time$2
00:00:00.002t

/ 2 + 00:00:00.000
```

Casting int to month

```q
`month$2
2000.03m

/ KDB time starts at 2000.01.01 
/ 2 + 2000.01.01
```

Casting int to minute

```q
`minute$2
00:02

/ takes 2 + 00:00
```

Casting int to seconds

```q
`seconds$2
00:00:02
```
Casting ints/0 to booleans

```q
`boolean$9
1b

/ casting a boolean will always be true (1b), unless its 0

`boolean$0
0b
```

Converting list of syms to string

```q
string `a`b`c`d`e
("a";"b";"c";"d";"e")

/ converting list of syms to singular string

raze string `a`b`c`d`e
"abcde"
```
```q
-7h

/ a negative type means it's an atom!
```

Float Rounding when Casting to Int

```q
`int$3.1
3i

`int$3.9
4i

/ will round accordingly up or down
```

Casting a date to a symbol

```q
`$2020.01.01
error

/ can't cast a date directly to a sym
/ need to cast as string first

`$string 2021.01.01

/ cast as string first, then cast as sym
```

<a name="enu_cast"></a>
### 🔵 2.4 Enumeration
* enumeration is converting a list of values to a defined domain which restricts values to that domain

```q
suits:`hearts`clubs`spades`diamonds
l: `hearts`clubs`diamonds
el: `suits$l

/ enumerate all symbols in list l under same domain as suits
/ will enforce/restrict their type as same domain 
```

```q
el,:`apple
cast

/ if you try adding a value that is NOT within that domain (apple), you will get a cast error
```

```q
el[0]:`pear
cast

/ also cannot update value if not in the existing domain
```

<hr>

<a name="casting_problemset"></a>
## 🔴 3. Data Types & Casting & Enumeration Problem Set
[Top](#top)

**🔵 3.1 What is the syntax to add to a list**
```q
el, : apple

/ use the ,: operator
```


<hr>

**🔵 3.2 Show 3 ways to conver float 4.5 to an integer**
```q
`int$4.5
"i"$4.5
6h$4.5
```

<hr>

**🔵 3.3 Given strings "2001.02.02" and "2003.08.09", parse the strings into KDB dates**
```q
"D"$("2001.02.02";"2003.08.09")

/ these are strings which you are trying to parse into the date datatype
/ have to use upper case when parsing
```


<hr>

**🔵 3.4 Given the mixed list L: ("100.1";"hello";"10"), convert elements to float, char, and int**
```q
"F*I"$("100.1";"hello";"10")
100.1
"hello" 
10i

/ have to use capital F and I
/ the astrik is used for strings
```

<hr>

**🔵 3.5 Create empty symbol list s**

```q
s: `symbol$()
```

**Append integer 3 to list s**
```q
s ,: 3
type 

/ error because 3 is an int and the list is enumerated as syms

```
**Append symbol ooo to list s**
```q
s,:`ooo
```

<hr>

**🔵 3.6 Create an enumeration t containing values p q r that is restricted to domain s**
```q
s: `symbol$()
t: `s$`p`q`r

/ t is now an enumeration which only contain domain s (symbols)
```

**🔵 3.7 Insert new value u into t**

```q
s,:`u
error

/ since t is restricted to domain s, need to first add u into s before adding to t

t,:`u
`p`q`r`u

/ now it works

```

<hr>

<a name="lists_header"></a>
## 🔴 4. Lists
[Top](#top)

<a name="simple_list"></a>
### 🔵 4.1 Simple Lists
```q
L1: 1 2 3 4
L2: 1;2;3;4
L3: 1 2 3 4i
L4: 1.0 2.0 3.0 4.0
L5: `p`q`r
L6: ("a";"b";"c")
```
* simple lists with same datatype don't need semi colons
* L3 = list of ints
* L4 = list of floats
* L5 = list of syms
* L6 = list of chars
 
<a name="mixed_list"></a>
### 🔵 4.2 Mixed Lists
```q
L7: (1; `p; 200.)
```
* mixed list of an int, sym, and float

```q
type L7
0h
``` 
* null because its a mixed list

<a name="empty_list"></a>
### 🔵 4.3 Empty Lists

```q
L: ()
count L
0
```

<a name="atom_list"></a>
### 🔵 4.4 Single Item Lists
```q
L9: enlist `C
```
* have to use enlist for single item lists

<a name="join_lists"></a>
### 🔵 4.5 Joining Lists

```q
atom to atom

1,2
1 2
```

```q
atom to list

`a, `b`c`d
`a`b`c`d
```

```q
list to list

1 2 3, 4 5 6
1 2 3 4 5 6

a: 1 2 3
a,:4
1 2 3 4

/ uses join assign function
```

<a name="retrieve_list"></a>
### 🔵 4.6 Retrieving from Lists using Indexing

```q
L: 10 20 30

L[0]
L[1 2]
L 1 2 3

10
10 20
10 20 30

/ retrieval uses 0 indexing logic (count starts with 0)
/ notice you DONT use colons : when retrieving from lists
```

<a name="update_list"></a>
### 🔵 4.7 Update List Values
```q
L: 10 20 30

L[0 1 2] : 40 50 60
40 50 60

/ notice you use colon : to update values
```

<a name="nest_list"></a>
### 🔵 4.8 Nested Lists (Lists of Lists)

```q
list: (1 2; 3 4; 5 6; 7 8)

first each list
1 3 5 7

/ returns first element of each nested list
```

```q
L: 10 20 30 40 50
K: 0.1 0.2 0.3
NL: (L; K; `pp`qq`rr)

/ NL is a list of 3 nested lists: L, K, and the syms

NL [0 2]
10 20 30 40 50
`pp`qq`rr

/ So think of list NL as 3 separate lists.
/ Retrieve index location 0 and 2, so returned the first and 3rd list
```

```q
NL[(0 1;2)]
(10 20 30 40 50; 0.1 0.2 0.3)
`pp`qq`rr

/ if your argument is a nested list, the output will also be nested list
/ the shape of your result will = the shape of your argument
/ 0 = first row (of l)
/ 1 = second row, but output is grouped as nested list together with 0
/ 2 = second argument = new row
```

index to depth

```q
NL [0][0]
10

/ retrieves index position 0 (first list = list L) 
/ and the first value from that list (index location 0)
```

<a name="matrix_list"></a>
### 🔵 4.9 Matrix

```q
m: (10 20 30; 40 50 60; 70 80 90)

0 | 1 | 2
----------
10| 20| 30
40| 50| 60
70| 80| 90

/ when retrieving in a matrix, always go ROW, then COLUMN
```

```q
m[1; ]
40 50 60

/ retrieves row 2 (index position 1 - row)
```

```q
m[ ; 1]
20 50 80

/ ignores row (blank),
/ retrieves 2nd column (index location 1 - col)
```

What happens when retrieve outside of range?

```q
/ assume irregular matrix

dl: (1 2 3; `a`b`c; 1.0 2.0)

 1  |  2  | 3
 a  |  b  | c
1.0 | 2.0 |  

dl[;2]
3
`c
0N 

/ returns null bc doesnt exist
/ want 3rd column aka 2nd index position for col
```


<a name="sublist_list"></a>
### 🔵 4.10 Retrieving from list using Sublist

```q
2 sublist 1 2 3 4 5
1 2

/ takes first 2
```

```q
-2 sublist 1 2 3 4 5
4 5

/ takes last 2
```

```q
10 sublist 1 2 3 4 5
1 2 3 4 5

/ take only what's available
/ won't wrap around like take
```

```q
2 2 sublist 1 2 3 4 5
3 4

/ from index position 2, take 2 items
```

<a name="find_list"></a>
### 🔵 4.11 Find in List

```q
/ ? find will return the index position

1 2 3 4 5 ? 3
2

/ find index position of 3
```
```q
1 2 3 4 5 ? 7
5

/ find index position 7
/ not found, returns max index + 1
```
```q
1 2 2 3 4 ? 2
1

/ find index position of 2
/ multiple occurence, only returns first
```

<a name="random_list"></a>
### 🔵 4.12 Random Operator in Lists

```q
5 ? 1 2 3 4 5
1 3 2 2 4

/ pick 5 random items from list
```

```q
5 ? 10
8 5 5 9 2

/ pick 5 random items less than 10
```
```q
-5 ? 10
8 5 1 9 2

/ pick 5 distinct random items less than 10
```

```q
5 ? `2
`ah `lj `ef `ie `jf

/ pick 5 random syms with length 2
```

```q
5 ? " "
"lwhev"

/ pick 5 random chars 
```

```q
list: 1 2 3 4 5

list ? 2
1

/ from list, find 2

2 ? list
3 4

/ from list, return 2 random elements
```

<a name="count_list"></a>
### 🔵 4.13 Count Operator in Lists

```q
count 1 2 3 4
4

/ counts number of elements in list
```
```q
count enlist 1 2 3 4
1

/ counts the first dimension of the enlisted structure
```
```q
count (1 2 3;4 5 6)
2

/ counts number of nested lists
```
```q
count each (1 2 3; 4 5 6)
3 3

/ counts number of elements in each nested list
```

<a name="raze_intro"></a>
### 🔵 4.14 Raze

Raze collapses one level of nesting

```q
t: (1 2; 3 4 5) / this is a nested list containing 2 levels
1 2
3 4 5

raze t
1 2 3 4 5 

/ collapses 1 level of nesting and joins all items together
```

```q
/ 2 levels of nesting

b: (1 2; (3 4; 5 6); 7; 8)
1 2
    3 4
    5 6
7
8

raze b
1
2
3 4
5 6
7 
8

/ collapses 1 2 to 2 levels
/ collapses 3 4 up a level
```

```
/ flatten all levels raze/

b: (1 2; (3 4; 5 6); 7; 8)
raze/ [b]
1 2 3 4 5 6 7 8

/ using raze/[x] will flatten all levels
```

```q
string `a`b`c
"a","b","c"

raze string `a`b`c
"abc"
```

<a name="union_lists"></a>
### 🔵 4.15 Union Lists

```q
1 2 3 union 3 4 5
1 2 3 4 5 

/ union returns only the distinct elements in both lists
```

<a name="where_lists"></a>
### 🔵 4.16 Where clause with Lists

```q
/ if you have 2 lists, you can use indexing to retrieve corresponding values in lists

size: 100 300 50 70
price: 4 8 6 2

price > 5
0110b

/ using comparison operator on list returns list of booleans

where price > 5
1 2

/ where + comparison operator = shows index position 

size where price > 5

/ returns value from 2nd list using index position from original list

avg size where price > 5

/ can perform calc on 2nd list too (avg price)
```
<a name="contain_ops"></a>
### 🔵 4.17 Contain

```q
/ in operator returns booleans

5 in 1 2 3 4
0000b

/ is x in y? 
/ no, so 0
```

<a name="except_ops"></a>
### 🔵 4.18 Except

```q
1 2 3 4 except 3
1 2 4

/ returns x except y
/ return the list except 3
```

<a name="inter_ops"></a>
### 🔵 4.19 Inter

```q
1 2 3 inter 2 3 4
2 3

/ x inter y
/ returns items in both x and y
/ inter returns values occuring in both lists
```

<a name="distinct_ops"></a>
### 🔵 4.20 Distinct

```q
/ distinct syms

distinct `a`a`b`b`c`c
a b c

/ distinct only returns distinct items/values
```

```q
/ distinct ints

distinct 1 2 2 3 3 4 4 5
1 2 3 4 5
```

```q
/ distinct lists

distinct 100?5
4 0 1 3 2

/ return only the distinct numbers
/ from 100 random numbers between 0-4
```

<hr>

<a name="list_problemset"></a>
## 🔴 5. Lists Problem Set
[Top](#top)

**🔵 5.1 What is the difference between 3 ? 10 and 3 ? 10 20 30**

```q
/ atom ? atom
3 ? 10

/ returns 3 random numbers from 0-10

/ atom ? list
3 ? 10 20 30
10 10 30

/ returns 3 random numbers from the list
```

<hr>

**🔵 5.2 Create a general list containing symbol p, boolean 1b, and long 1000200j**

```q
GL: (`p; 1b; 100200j)

/ general lists with different data types have to be contained within ( ) with ; separating each item
```

<hr>

**🔵 5.3 Given the following**

p: 100 200 300 400 500 600 <br>
t: "say hello world to bob" <br>
m: (1 2 3; 10 20 30; 100 200 300) <br>

**Retrieve first 3 items from p**
```q
3#p
100 200 300
```

<hr>

**🔵 5.4 From t, retrieve the list "sold"**

```q
t?"sold"
0 8 6 14

/ retrieve index positions for chars in string "sold"

t[0 8 6 14]
"sold"

/ then you can retrieve chars using indexing
```

<hr>

**🔵 5.5 Create the nested list ("shoot";"bob") by indexing into t**

```q
t?"shoot"
0 4 8 8 16

t? "bob"
19 8 19

t(0 4 8 8 16; 19 8 19)
("shoot";"bob")

/ find index location of chars in string "shoot" and "bob"
/ then retrieving those index positions (letters) to spell out
/ since you are retrieving a list of chars, need to use () instead of [ ]
```

<hr>

**🔵 5.6 Change the last number in p to 1000**

```q
p[5]: 1000

/ upsert function (update insert)
/ find index location 5, replace value with 1000
```

<hr>

**🔵 5.7 Find the 3 highest numbers in p**

```q
3#desc p
100 500 400

/ take 3 numbers from descending list p
```

<hr>

**🔵 5.8 Find values of p that are below the mean**

```q
p where p<avg p
100 200 300 400
```

<hr>

<a name="primitive_header"></a>
## 🔴 6. Primitive Operations
[Top](#top)

<a name="add_list"></a>
### 🔵 6.1 Addition

```q
10 + 10 20 30
20 30 40
```

```q
10 20 30 + 1 2 3 
11 22 33
```

```q
10 20 30 + 1 2
length

/ error because different list lengths
```

<a name="compare_lists"></a>
### 🔵 6.2 Comparing Lists

```q
1 2 3 = 1 2 3 
111b

/ comparing 2 lists will result in boolean answer (true true true)
```

<a name="match_diff"></a>
### 🔵 6.3 Match and Equal Differences

```q
Equals
1 2 3 = 1 2 3 
1b

/ Equals is type tolerant. allows for some rounding. accomodates different data types
```

```q
Match
1 2 3 ~ 1.0 2.0 3.0
0b

/ Match will check value and data type. Requires EXACT match
/ Single item return (false)
```

<a name="basic_operations"></a>
### 🔵 6.4 Basic Operations

l: 10 20 30 40 50 

```q
max l
min l
med l
avg l
dev l
sqrt l
x xexp y

/ med = median
/ dev = standard deviation
/ xexp = to the power of
```

<a name="mod_operations"></a>
### 🔵 6.5 Division Remainders Mod

```q
11 21 31 mod 2

1 1 1
/ modulus function returns remainder after dividing it
```

<a name="running_sums"></a>
### 🔵 6.6 Running Sums/Moving Windows
```q
sums l
prds 1
maxs l

/ running sums, running products, running max
```

```q
/ moving window sums

l: 0 10 20 30 40 50 

3 msum 1
0 10 30 60 90 120

/ initial values less than window returns values 
/ 0, 10 (less than window 3)
/ 0 + 10 + 20 = 30
/ next window 10 + 20 + 30 = 60
```

```q
3 mmax 10 30 20 30 20
10 30 30 30 30

/ returns MAX in window of 3
/ initial values less than window returned (10, 30)
/ next element also 30, since still max
```

<a name="reverse_ops"></a>
### 🔵 6.7 Reverse

```q
/ reverse ints

reverse 1 2 3
3 2 1
```

```q
/ reverse strings

reverse "hello"
"olleh"
```

<a name="uppercase_ops"></a>
### 🔵 6.8 Upper/Lowercase

```q
upper "adsf"
ADSF


lower "ADSF"
adsf

/ converts a sequence of characters to upper or lower
```

<a name="uppercase_ops"></a>
### 🔵 6.9 Timing Queries

```q
/ KDB is all about speed
/ \t function allows you to time your queries
```

Example 1: Vector Addition Method

```
n: 1000000

a:n?100f
b:n?100f

/ a and b are lists of a million random floats

\t r1:a+b
1

/ query time took less than 1 millisecond
```

```q
/ vector addition is very fast

\t:100 r1:a+b
120

/ \t: 100 = run it 100x
/ query time still only 120 ms
/ much faster than executing a while loop 
```

Example 1: Iterative method (while loop)

```q
a:n?100f
b:n?100f

/ a and b are lists of a million random floats

r2: n#0f
/ first setup empty results list

i: 0
/ then an setup index which will cycle through the 2 lists
/ initialized at 0

while[i<n;r2[i]:a[i]+b[i];i+:1]

/ i<n = while our index i is less than n
/ r2[i] = the results list at position i is equals to
/ a[i]+b[i] = the value of a at i plus b at i
/ i+:1 = then increment i by 1

/ if you time the iterative while loop:

\t while[i<n;r2[i]:a[i]+b[i];i+:1]
1388

/ much slower than vector addition
```

Example 1: Adverb method using EACH '

```q
r3:+'[a;b]

/ add EACH element of a and b

/ if you time it

\t r3:+'[a;b]
111

/ faster than while loop, but still slower than vector addition
```

Example 2

```q
/ generate list of 1mm ints from 0-199

d: 1000000?200

/ OBJECTIVE: sum all values > 100
```

While Loop

```q
i:0
r1:0

while[i<count d; if [d[i]>100;r1+:d[i]]; i+:1]

/ runs while i is less than the count of the list
/ if value of list at index i is greater than 100
/ then add to value of result
```

Adverb Version

```q
/ uses a lambda function which
/ adds x to the result if x > 100
/ and does this for each element x in list d

r2: 0
{if[x>100;r2+::x];}each d

/ faster than using while loop
```

Vector Version

```q
d: 1000000?200

sum d where d > 100

/ much faster than while loop or adverb
/ and much easier logically
```

<hr>

<a name="primitive_problemset"></a>
## 🔴 7. Primitive Operations Problem Set
[Top](#top)

**🔵 7.1 Find index location for "ryan" in "hello ryan where is ryan"

```q
"hello ryan where is ryan" ss "ryan"
6 20

/ ss = string search
/ returns index location
/ ryan appears twice; at the 6th and 20th index location
```

<hr>

**🔵 7.2 replace "ryan" with "john"**

```q
ssr["hello ryan where is ryan";"ryan";"john"]
hello johhn where is john

/ ssr = search string replace function
/ first arg = input string
/ second arg = what to replace
/ third arg = what to replace with
```

<hr>

**🔵 7.3 Find the number of days in 2004**
```
2005.01.01 - 2004.01.01
366

```

<hr>

**🔵 7.4 Given list L and K, find the common numbers in both lists** <br>
l: 7 5 13 20 19 17 30 <br>
k: 7 17 200 300 400 1000 <br>

```q
l inter k
7 17

/ inter = finds same values in x inter y
```

<hr>

**🔵 7.5 Find the sum of the first 5 numbers in l**
```q
sum 5#l
64

/ take first 5 numbers from l
/ then sum them together
```

<hr>

**🔵 7.6 Find the result when you remove the last 2 items from k**
```q
-2_k
7 17 200 300

/ drop last 2 items from k
```

<hr>

**🔵 7.7 Return only numbers in l that are wholly divisible by 5**
```q
l mod 5
2 0 3 0 4 2 0

/ returns remainder where l divide by 5
/ 0 means fully divisible

l where not l mod 5
5 20 30

/ l where not l mod 5 = 

/ return value where l mod 5 = 0
/ not l mod 5 will return the values at 0
```

<hr>

**🔵 7.8 Subtract the average of list l from max value in list k**

```q
max[k] - avg [l] 
984.14

/ or also:

max k - avg l
9784.14
```

<hr>

**🔵 7.9 Generate list p of 1000 random integers between 0 and 100. Find all values in p that are square numbers**
```q
p: 1000?100
a: sqrt p

/ a = list containing square roots of every number in p
/ a will contain both ints and floats

a = `int$a

/ cast a as an integer (whole number)
/ since a is made up ints and floats

p where a=`int$a

/ return value in p where a = whole number (square numbers)

count p where a=`int$a

/ count number of p = square numbers
```

<hr>

<a name="dict_header"></a>
## 🔴 8. Dictionary
[Top](#top)

```q
/ A dictionary is a data structure that maps between a domain of keys and a range of values
/ left of ! = list of keys
/ right of ! = list of values
/ can map from any TYPE of domain to any TYPE of range
```

<a name="dict_from_list"></a>
### 🔵 8.1 Different Ways to Construct Dictionaries

Construct Dictionary using 2 Lists

```q
k:`apple`plum
v:`green`purple
d:k!v

key   | value
--------------
apple | green
plum  | purple
```

Construct Dictionary using atoms

```q

d: `a`b`c!1 2 3

key | values
------------
a   | 1
b   | 2
c   | 3
```
Construct Dictionary using atoms and variables (strings)

```q
/ atom ! string

a: "yes, its red"
b: "yes, its blue"

d: `red`blue ! (a;b) 

key  | value
--------------
red  | yes, its red
blue | yes, its blue

/ a and b are simply strings stored as a variable
/ VALUES for variables have to be encased by ( ) and separated by ; 
```

Construct Dictionary using atoms and variables (ints)

```q
c: 1
d: 2

d2: `one`two ! (c;d)
d2

key | value
------------
one | 1
two | 2

/ c and d are ints stored as a variable
/ VALUES for variables have to be encased by ( ) and separated by ; 
```

<a name="retrieve_dict"></a>
### 🔵 8.2 Retrieving Values from Dictionaries

Given dictionary d, 3 ways to retrieve a

```q
d:`a`b`c!1 2 3

key | values
------------
a   | 1
b   | 2
c   | 3

d[`a]
d`a
d@`a

/ note - this only returns the values. if you want to return a dictionary, use # take

`a`b # d

key | value
-----------
a   | 1
b   | 2

/ key # dict_name
/ returns a dictionary

(enlist `a) # d

key | value
-----------
a   | 1

/ for single row retrieval, need to use enlist
```

```q
/ retrieves all keys in d

key d
a b c
```

```q
/ retrieves all values in d

value d
1 2 3
```

```q
/ Retrieve multiple values

d @ `a`b`a`
1 2 1 1
```

<a name="index_retrieve_dict"></a>
### 🔵 8.3 Index Retrieve

```q
dc:`c1`c2!(10 * til 5; 1+ til 3)

key| value
------------------
c1 | 0 10 20 30 40
c2 | 1 2 3

dc[`c2]
1 2 3 

/ retrieves values in key c2

dc[`c2;2]
3

/ retrieves from key c2, index position 2 (0 1 2)

dc[ ; 1]

key| value
----------
c1 | 10
c2 | 2 

/ takes index position 1 from values (2nd column)
```

<a name="take_dict"></a>
### 🔵 8.4 Take

```q
/ another form of retrieving from dictionaries

2#d

key | value
----------
a   | 1
b   | 2

/ take first 2 entries from d

`a`b#d

key | value
-----------
a   | 1
b   | 2

/ take keys `a and `b and retrieve its values from d

d`a`b
1 2

/ retrieve keys `a and `b and return its values from d
```

```q
/ retrieving single row from dictionary

(enlist`a)#d
1

/ have to use enlist when retrieving a single item from dictionary
```

<a name="drop_dict"></a>
### 🔵 8.5 Drop

```q
/ drop ROWS in dictionaries

key | value
----------
a   | 1
b   | 2
c   | 3

2_d

key | value
-----------
C   | 3

/ drop first 2 rows from dictionary d
```

```q
/ drop keys + values from dict

d: `a`b`c ! 1 2 3

key | value
----------
a   | 1
b   | 2
c   | 3

`b _ d

key | value
----------
a   | 1
c   | 3

/ drop key b and its associated value from the dict
/ can drop multiple keys at once
```


<a name="upsert_dict"></a>
### 🔵 8.6 Upsert

```q
d [`e]: 99

key|value
--------
a  |1
b  |2
c  |3
e  |99

/ upsert = update insert
/ if key exists, will update value
/ if key doesn't exist, will insert new key + value

```
<a name="upsert_dict"></a>
### 🔵 8.6 Nested List within Dictionaries

```q
dict:`alpha`bravo`charlie!((1 2 3);(4 5 6); (7 8 9))

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 7 8 9
```

Adding new row to dict via join

```q
dict,(`delta`echo)!(10 11 12;13 14 15)

/ join not in place, which means its not saved to dict
/ to update the underlying table, need to use join assign ,:
```

Adding new row via Join Assign

```q
dict,:(`delta`echo)!(10 11 12;13 14 15)

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 7 8 9
delta   | 10 11 12
echo    | 13 14 15

/ join assign adds the row + updates underlying dict
```

Upserting Rows

```q
dict[`charlie]: 100 200 300

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 100 200 300
delta   | 10 11 12
echo    | 13 14 15

/ updates values based on indexed key (`charlie)
```

Inserting a single row to dict (enlist!)

```q
dict,:(enlist `golf)! enlist 10

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 100 200 300
delta   | 10 11 12
echo    | 13 14 15
golf    | 100

/ need to use enlist when adding / upserting single row to dict
/ for dict enlist, need to enlist both key AND value

```

```q
/ avg + avg each dictionary

dict:`alpha`bravo`charlie!((1 2 3);(4 5 6); (7 8 9))

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 7 8 9

avg dict
4 5 6

/ avg nested dictionary = average per COLUMN

avg each dict

key     | value
---------------
alpha	| 2
bravo	| 5
charlie | 8

/ avg each nested dictionary = average per ROW
```

<a name="multi_key_dict"></a>
### 🔵 8.7 Multi Key Dictionaries

```q
md: (`a`b;`c`d;`e`f) ! 1 2 3

/ created a dictionary md with 2 keys for every 1 value
/ ; separate the various rows

key | value
----------
a b | 1
c d | 2
e f | 3
```

<a name="repeat_key_dict"></a>
### 🔵 8.8 Repeat Keys

```q
/ You can technically have multiple repeat keys, but this is NOT recommended

dk: 1 2 3 1 ! `a`b`c`d

key| values
-----------
1  | a
2  | b
3  | c
1  | d

/ notice key 1 is repeated

dk[1]
a

/ if you attempt to retrieve a repeated key, it will only return the first value
```

<a name="find_dict"></a>
### 🔵 8.9 Find Operator ? on Dictionaries

```q
dict: `a`b`c`d!1 2 3 4

Key | Value
-----------
a   |	1
b   |	2
c   |	3
d   |	4

dict ? 3
`c

/ ? FIND value 3, and return the key
/ ? FIND works for both lists and dictionaries
```

<a name="dict_opt"></a>
### 🔵 8.10 Dictionary Operators

sum 
```q
d: `a`b`c ! 1 2 3

sum d
6

/ sums all values together, returns single atom
```
avg

```q
avg d
2

/ avg of values
```

neg

```q
neg d

key|value
--------
a  | -1
b  | -2
c  | -3

/ turns all values negative
```
% all values

```q
d%100
key|value
---------
a  |0.01
b  |0.02
c  |0.03

/ divides all values by 100
```

<a name="dict_adding"></a>
### 🔵 8.11 Adding / Joining Dictionaries

```q
/ partial match on keys

d1:`a`b`c!1 2 3
d2:`a`b`d!1 2 3

d1+d2
d1,d2

key|value
--------
a  | 2
b  | 4
c  | 3
d  | 3

/ finds matching keys, add values together
/ if no matching keys, simply returns original values (kinda like union)
```

```q
/ keys match, values don't

d1: `a`b`c ! 1 2 3
d2: `a`b` ! 100 200

d1, d2

key|value
--------
a  | 100
b  | 200
c  | 3

/ when joining dict, if keys match, but values are different
/ 2nd dict over-rides value of first dict
```

<a name="dict_boo"></a>
### 🔵 8.12 Boolean Comparisons

```q
dict: `a`b`c`d ! 1 2 3 4

dict = 2

Key | Value
-----------
a   | 0b
b   | 1b
c   | 0b
d   | 0b

/ compares every value in dict =2
/ and returns a dictionary of booleans
```

boolean comparison 2 dictionaries

```q
d1: `a`b`c ! 1 2 3
d2: `a`d ! 4 5

d1 < d2

Key | Value
-----------
a   | 1b
b   | 0b
c   | 0b
d   | 1b

/ when comparing 2 dict using comparison operator
/ if no match on key, returns 0 false
```

<hr>

<a name="dict_problemset"></a>
## 🔴 9. Dictionary Problem Set
[Top](#top)

**🔵 1. Given the below dictionary, find the type, the keys, and its values**
```q
d:`p`q`r`s!10 20 40 100

key|value
---------
p  | 10
q  | 20
r  | 40
s  | 100

type d
99h

key d
p q r s

value d
10 20 40 100
```

**🔵 2. Add new entry u 200 to list d**
```q
d[`u]: 200

key|value
---------
p  | 10
q  | 20
r  | 40
s  | 100
u  | 200

/ upsert. will update if key exists, if not, will append it
```

**🔵 3. Change value of p to 2**
```q
d[`p]:2

key|value
---------
p  | 2
q  | 20
r  | 40
s  | 100
u  | 200
```

**🔵 4. Create dictionary d2, by TAKING values of p q r from dictionary d**
```q
d2:`p`q`r#d

key|value
---------
p  | 2
q  | 20
r  | 40

/ when TAKE # from dict, output is a dict contains both keys + values
```

**🔵 5. Find common keys in d and d2, and retrieve keys + values from combined d+d2

```q
d+d2

key|value
---------
p  | 4
q  | 40
r  | 80
s  | 100
u  | 200

/ wrong - adds ALL values together
/ includes non common keys
```

```q
d inter d2
2 20 40

/ dict inter dict will return values occuring in both dicts
/ but you want to return both keys + values, not just values
```

```q
key[d] inter key[d2]
`p`q`r

/ retrieve keys in both d and d2
/ inter = retrieves common values 
/ so this will return the keys in both dict
```

```q
/ now that you know the common keys, use TAKE
/ to retrieve a dict from combined d + d2

(key[d] inter key[d2]) # d + d2

key|value
---------
p  | 4
q  | 40
r  | 80

/ combining together, you take the keys occuring in both dict from d1 + d2
/ and show its values
```

**🔵 6. Given the 2 dictionaries below, find those who are greater than 1.7m in height**

```q
dheight:`john`mark`luke`paul`ian`peter!1.5 1.6 1.7 1.8 1.9 1.4
dweight:`john`mark`luke`paul`ian`peter!81 72 88 91 55 110

dheight
key  | value
------------
john | 1.5
mark | 1.6
luke | 1.7
paul | 1.8
ian  | 1.9
peter| 1.4

dweight
key  | value
------------
john | 81
mark | 72
luke | 88
paul | 91
ian  | 55
peter| 110

dheight > 1.7

key  |value
-----------
john | 0b
mark | 0b
luke | 0b
paul | 1b
ian  | 1b
peter| 0b

/ comparison operator on a dict returns a table of booleans

where dheight > 1.7
paul ian

/ where = returns the keys
```

**🔵 7. Find the average height of people who weight over 90**
```q
where dweight > 90
paul peter

dheight where dweight > 90
1.8 1.4

avg dheight where dweight > 90
1.6
```

**🔵 8. Find the body mass index (weight) / (height x height)**
```q
dweight%dheight*dheight

key  | value
------------
john | 36.0
mark | 28.1
luke | 30.4
paul | 28.0
ian  | 15.2
peter| 56.1
```

<hr>

<a name="functions_header"></a>
## 🔴 10. Functions
[Top](#top)

<a name="define_func"></a>
### 🔵 10.1 Defining & Calling Functions

```q
/ create function f
/ with has argument a
/ and multiples a to itself

f: { [a] a * a}

/ now call this function f with a = 3

f[3]
9

/ [a] = [ ] defines the argument (a)

alternative syntax:

f 3
f @ 3

/ these also all work
```

Function with 2 Arguments

```q
/ create function named add
/ with 2 arguments, a and b

add: { [a;b] a + b}
add [3;5]
8

/ multi argument function
/ [a;b] = defines arguments A and B
```

Multi Statement Functions

```q
/ the answer returned is the LAST expression evaluated in function
/ statements separated by semi colons

f:{[arg1;arg2;arg3] t:arg1*arg2*arg3; t*2}
t[1;2;3]
12

/ 1*2*3 = 6
/ 6*2 = 12
```

Supressing Functions

```q
/ can supress the function by adding ; to end 

f:{[arg1;arg2;arg3] t:arg1*arg2*arg3; t*2;}
t[1;2;3]
-

/ nothing returned
```

Forcing Function Output

```q
/ can force an output by adding semi colon :

f:{[arg1;arg2;arg3] t:arg1*arg2*arg3; :t*2; t+3}
t[1;2;3]
12

/ semi colon in front of 2nd expression so it will force that output
/ colon halts everything after 
```

Special Built in Functions

```q
/ plus function

+[1;2]
3

f:+
f[1;2]
3
```

### 🔵 10.2 Types of Function Arguments

```q
/ niladic (accept no arguments)

f:{[] 1+2+3}
f[]
6

/ call func by passing empty [ ] 
/ if you call func with arg, it will be ignored

f:{[] 1+2+3}
f[3]
6
/ argument 3 is ignored

/ monadic (accepts 1 argument)

f:{[arg1] arg1+10}
f[2]
12

/ implicit (up to 3 arguments: x, y, z)

f:{x+10}
f[2]
12

/ don't need to declare argument; x will be first parameter passed through function

/ diadic (accepts 2 arguments)

f:{[a;b] a*b}
f[2;4]
8

/ triadic (accepts 3 arguments)

f:{x*y*z}

/ multivalent (must define parameters)

f:{x*y*z*a}
f[1;2;3;4]
`rank

/ this doesnt work. you have to define argument if more than 3

f:{[x;y;z;a] x*y*z*a}
f[1;2;3;4]
24

/ now this works
```

```q
/ max amount of arguments is 8!
/ can get around by using dictionary as argument

d:(10?" ")! 1+til 10
f:{[d] (+/)d}
f[d]
55
```

<a name="anon_function"></a>
### 🔵 10.2 Anonymous Functions

```q
/ in q, you do NOT need to assign a function to a variable name
/ this is known as an ANONYMOUS function (lambda function)

{[a] a*a} 6
36

/ notice how there's no variable assignment to function
/ you can simply call your argument after the body of function

/ alternative syntax:

{[a] a*a}[6]
36
```

Multiple ways to CALL anonymous function

```q
{x+y} [3;4]
7

{x+y} [3;] 4
7

{x+y} [3] 4
7

{x+y} [;4] 10
7
```

<a name="anon_function"></a>
### 🔵 10.2 Anonymous String Function Problem Set (AQ)

```q
/ create a function that uses SSR (string search replace)
/ to convert sym `welcome to string "welcoME"

/ quick reminder on SSR

ssr["hello ryan where is ryan";"ryan";"john"]
hello johhn where is john
```

Part 1: Pass single sym through function

```q
f: {ssr[(string x);y;z] }
f[`welcome;"me";"ME"]
"welcoME"

/ so x gets converted from `sym to string
/ then SSR is run on string "welcome"
/ and replaces "me" with "ME"
```

re-written as lambda function

```q
/ alternative syntax (lambda function)

{ssr[string x;y;z]} [`welcome; "me";"ME"]
"welcoME"

/ did not define function (lambda)
/ uses implicit arguments x, y, z
/ passes arguments immediately after function
/ string x = ONLY applies to argument x
```

Alternative method to call arguments 

```q
/ alternative syntax (lambda + alt method to call argument)

{ssr[string x;y;z]} [ ; "me";"ME"] `welcome
"welcoME"

/ so sym `welcome is implicit argument x
/ since arguments y and z are already defined as "me" and "ME"
/ this is useful when iterating through a LIST of syms
```

PART 2: re-write function to pass a LIST of syms

```q
/ instead of converting one sym
/ need to iterate function through list of syms

f:{ssr [string x;y;z]} 
f[ ;"me";"ME"] each `welcome`home`mermaid
"welcoME"
"hoME"
"MErmaid"

/ function remains the same
/ but when you CALL the function, need adverb EACH
/ this iterates through each sym
/ the list of syms `welcome`home`mermaid gets passed through x
/ REQUIRES x to be left blank inside [ ] 
/ while locking in arguments y and z as constants
```

re-written as lambda function

```q
/ lambda notation

{ssr [string x;y;z]} [ ;"me";"ME"] each `welcome`home`mermaid
"welcoME"
"hoME"
"MErmaid"

/ function remains the same
/ but when you CALL the function, need adverb EACH
/ this iterates through each sym
/ the list of syms `welcome`home`mermaid gets passed through x
/ REQUIRES x to be left blank inside [ ] 
/ while locking in arguments y and z as constants```
```

<a name="implicit_argu"></a>
### 🔵 10.3 Implicit Arguments

```q
/ implicit arguments = variable names that when used inside body of function
/ are assumed to be arguments
/ q permits up to 3 implicit arguments: x, y, z
```

```q
{x*x}5
25

/ this is an ANONYMOUS function
/ which uses implicit variable x
/ omit defining argument [x], q implicitly understands x is an argument
```

```q
{x+y+z}[1;2;3]
6

/ q has x, y, z as implicit arguments
/ [1;2;3] you are calling x y z as arguments
```

```q
{x+z}[1;2]

/ error because you can't skip the y
/ if only 2 implicit arguments, need to use x and y
```

<a name="local_global_variables"></a>
### 🔵 10.4 Local vs Global Variables

Locally Defined Variables (inside Function)

```q
{a:1; b:2; a+b*x} [12]
25

/ 3 statements inside function body
/ the LAST statement will be returned by function
/ anonymous function (no variable assignment)
/ x = implicit argument (since not defined)
/ calls in 12 = x
/ RIGHT to LEFT: 12 * 2 + 1 = 25
/ a and b are LOCALLY DEFINED VARIABLES within the function
/ will NOT work if you try to recall variable a or b outside the function
```

Global Variables

```q
d:10
f:{d+x}
f [1]
11

/ assign global variable D to 10 (outside the function)
/ global variables can be pulled into function
/ f[1] calls in 1 for x (implicit argument)
/ = 10 + 1 = 11
```

Global vs Local Variables in Functions

```q
d: 10
g: {d:20; d+x}
g [1]
21

/ d:10 = GLOBAL variable
/ but d appears again, inside function
/ d:20 is a LOCALLY defined variable
/ LOCAL (20) TAKES PRIORITY over global (10)
/ x is implicit argument = 1
/ 20 + 1 = 21
```

Global Variable Assignment

```q

h:{r::x;r}

/ r :: x = to the global variable r, assign value x
/ essentially, r is a global variable and assign it x

h[100]
100

/ by calling 100 = implicit argument x
/ r = 100
/ function returns LAST statement = r
```

<a name="projected_func"></a>
### 🔵 10.5 Projected Functions

```q
/ create one function
/ create another function, which is a PROJECTION of first function
/ allows for one variable to be set as a CONSTANT
/ allows us to apply functions to a list of variables
```

Example 1

```q
/ create first function called raise

raise: {x xexp y}
raise [10; 2 3 4]
100 1000 1000f
 
/ calls x = 10 and y = 2 3 4
```

```q
/ create second function called g, which projects function raise
/ keeps x constant @ 10

g: raise [10; ]
g 1 2 3
10 100 1000

/ you've already created function raise previously
/ so g is a PROJECTION of the original function RAISE
/ so x = constant 10
/ y becomes arguments you call in (1 2 3)
```

```q
/ create another function square, which projects function raise

square: raise[ ;2]
square 1 2 3
1 4 9

/ in this case, leaves first argument blank (x)
/ and keeps second argument constant at 2
/ calls in 1 2 3 for x xexp 2
```

Example 2

```q
f:{x*y}
f[4;5]
20
```

```q
/ let's assume y will stay constant @ 5 and only x will change

f:{x*y}

g:f[ ;5]
g[3]
15

/ g is a projected function of f
/ f[x;y] = y is set constant @ 5
/ now when you call g[3], x=3 while y stays the same
/ g becomes a nomaic parameter
```

```q
f:{x*y}

h:f[10; ]
h[2]
20

/ so this time, we set x as constant 10
/ when we call 2 for function h
/ that automatically gets passed as the y argument
```

```q
g
{x*y}[;5]

/ if you call g, you'll see it contains original expression
/ and the set parameters are shown in [ ]
```

<a name="iftrue_state"></a>
### 🔵 10.6 If Statements

```q
/ if[condition_true; do_this]
/ if condition TRUE, execute all statements that follow
/ if condition FALSE, do nothing
/ if statements do NOT return a value
```

Example 1

```q
if[10>3; a:11; show a*10]
110

/ since the first condition is TRUE, execute all statements that follow
/ if FALSE, do nothing
```

Example 2

```q
if[3<5; show 1+1]
/nothing happens

/ since first condition = FALSE, nothing gets executed
```

Example 3

```q
if[10>3; a:11; show a*10; show "hello"]
110
"hello"

/ as long as the first condition is true, execute all following statements
```

IF Statements DON'T return value

```q
r: if [2>1; 10]
r
/ r returns nothing

/ even though IF statement is true
/ r doesn't get assigned a value
```

If Statements - Booleans

```q
/ Any number = boolean TRUE 
/ 0 = defaults to boolean FALSE (0b)
/ Combine booleans + IF statements
```

True Example

```q
if[10; show "true"]
"true"

/ Any number = boolean TRUE 
/ 0 = defaults to boolean FALSE (0b)
/ since 10 is an int, and int will default to 1b (true)
```

False Example

```q
if[0; show"false"]
/ nothing happens

/ 0b=false, so nothing happens
```

False Example 2

```q
if[count(); show "true"]

/ nothing shows, since count empty list = 0, hence false
```

<a name="iftrue_else_state"></a>
### 🔵 10.7 If/Else Statements

```q
/ IF/ELSE statements use $[ ] syntax
/ $[cond_true; do_this; else_do_this]
/ IF first condition TRUE, execute first statement
/ ELSE, execute last statement
/ IF/ELSE statements DOES return a value
```

Example 1

```q
$[1b; show "true"; show "false"]
true

/ always starts with $[ ] 
/ IF first condition TRUE, then execute second condition. ELSE, execute third condition
/ First condition = 1B = false boolean
```

Example 2

```q
$[100>1; [show "message"; `a];`b]
"message"
`a

/ first condition = TRUE
/ executes second statement (everything in the [ ] )
```

Example 3 (Returns Value)

```q
/ IF ELSE statements return value!

r: $[2>1; 10; 20]
r
10

/ since the first condition is TRUE
/ the first expression gets executed
/ and r gets assigned 10
/ when you call r, you get 10
```

```q
r: $[10<1; 10; 20]
r
20

/ since the condition is FALSE
/ r gets assigned 20
/ when you call r, you get 20
```

Example 4

```q
/ if you want to pass an argument to IF/ELSE statement
/ need to encase with { }

{ $ [x<0; `negative;`positive]} -2
`negative

/ first condition TRUE
/ so returns second statement
```

Example 5 - Vector Conditional

```q
/ vector conditional examines a list of booleans

? [vector_condition; true_expression; false_expression]

/ the condition will be a list of booleans
/ be careful about inconsistent lengths!
```

```q
l: 1 2 3 4 5
l > 2
00111b

/ you have a list of atoms
/ l > 2 returns a list of booleans

? [l>2; `TRUE; `FALSE]
`FALSE`FALSE`TRUE`TRUE`TRUE

/ first condition = pass the list of booleans
/ where TRUE, return first statement
/ where FALSE, return second statement

/ IF/ELSE only operates in atoms
/ but vector conditional takes a LIST of booleans
```

<a name="add_cond_branch"></a>
### 🔵 10.8 Adding Conditional Branch Pair

```q
/ by adding an expression (x=0), and another statement (`positive)
/ you create an if/else branch
/ if first condition = TRUE, execute first statement
/ if first condition = FALSE, move onto second Condition
```

Example 1

```q
{$[x<0; `negative; x=0; `zero; `positive]} -2
`negative

/ first condition is TRUE, so executes first Statement
/ pass implicit argument -2
/ so need to wrap in { }
```

```q
{$[x<0; `negative; x=0; `zero; `positive]} 0
`zero

/ first condition FALSE (0 < 0)
/ move onto second condition (0 =0) = TRUE
/ returns second statement = `zero
```

```q
{$[x<0; `negative; x=0; `zero; `positive]} 3
`positive

/ first condition = FALSE
/ moves onto second condition = FALSE
/ moves onto third condition = TRUE
/ returns 3rd statement
```

```q
/ if condition is true, evaluate all the following expressions
/ finishes with condition to be executed if all conditions are false
/ if true condition encountered, no further condition evaluated
```

Example 2

```q
a:5
$[a<2; 1; a<4; 2; a<6; 3; a<8; 4; 20]
3

/ first condition = FALSE
/ moves onto second condition = FALSE
/ moves onto third condition = TRUE (5<6)
/ returns 3rd statement = 3
```

IF/ELSE Statement with Multiple Expressions

```q
/ if you want to execute more than 1 expression
/ need to make it a statement block
/ and enclose your expressions in square brackets [ ]

$ [a>10; [b:10; c:11]; [b:98; c:99]]

/ if condition TRUE
/ then b gets 10 AND c gets 11
/ if condition FALSE
/ then b gets 98 AND c get 99


a:20
$ [a>10; [b:10; c:11]; [b:98; c:99]]
b
10
c
11

/ since condition true, when you call b, you get 10
/ and when you call c, you get 11
```


<a name="do_loop"></a>
### 🔵 10.9 Do Loops

```q
/ do loops repeat the function x number of times
/ useful to time how long it takes to run your function
```

```q
do[3;show "hi"]
hi
hi
hi

/ first statement = how many times to loop
/ second statement = what to execute
/ loop this 3x
```

Time your do Loop

```q
f:{avg x xexp 1000?2}
\t do[1000;f]
0

/ time the loop 1000x on function f
/ x to the power of 1000 random numbers 
1000? = 1000 random numbers from 0-1
```

<a name="while_loop"></a>
### 🔵 10.10 While Loops

```q
/ while condition = True, keep executing until condition = False
/ while will execute a statement x number of times until statement is no longer true
/ usually involves some sort of iterator (x:x+1)
```

Example 1

```q
a:1
while[a<3; show a; a:a+1]
1
2

/ 1 is less than 3, so show 1
/ a becomes 1+1 =2
/ 2 less than 3, so show 2
/ a becomes 2+1=3
/ 3 not less than 3, so stop executing
```

Example 2

```q
/ while loop keeps running until no longer true

a:1
b:2
while[a<10; a:a+1; b:b+1; show enlist b,a]

b  | a
--------
3  | 2
4  | 3
5  | 4
6  | 5

/ a = 1; a becomes 1+1(2)
/ b = 2; b becomes 2+1(3)
/ show enlist shows b and a in a clean list
/ stop running this loop when first condition becomes false
```

Example 3

```q
/ warning! be careful with this
/ functions run RIGHT to LEFT

a:1
b:2
while[a<100 and b<5; a:a+1; b:b+1; show enlist b,a]
nothing happens!

/ RIGHT TO LEFT
/ 1<5 = TRUE
/ 100 and TRUE = TRUE
/ a < TRUE = FALSE (since a = 1)
/ since the first condition is false, the function doesn't run
```

```q
/ to make it run correctly, add in parathesis!

a:1
b:2
while[(a<100) and b<5; a:a+1; b:b+1; show enlist b,a]
3 2
4 3
5 4

/ now it works 
```

<a name="multi_cond_while_loop"></a>
### 🔵 10.11 Multi Condition While Loops

Example 1

```q
/ generate list of 100 random numbers from 0-99
/ sum all values in list > 50 using while loop

d: 100?100
i: 0
r1: 0

while [i < count d; if [d[i]>50; r1+:d[i] ]; i+:1]

/ d = list of 100 random numbers from 0-99
/ i = iterative counter (goes from 0-99). Counts through every element of list d
/ r1 = result of while loop

/ while i is less than total number of items in list d (99)
/ if value of list d at index position i is less than 50
/ add this value to results list (r1)
/ then go onto next iteration (i+1)

/ remember, WHILE LOOPS -> if first argument is TRUE, execute all arguments that follow
/ WHILE LOOP = used as iterative counter through all elements of list d (0-99)
/ IF STATEMENT = tests IF condition true, add to list
```

Vector Operation Solution

```
HOWEVER, much faster using vector operations:

r2: sum d where d > 50

/ so use vector operations whenever possible
/ also a lot more flexible:

max sum d where d>50
min sum d where d>50
avg sum d where d>50
```

<a name="prime_func"></a>
### 🔵 10.12 PRIME NUMBERS FUNCTION CASE STUDY

```q
/ create function that finds primes up to argument x
/ since you are returning list of numbers
/ will require an 1) empty list
/ and 2) an iterator to check every number up to x

/ iterator starts from 1
/ if iterator is prime, append to list r (need to use ,: NOT sum)
/ then go onto next number
/ keep checking until WHILE condition is no longer true (a<n)
/ then return list r

findprime: {[n] r:(); a:1; while [a<n; if[isprime[a];r,:a]; a:a+1];r}
findprime 10 
2 3 5 7

/ n = single argument
/ r() = empty list thats gonna contain our result
/ a starts from 1 (iterator)
/ while a(1) < n = TRUE
/ if a = prime number,
/ append a to list r (r,:a = append a to list r)
/ go through every value of a (a+:1)
/ finally, return our list r

/ in other words..
/ starting from 1, look up to our argument
/ checking if each number is a prime number
/ and if it is, append it to our list (r)
/ finally, return the list of primes
/ still need to write the isPrime function

/ a:1, n:5
/ while a(1) < n(5) = TRUE
/ if a(1) = prime = FALSE
/ skip rest of while loop
/ a:a+1 = 1+1 = 2

/ while a(2) < n(5) = TRUE
/ if a(2) = prime = TRUE
/ append a(2) to r (2)
/ a:a+1 = 2+1 = 3

/ while a(3) < n(5) = TRUE
/ if a(3) = prime = TRUE
/ append a(3) to r (2,3)
/ a:a+1 = 3+1 = 4

/ while a(4) < n(5) = TRUE
/ if a(4) = prime = FALSE
/ skip rest of while loop
/ a:a+1 = 4+1 = 5

/ while a(5) < n(5) = FALSE
/ skips entire while loop
/ returns r (2, 3)
```

```q
/ isPrime function

/ create function with 1 argument input
/ and checks whether argument is Prime (True) or not (False)

/ prime = any num can only % by itself and 1
/ prime numbers begin on 2
/ will need 3 components:
/ 1. number < 2 (not prime)
/ 2. number = 2 (prime)
/ 3. number > 2 (could be prime)

/ the outcomes for component 1 and 2 are quite binary. 
/ component 3 -> requires you to check if number has any factors
/ which means dividing by every number up to x number

/ general reminder:
/ IF brackets [contain condition + statement to execute if true]
/ WHILE brackets [contain condition + statement to execute if true]

isprime:{if[x<2; :0b]; a:2; while[a<x; if[(x mod a)=0; :0b]; a+:1]; 1b}

Component 1 (number < 2)
/ if argument less than 2, return FALSE 0b (not prime)
/ since primes cannot be less than 2
/ if[x<2; :0b]
/ single colon : means return. nothing after gets executed
/ if x = 1
/ x(1) < (2) (TRUE) so returns 0b (not prime)
/ if FALSE, then moves onto NEXT statement

Component 2 (number = 2)
/ Create variable a, which begins on 2
/ a is your iterator (will check every number up to x number)
/ while[a<x; if_false_skip_this_entire_while_loop]; 1b
/ while condition a < x is FALSE
/ skip ENTIRE while loop
/ and go straight to the end, return TRUE 1B (prime)
/ if x = 2
/ x(2) < a(2) = FALSE. Skip while loop
/ goes to end, returns 1b (True)

Component 3 (number > 3)
/ while condition a < x is TRUE (iterator < x number)
/ check if a is a factor of x number
/ this check is done by x mod a = 0 (even number/factor exists = NOT PRIME)
/ if TRUE, return false :0b
/ otherwise, iterate through until WHILE condition (a<i) is no longer true

/ if x = 5
/ a(2) < x(5) = TRUE
/ x(5) mod a(2) = 0 = FALSE = skips :0b
/ a:a+1 so 2 + 1 = 3
/ a(3) < x(5) = TRUE
/ x(5) mod a(3) = 0 = FALSE = skips :0b
/ a:a+1 so 3+1 = 4
/ a(4) < x(5) = TRUE
/ x(5) mod a(4) = 0 = FALSE = skips :0b
/ a(5) < x(5) = FALSE, SKIPS entire while loop
/ goes to end, returns 1b (True) 
```

Vector Based Solution

```q
/ the above function uses control statements and loops
/ but this is very slow
/ instead, can re-write without do or while loops 
/ using a vector based solution
```

isprime Vector Solution

```q
/ re-write isprime function using vector based solution

/ original function

isprime:{if[x<2; :0b]; a:2; while[a<x; if[(x mod a)=0; :0b]; a+:1]; 1b}

/ we can rewrite the while loop portion

/ instead of looping through every iteration of argument x 
/ we can simply use til to generate a list

{til x} 10
0 1 2 3 4 5 6 7 8 9

/ removes first 2 elements (since not prime)

{2_til x} 10
2 3 4 5 6 7 8 9
/ drops 0, 1 since not prime

/ check each number if it is a factor of argument x(10)

{x mod 2_til x} 10
0 1 2 0 4 3 2 1

/ 10 mod 2 = 0
/ 10 mod 3 = 1
/ 10 mod 4 = 2
/ 0 means no remainder = factor of x = NOT PRIME

/ show us factors of argument x

{0=x mod 2_til x} 10
10010000b
/ shows us factors of argument 10
/ 1 = true
/ 0 = false

/ are there ANY factors of 10? (mod = 0)

{any 0=x mod 2_til x} 10
1b
/ TRUE, because list contains SOME factors of 10

/ does the list NOT contain any factors of 10?

{not any 0=x mod 2_til x} 10
0b
/ FALSE, because list DOES contain factors of 10
/ hence, NOT prime

/ still need component for numbers less than 2
/ so re-use the x<2 IF/Else clause

isprimeB: {if[x<2; :0b]; not any 0=x mod 2_til x}
isprimeB 10
0b

/ x(10)<2 = FALSE, skips if statement
/ goes onto second statement
/ FALSE, 10 is NOT prime
```

findprimes Vector Solution

```q
/ re-write findprimes function using vector based solution

/ original findprime function:

findprime: {[n] r:(); a:1; while [a<n; if[isprime[a];r,:a]; a:a+1];r}

/ use til instead of while loop

{til x} 10
0 1 2 3 4 5 6 7 8 9

/ perform isprime function on EACH of the numbers
{isprimeB each til x} 10
0011010100b

/ returns us a list of booleans
/ does this list contain any prime?
/ 0 = no
/ 1 = yes

/ convert booleans BACK into numbers
/ want 1 (true) = prime turned back into numbers
/ use WHERE function

findprimesB: {where isprimeB each til x}
findprimesB 10
2 3 5 7
```

<a name="func_lambda"></a>
### 🔵 10.13 Function within a Function (Projected Functions)

```q
f:{x*x}
g:{10 + f[x] }
g[2]
14

/ 2 becomes x, 10 + 4 = 14
```

Can define a function within a function inline

```q
z:{f:{x*x}; f[x] + 10}
z[2]
14

/ on the same line, can call function f into another function body
/ function f = 2 *2 = 4
/ f[x] = the output of function f{x*x} = 4
```

Can be anonymous / lambda

```q
/ this is weird syntax, dont know if useful

{{x*x}[x] + 10}
{x+y} [3;4]
7

/ you can write same operation without defining the function f 
/ write expression + parameters in [ ] 

/ flexible in syntax

{x+y} [3;] 4
7

{x+y} [;4] 3
7
```

<hr>

<a name="func_problem_set"></a>
## 🔴 11. Functions Problem Set
[Top](#top)

**🔵 11.1 Volume of cone function**

```q
/ create func called volc that accepts 2 arguments (r and h)
/ returns volume of cone
/ vol of cone = 1/3 * pi * r^2 * h
/ pi = -4 * atan -1

volc: {[r;h] pi:-4*atan -1; pi*r*r*h%3}
volc[2;3]
12.57

/ define arguments [r;h] first
/ define variable pi
/ must have space after atan and before -1
/ no space for volc[2;3]
```

**🔵 11.2 Area and Volume of cone function**

```q
/ create function, called sph, that accepts argument radius
/ and returns the area and volume of a cone as a dict

/ volume = 4/3 * pi * r^3
/ area = 4 * pi * r^2
/ pi = -4 * atan -1

sph:{[r] pi:-4 * atan -1; v:(4%3)*pi*r xexp 3; a:4* pi * r xexp 2; `area`volume!(a;v)}
sph[1]

key    | value
----------------
area   | 12.56
volume | 4.188

/ define argument [r]
/ you can define variables with functions inside your function!
/ define variable pi with formula
/ define variable a with formula
/ define variable v with formula
/ then you can create dictionary using the variables you defined
/ show dictionary with keys `area `volume against values a and v
/ create keys as syms (`area`volume) mapped to values defined by your variables (a;v)
```

**🔵 11.3 Implicit Arguments and Global Variables**

```q
/ create function, setc, that takes 1 implicit argument
/ and sets the value of global variable c to that argument

c:10

setc: {x::c}
setc[15]
10

/ set global variable c to 10
/ x is your implicit variable
/ you assign x the value of global variable c
/ so WHATEVER value you call using setc, it assigns
/ that value to the global value of q
/ so even though you call func with 15
/ the output is 10 (global variable)
```

**🔵 11.4 Projected Functions**

```q
/ raise:{x xexp y}
/ create projection of raise called root
/ which calculates the square root of argument 
/ ie, root[9] = 3

raise: {x xexp y}
root: raise[ ; 0.5]
root[9]
3

/ first define function raise
/ then we take a PROJECTION of that function, rename as root
/ and we set the y variable CONSTANT as 0.5
/ this allows the projected function ROOT to only allow 1 input as x
/ so the projected function will always be x xexp 0.5
```

**🔵 11.5 Casting Mixed List to Strings**

```q
/ convert all elements of list l to a string

l: (100;`price;1b)
string l
"100"
"price"
"1b"

/ l is a list of long, sym, and boolean
/ simply using the "string" function, converts all elements to strings
/ mixed lists have to be contained in parathesis ( )
```

**🔵 11.6 SSR Function**

```q
/ given string st, replace "cow" with "kangaroo"
/ st: "the cow jumped over the moon"

st: "the cow jumped over the moon"
ssr [st; "cow";"kangaroo"]
"the kangaroo jumped over the moon"

/ ssr = string search replace.
/ first condition = string
/ second condition = what to target
/ third condition = what to replace with
```

**🔵 11.7 Multi Argument Functions**

```q
/ create function, sayHi, that takes 2 arguments: name and age
/ and returns "hello age year old name"
```

```q
sayHi:{[name;age] "hello " , string[age] , " year old " , name}
sayHi["joe";90]
hello 90 year old joe

/ name and age are your arguments
/ name is a string
/ age is an int
/ the output is a list of chars (or one long string)
/ so you have to convert your [age] argument to a string
/ and join them together using string concatenation
/ string concatenation simply done with a comma ,
/ when you define argument "joe" have to use parathesis otherwise wont work
```

**🔵 11.8 Arithmetic on Lists**

```q
/ I have a box of 7 eggs, and the weights are
/ eggs: 10 20 30 40 50 60 70
/ find the median and average weight of these eggs

med eggs
40f

avg eggs
40f

/ note, division will always return a float
/ apparently same with med and avg functions
```

**🔵 11.9 Weighted Averaged WAVG Function**

```q
/ I sold 2 boxes of eggs
/ one box had 10 eggs and i sold each egg for 50 each
/ the other box had 20 eggs and i sold each for 100 each
/ find the average price paid per egg

10 20 wavg 50 100
83.3

/ to find the average price per egg
/ you want to find the weighted average of the 2 lists
/ wavg = weighted average function
/ qty1 qty2 wavg value1 value2
```

**🔵 11.10 Moving Average Window Functions**

```
/ generate list k with 10 random ints
/ find moving average with window size of 3

k: 10?10
8 7 9 9 7 7 1 9 1 0

mavg[3;k]
8 7.5 8 8.3 8.3 7.6 5 5.6 3.6 3.3
```

```q
/ Find the 3 largest numbers in list k

desc k
9 9 9 8 7 7 7 1 1 0

3#desc k
9 9 9 

/ take 3 of the largest from k, sort by desc
```

```q
/ Find the difference between the successive elements of k

k
8 7 9 9 7 7 1 9 1 0

deltas k
8 -1 2 0 -2 0 -6 8 -8 -1

/ the deltas functions returns the difference (delta) of each element
/ 8-0 = 8
/ 7-8 = -1
/ 9-7 = 2
/ etc
```

**🔵 11.11 Factorial Function using While Loops**

```q
/ Create function factw, which uses a loop to write a factorial function
/ factorial = multiply every iteration up to number x

factw:{i:1; r:1; while[i<x; r*:i; i+:1];:r*x}
factw 4
24

/ while loop, so need some sort of iterative counter (i)
/ want to mutiply every iteration of x, up to x 
/ so also need an empty list to store these iterations (r) 
/ first define i:1 (no point starting at 0)
/ and define r:1 (this is the list of numbers you want to multiply)
/ while i is less than implicit argument x (your input number)
/ multiply i with r, and r becomes that new number (r*:i mean r: r*i)
/ then move onto next iteration (i+:1 means i:i+1)
/ keep running this while loop until x-1, then stop executing
/ finally, return r * x (your original input)
```

```q
/ alternative syntax (shorter)

factw:{r:i:1; while[i<=x; r*:i; i+:1];r}
factw 3

/ x is implicit variable= 3
/ set r = i = 1
/ while i(1) <= x(3) TRUE, execute following statements
/ r = r(1) * i(1) = 1
/ i = i(1) + 1 = 2

i(2) <= x(3) TRUE, so continue executing
/ r = r(1) x i(2) = 2
/ i = i(2) + 1 = 3

i(3) <= x(3) TRUE
/ r = r(2) x i(3) = 6
/ i = i(3) + 1 = 4

i(4) <= x(3) FALSE, so returns r = 6
```

**🔵 11.12 Factorial Function using Vector Conditional**

```q
/ re-write the factorial function as factp WITHOUT using loops
/ must use vector conditional approach

/ to replace WHILE loop using vector conditional
/ usually replaces with til function

til 4
0 1 2 3

1_til 4
1 2 3

prd 1_til 4
1*2*3

4 * prd 1_til 4
1*2*3*4

/ so putting it all together, replacing variable with x

factp:{x*prd 1_til x}
factp 4
24

/ KEY TAKEAWAY
/ prds = multiplies all elements together
/ must remember to drop first element 0 (otherwise will all be 0)
/ must multiple original x back in
/ since til only generates list up to, but not including x
```

**🔵 11.13 Timing Calculations**

```q
/ Demonstrate which calculation is faster,
/ factorial using loops or via KDB (vector conditional)
/ use \ts to time
/ do function useful (do x number times)

\ts do[1000;factw 12]
4 1008

/ 4 miliseconds 1008 bytes of memory

\ts do[1000;factp 12]
0 1008

/ 0 miliseconds 1008 bytes of memory
```

**🔵 11.14 Protetcted Evaluations on Functions**

```q
/ Create function called safefact
/ that wraps factp with protected evaluation
/ to return null On instead of error 
/ when calling on a negative number

safefact:{@[factp; x; 0N]}
safefact -10
0N

/ you "wrap" your function using the @ operator ("apply")
/ @ = apply 
/ first condition = factp function
/ if TRUE, return x
/ if FALSE, return ON
```

**🔵 11.15 If/Else Statements (w reverse operator)

```q
/ Write a function called isPalindrome 
/ that accepts single argument as a list of ints 
/ returns `yes if list of ints is a palindrome
/ otherwise return `no

/ palindrome = same forwards + backwards
/ example = 1 2 3 3 2 1

isPalindrome:{$[x~reverse x;`yes;`no]}
isPalindrome 1 2 2 1
yes

/ since we are taking in 1 argument
/ with a binary outcome (true vs false)
/ need to use if/else statement $ [ ]
/ implicit argument x is a list of integers
/ need to utilize REVERSE function 
/ to compare if x = reverse x
```

**🔵 11.16 Find the sum of all multiples of 3 or 5 below 1000**

```q
/ check every number up to 1000
/ if its a factor of 3 or 5
/ x mod 3 = 0
/ x mod 5 = 0

/1. generate list of ints from 0-999

til 1000
0 1 2 3...999

/2. check if number is a factor of 3 or 5

{(0=x mod 3) or (0=x mod 5)} [til 1000]
1001011

/ you get a list of booleans
/ ie, true, the number is a factor of 3 or 5
/ IMPORTANT! the 0 = has to come in FRONT of (0=x mod 5)
/ (x mod 5 = 0) does NOT work

/3. CONVERT list of booleans to their numbers, use WHERE

where {(0=x mod 3) or (0=x mod 5)} [til 1000]
0 3 5 6 9 10 12 15 18 20 21 

/4. lastly, use sum to add up all numbers in the list

sum where {(0 = x mod 3) or (0 = x mod 5)} [til 1000]
233168

/ by using anonymous function, you can perform QSQL (sum where)
/ as well as call argument x as a list (til 1000) in place
/ x mod 3 and x mod 5 = search for any multiples of 3 or 5
/ since dividing by a factor will be 0
/ oddly enough, the 0 = in (0 = x mod 3) HAS TO come first
/ (x mod 3 = 0) doesn't work for some reason
```


<a name="tables_header"></a>
## 🔴 12. Tables
[Top](#top)

```q
/ a table is a flipped dictionary.
/ vectors of data are organized by columns. 
/ tables are encased by parathesis ( ) and contain brackets [ ] which assigns the key.
```

<a name="dict_to_table"></a>
### 🔵 12.1 Flipping Dictionary to Table

```q
d: `company`employees`! (`ford`bmw; 300 100)

key      |  value
---------------------
company	 | `ford`bmw
employees| 300 100

flip d
company | employees
-------------------
ford    | 300
bmw	| 100

/ when you flip a dictionary, you get a table

```

<a name="simple_table"></a>
### 🔵 12.2 Simple Table

```q
( [] company: `ford`bmw; employees: 300 100)

company | employees
-------------------
ford    | 300
bmw	| 100

/ have to define a table within parathesis ( )
/ tables must have [] which are for key columns
/ semi colon ; separates next column
```

<a name="single_row_table"></a>
### 🔵 12.3 Single Row Table (enlist)

```q
( [] company: enlist `ford; employees: enlist 300)

company | employees
--------------------
ford    | 300

/ have to use enlist for atoms and single row tables
```

<a name="mixed_table"></a>
### 🔵 12.4 Mixed Table

```q
/ table of SYM, FLOAT, STRING

( [] syms:`a`b`c; floats: 1.1 2.2 3.3; strings: ("bob"; "jim"; "john"))

syms|floats|strings
-------------------
a   | 1.1 | bob
b   | 2.2 | jim
c   | 3.3 | john

/ syms have to start with backtick
/ strings have to enclose within (" ")
```

```q
/ table of SYM, CHARS, TIME

([] syms:`a`b`c; chars:"aaa"; times:08:00 08:30 09:00)

syms | chars |	times
----------------------
a    |	 a   |	08:00
b    |	 a   |	08:30
c    |	 a   |	09:00

/ notice chars "aaa" gets split into rows
```

```q
/ columns with repeated values

([] syms:`a`b`c; num: 33)

syms | num
------------
a    | 33
b    | 33
c    | 33

/ since syms column has 3 rows, a single value in second column will duplicate
```

<a name="meta_datatypes_table"></a>
### 🔵 12.5 Meta / Data Type Table

```q
/ Meta returns a table of information on underlying columns

t: ( [] company:(); employees:() )
meta t

/ create empty table with no types
/ c = column names
/ t = datatype (s = symbol, j = long)
/ f = foreign key
/ a = attributes

c        |t|f|a
---------------
company  | | | 
employees| | | 
```

```q
/ cast columns to specific type

( [] company: `symbol$(); employees: `int$())

/ changed company type to SYM and employees to INT
/ if J is capital = nested lists

c        |t|f|a
---------------
company  |s| | 
employees|j| | 
```

<a name="countrowsimple_table"></a>
### 🔵 12.6 Count Row Table

```q
company | employees
--------------------
ford    | 300
bmw	| 100

count t
2

/ counts number of rows in table
```
<a name="countrowsimple_table"></a>
### 🔵 12.6 View Columns in Table (cols)

```q
cols t
`company`employee

/ returns list of all columns
```

<a name="rename_column_table"></a>
### 🔵 12.7 Rename Column Table (xcol)

```q
company | employee
------------------
ford    |   300
bmw     |   100

`a`b xcol t

 a  | b
---------
ford| 300
bmw | 100

/ renames first 2 columns from company/employee to a/b
/ xcol will only change col names from left to right
/ NOT in place, not saved to underlying table
```
<a name="rename_column_table"></a>
### 🔵 12.7 Reorder Column Table (xcols)

```q
company | employee
------------------
ford    |   300
bmw     |   100

`employees`company xcols t

employee | company
------------------
300      |  ford 
100      |  bmw  

/ reorders columns
/ doesn't have to be complete list of columns
/ just moves it to left of table
/ NOT in place, not saved to underlying table
```

<a name="add_column_table"></a>
### 🔵 12.8 Add Column

```q
select company, employees, newval: 101 from t

company | employees | newval
----------------------------
ford    |   300     | 101
bmw	|   100     | 101

/ select will retrieve columns as values
/ if you select a column that doesnt exist, it will add it (newval)
```

<a name="sort_column_table"></a>
### 🔵 12.9 Sort Column Table (xasc/xdesc)

```q
/ sort by 1 column

`employees xasc t

company | employees | newval
----------------------------
bmw	|    100    | 101
ford    |    300    | 101

/ will sort ascending by employees
/ or xdesc for descending
```

```q
/ sort by 2 columns

`company`employees xasc t

company | employees | newval
----------------------------
bmw	|    100    | 101
ford    |    300    | 101

/ will sort by company first, then employees
```

```q
/ sort using >

fruit   grocer  price   quantity
--------------------------------
apple	mark	1	10
orange	mark	2	20
pear	allen	3	30
banana	tom	4	40

select [>grocer] from sales

fruit   grocer  price   quantity
--------------------------------
banana	tom	4	40
apple	mark	1	10
orange	mark	2	20
pear	allen	3	30

/ order our table in descending according to grocer
```

<a name="union_table"></a>
### 🔵 12.10 Union Table

```q
/ table union merges 2 tables together, but does NOT dupe values!

table t
company | employees
-------------------
ferrari | 100
ford    | 100 
rover   | 100

table u
company | employees
--------------------
ferrari | 100
bmw     | 5 
ford    | 5

t union u

company | employees
-------------------
ferrari | 100
ford    | 100 
rover   | 100
bmw     | 5 
ford    | 5

/ matches on keys (ferrari). if same value, copies value
/ does NOT dupe same values
/ if match on key (ford), but no match on value (100 v 5), returns BOTH values
/ if no match on key (rover), returns key + value as new row
```

<a name="except_table"></a>
### 🔵 12.11 Except Table

```q
/ x except y
/ only returns values found in x NOT found in y

t except u

company | employees
-------------------
ford    | 100
rover   | 100 

/ from table t, check table u for any key + value matches, and remove
/ ferrari 100 appears in both tables, hence removed
/ then returns remaining rows in table t
/ in table u, bmw + ford aren't matches, so ignored
```

<a name="inter_table"></a>
### 🔵 12.12 Inter Table

```q
/ x inter y
/ inter table = think of it as inner join
/ only returns key/values that matches in both tables

t inter u
company | employees
-------------------
ferrari | 100

/ only returns rows from both table t and u that match
```

<a name="distinct_table"></a>
### 🔵 12.13 Distinct Table

```q
([] a: 1 1 2; b: 1 1 3)

a|b
---
1|1
1|1
2|3

distinct ([] a: 1 1 2; b: 1 1 3)

a|b
----
1|1
2|3

/ will return distinct values per row
```

<a name="retrieve_table"></a>
### 🔵 12.14 Retrieve From Table

```q
3 methods to retrieve from table

1) QSQL
2) retrieve as a DICT
3) retrieve as a LIST

/ QSQL most common method
```

```q
table t:

company | employees
-------------------
ferrari | 100
ford    | 100 
rover   | 100
bmw     | 5 
ford    | 5
```

Retrieves ALL columns from table

```q
select from t

company | employees
-------------------
ferrari | 100
ford    | 100 
rover   | 100
bmw     | 5 
ford    | 5

/ QSQL method
```

Retrieve values from column as a COLUMN

```q
select company from t

company 
--------
ferrari 
ford   
rover 
bmw 	 
ford 

/ QSQL method
```

Retrieve values from column as a LIST

```q
t[`employees]
100 100 100 5 5
```

Retrieves row where company = ford 

```q
select from t where company = `ford

company | employees
-------------------
ford    | 100 

/ note - since you are using QSQL and filtering with WHERE
/ don't need backtick on column name = company
/ you need a backtick on `ford since ford is a sym
```

Retrieves columns values as a ROW

```q
t [`employees]
100 100 100 5 5 

/ retrieve using indexing on column name returns all values in column
```

Perform operations on entire column

```q
trade
date      | time        | sym |price   |size |cond
--------------------------------------------------
2021.11.09| 09:30:02.553| C   |107.2|63500|B   
2021.11.09| 09:30:02.701| MSFT|96.87|1700 |B   
2021.11.09| 09:30:02.743| RBS |97.11|80700|C   
2021.11.09| 09:30:02.758| A   |100.3|50300|B   

select sym, price, newprice:trade[`price]+100 from trade

sym | price| newprice
---------------------
C   | 107.2| 207.2
MSFT| 96.87| 196.87
RBS | 97.11| 197.11
A   | 100.3| 200.3  

/ adds 100 to each value in column price
```

Retrieve first 2 rows

```q
/ TAKE method

2#t

/ INDEXING method

t[0 1]

company | employees
--------------------
ferrari | 0
ford    | 0 
```

Retrieve last 3 rows

```q
-3#t

company | employees
-------------------
rover   | 0
bmw     |-105 
ford    |-105
```

Randomly selects 2 rows from table

```q
2 ? t

company | employees
-------------------
rover   | 0
ford    |-105
```

<a name="insert_table"></a>
### 🔵 12.15 Add / Insert Rows Table

```q
/ to add rows into a table, either use INSERT or UPSERT
/ 2 different syntax when using INSERT

`t insert (`ferrari`bmw;9 7)

/ or

insert [`t; (`ferrari`bmw; 9 7)]
```

INSERT Example 1 (syntax 1)

```q

/ create empty table with the following columns:
/ brand = sym datatype
/ model = sym datatype
/ purchasedate = date datatype

cars:([] brand:`$(); model:`$(); purchasedate:`date$())

/ insert `bmw, 318; 2021.01.01

`cars insert (`bmw;`318;2021.01.01)

brand model date
----------------------
bmw   318   2021-01-01

/ HAVE TO BACKTICK table (`cars) to insert, otherwise will fail
/ have to insert correct datatype. `318 is a sym
/ don't need enlist
```

INSERT Multiple Rows to Table (syntax 1)

```q
/ insert the following rows into cars table
/ `audi; `a5; 2021.01.02
/ `ford; `fiesta; 2021.01.03

`cars insert (`audi`ford;`a5`fiesta;2021.01.02 2021.01.03)

brand model  date
----------------------
bmw   318    2021-01-01
audi  a5     2021-01-02
ford  fiesta 2021-01-03
```

INSERT table into table (syntax 1)

```q
/ insert table cars into existing table of cars

`cars insert cars

brand |	model  | purchasedate
----------------------------
bmw   | 318    | 2021-01-01
audi  | a5     | 2021-01-02
ford  | fiesta | 2021-01-03
bmw   | 318    | 2021-01-01
audi  | a5     | 2021-01-02
ford  | fiesta | 2021-01-03

/ alternative syntax: `cars ,:cars
```

INSERT table with deleted column (syntax 1)

```q
/ delete column model from cars
/ then join onto existing table cars

`cars insert delete model from cars

brand model  date
----------------------
bmw   318    2021-01-01
audi  a5     2021-01-02
ford  fiesta 2021-01-03
bmw	     2021-01-01
audi	     2021-01-02
ford	     2021-01-03

/ deletes the column model first
/ then that table is inserted into existing table
```

INSERT Example 2 (syntax 2)

```q
/ create empty table t with columns company and employees

t: ( [] company: (); employees: () )
company|employees
```

INSERT SINGLE Row to table (syntax 2)

```q
/ insert single row `ferrari; 8 into table t

insert [`t; (`Ferrari; 8)]

company|employees
-----------------
Ferrari| 8

/ backtick t to update underlying table
/ first argument is table name(t), second argument are the values to be inserted
/ semi colon separate columns for the values
/ DON'T need enlist
```

INSERT MULTIPLE rows to Table (syntax 2)

```q
/ insert `ferrari`bmw; 9; 7 to table t

insert [`t; (Ferrari`bmw; 9 7)]

company|employees
-----------------
Ferrari| 8
Ferrari| 9
bmw    | 7

/ insert will append to the table each time (ferrari repeated)
/ column values separated by semi colon
```

INSERT table into another table (syntax 2)

```q
/ create table x with `subaru`hyundai; 55; 56

x: ( [] company: `Subaru`Hyundai; employees: 55 56)

company|employees
-----------------
Subaru | 55
Hyundai| 56
```

```q
/ insert table x into table t

`t insert x

company|employees
-----------------
Ferrari| 8
Ferrari| 9
bmw    | 7
Subaru | 8
Hyundai| 56

/ alternatively:

t:t,x
```

<a name="upsert_table"></a>
### 🔵 12.16 Upsert Rows Tables

```q
t:([fruit:`apple`banana] price:10 20; quantity: 100 50)

fruit  price quantity
--------------------
apple  10    100
banana 20    200

`t upsert(`apple;100;800)

fruit  price quantity
--------------------
apple  100   800
banana 20    200

/ upsert = update/insert
/ so in this case, it will find value `apple
/ and update its values in price and quantity to 100 800
```

You cannot upsert multiple rows

```
`t upsert (`apple`orange;11 23; 100 200)
/error
```

Instead, you have to upsert a table

```q
`t upsert ([]fruit:`apple`orange; price: 11 23; quantity:100 200)

fruit  price quantity
--------------------
apple	11   100
banana	20   200
orange	23   200

/ when upserting into tables, column order doesnt matter
/ can also miss columns

`t upsert ([]price: 20 30; fruit:`pear`guava)

fruit  price quantity
--------------------
apple	11   100
banana	20   200
orange	23   00
pear	20	
guava	30	
```

<a name="operations_table"></a>
### 🔵 12.17 Operations on Tables

```q
/ with KEYED tables, you can use arithmetic between tables

t1: ([sym: `a`b`c] num: 1 2 3)
t2: ([sym: `a`b`c] num: 1 1 1)

t1 + t2

sym | num
---------
a   | 2
b   | 3
c   | 4

/ BOTH tables have to be keyed
/ column names have to MATCH
```

if UNKEYED, can only do math on tables with numeric fields

```q
t1: ([] sym: `a`b`c; num: 1 1 1)
t2: ([] sym: `a`b`c; num: 1 1 1)

t1 + t2
/ error
```

```q
/ only works if table is ALL nums

t1: ([] num1: 1 1 1; num2: 1 1 1)
t2: ([] num1: 1 1 1; num2: 1 1 1)

t1 + t2

num1 | num2
-----------
2   | 2
2   | 2
2   | 2

/ Finds column names that match, and add values together
/ column names that dont match will be union joined as a new column
```

Math on Partial Key Matches

```q
/ partial key match 

t1:( [id:`a`b`c] price: 1 2 3; rating: 10 20 30)
t2:( [id:`b`c] price: 10 10 ; rating: 100 100)

/ t2 only has `b`c keyed

t1
id price rating
---------------
a    1     10
b    2     20
c    3     30

t2
id price rating
---------------
b   10    100
c   10    100
```

```q
t1 + t2
id price rating
---------------
a   1     10
b   12    120
c   13    130

/ ONLY keys `b`c are matching between the 2 tables
/ will only add values in these 2 rows
/ `a will simply return its original value
```

<a name="joins_table"></a>
### 🔵 12.18 Joins on Tables

```q
/ if 2 tables columns MATCH, can JOIN to ADD ROW
/ called vertical joins

t1
sym  side price size
---------------------
IBM  buy   10 	 100
AAPL sell  20    200

t2
sym  side price size
---------------------
GOOG buy   30 	 300
MSFT sell  40	 400

t1, t2

sym  side price size
---------------------
IBM  buy   10 	 100
AAPL sell  20	 200
GOOG buy   30 	 300
MSFT sell  40	 400
```

```q
/ if 2 tables have same number of rows
/ and NO matching columns
/ can join tables together by adding extra columns
/ similar to LEFT JOIN

t1
sym  ex
----------
IBM  nyse
AAPL nyse
GOOG nasdaq

t2
price size
----------
10    100
20    200
30    300

t1,'t2

sym  ex     price size
----------------------
IBM  nyse    10   100
AAPL nyse    20   200
GOOG nasdaq  30   300

/ t1 and t2 have diff column names
/ but same number of rows
```

Joining Tables using Take #

```q
/ assume large table called trade

/ create t1, which is the first 3 rows of trade

t1: 3#trade

sym	price	size
----------------------
C	107.2	63500
MSFT	96.8	1700
RBS	97.1	80700
```

```q
/ join t1 with last 3 rows of trade

t1, -3#trade

sym	price	size
----------------------
C	107.2	63500
MSFT	96.8	1700
RBS	97.1	80700
A	100.3	50300
B	55.8	92700
C	45.3	99930

/ combining first 5 rows of trade with last 5 rows of trade

```
### LEFT JOIN on tables

```q
/ using left join to join tables

t1:( []sym:`a`b`c; ex:`one`two`three; size:100 200 300)
t2:( []sym:`a`b`c; ex:`one`two`three; price:0.1 0.2 0.3)

t1
sym |ex   | size
-----------------
a   |one  | 100
b   |two  | 200
c   |three| 300

t2
sym |ex   | prrice
-----------------
a   |one  | 0.1
b   |two  | 0.2
c   |three| 0.3
```

Tables must be keyed!

```q
/ to use LEFT JOIN to join tables, the tables must first be keyed!

2!t1
2!t2

/ keys first 2 cols of both t1 and t2

(2!t1) lj (2!t2)

sym |ex   | size | price
-------------------------
a   |one  | 100  | 0.1
b   |two  | 200  | 0.2
c   |three| 300  | 0.3
```

<a name="find_table"></a>
### 🔵 12.19 Find on Tables

```q
t: ( [] a: 1 2 3; b: 4 5 6; c: 7 8 9)

a b c
------
1 4 7
2 5 8
3 6 9

t ? 3 6 9
2

/ find these values within the table
/ returns index position 2 (row 3)
```

```q
t ? (2 5 8; 3 6 9)
1 2 

/ can retrieve more than 1 set of values at once
/ returns list of indices (rows 2, 3)
```

```q
/ find first index position where chem appears in tab2

tab1:( [id:"abc"] pupil:`john`paul`rachel; subject:`maths`physics`chem; mark:96 55 82)

id| pupil |subject  | mark
--------------------------
a | john  | maths   | 96
b | paul  | physics | 55
c | rachel| chem    | 82

tab2[`subject]?`chem
2

/ you can lookup index position by finding VALUE from table[col_name]
/ syntax = tablename[col_name]?`sym
```

<hr>

<a name="tables_problem_set"></a>
# 🔴 13. Tables Problem Set
[Top](#top)

**🔵 Problem Set 1**

```q
stock: ( [] sym: `MS`C`AAPL; sector:`Financial`Financial`Tech; employees: 100 100 100)

sym |sector    |employees
-------------------------
MS  |Financial |100
C   |Financial |100
AAPL|Tech      |100
```

**🔵 13.1 Extract the employees values (without the header)**

```q
/ since they only want values and no header, use INDEX retrieve

stock[`employees]
100 100 100
```
other syntax:

```q
stock.employees
```
```q
stock`employees
```
```q
stock [ ; `employees]
```

**🔵 13.2 Key the first column in stock table above**

```q
1!stock

`sym` |sector    |employees
-------------------------
`MS`  |Financial |100
`C`   |Financial |100
`AAPL`|Tech      |100
```

**🔵 13.3 Display only the first and second rows of the stock table**

```q
/ use TAKE # method

2#stock

sym |sector    |employees
-------------------------
MS  |Financial |100
C   |Financial |100
```

alternative solution:

```q
/ use index retrieve method

stock [0 1]

/ returns index position 0 and 1 (first 2 rows)
```

**🔵 13.4 Select the last row of stock table as a dictionary**

```q
last stock

key       | value
-----------------
sym       | AAPL
sector    | Tech
employees | 100

/ LAST will retrieve the last row from table stock
/ and return it as a dictionary
```

**🔵 13.5 Insert GOOG in the tech sector with 100 employees**

```q
`stock insert(`GOOG; `Tech; 100)

sym |sector    |employees
-------------------------
MS  |Financial |100
C   |Financial |100
AAPL|Tech      |100
GOOG|Tech      |100

/ remember need to `stock otherwise error
/ saves + updates underlying table
```

alternative solution:

```q
insert [`stock; ([] sym: enlist `GOOG; sector: enlist `tech; employees: enlist 100)]

sym |sector    |employees
-------------------------
MS  |Financial |100
C   |Financial |100
AAPL|Tech      |100
GOOG|Tech      |100

/ syntax is insert + [table name; table with corresponding columns]
/ must use enlist when adding single row!!
```

**🔵 Problem Set 2**

```q
boss: ( [] name:`bob`bill`belinda; height: 188 186 174)
employees: ( [] name:`jim`jane`john; height: 180 160 170)

boss:
name    | height
----------------
bob     | 188
bill    | 186
belinda | 174

employees:
name| height
-----------
jim | 180
jane| 160
john| 170
```

**🔵 13.6 Find the average height of the bosses, the employees, and both the bosses and employees**

```q
avg boss[`height]
182.667

avg employees [`height]
170f

avg (boss,employees)[`height]
176.33

/ first JOIN boss and employees tables together
/ index retrieve values from the height column
/ then find average
```

**🔵 13.7 Find the 2 tallest employees**

```q
2 # `height xdesc employees

name | height
-------------
jim  | 180
john | 170

/ first sort employees table by height (xdesc)
/ syntax is column_name xdesc table_name
/ then you take the first 2 rows 
```

**🔵 Problem Set 3**

```q
stock: ( [sym:`MS`C`AAPL] sector:`Fin`Fin`Tech; employees: 100 100 100)
trade: ( [] dt: 2021.01.01+til 5; sym:`C`C`MS`C`AAPL; price: 10 20 30 40 50; size: 100 200 300 400 500)

stock:
sym  |sector| employees
-----------------------
MS   |Fin   | 100
C    |Fin   | 100
AAPL |Tech  | 100

trade:
dt        |sym  |price| size
----------------------------
2021-01-01|C	|10   | 100
2021-01-02|C	|20   | 200
2021-01-03|MS   |30   | 300
2021-01-04|C	|40   | 400
2021-01-05|AAPL	|50   | 500
```

**🔵 13.8 Insert the following rows into trade table**

```q
dt        |sym  |price| size
----------------------------
2021-11-01|JPM	|1    | 100
2021-11-02|UBS	|2    | 200

meta trade

c	t f a
---------------
dt	d		
sym	s		
price	j		
size	j		

/ since the values you insert HAS to match the datatype of table trade
/ meta helps you know what each column datatype is

`trade insert (2011.11.01 2021.11.02; `JPM`UBS; 1 2; 100 200)

dt        | sym  | price| size
-------------------------------
2021-01-01| C	 |  10  | 100
2021-01-02| C	 |  20  | 200
2021-01-03| MS   |  30  | 300
2021-01-04| C	 |  40  | 400
2021-01-05| AAPL |  50  | 500
2021-11-01| JPM	 |   1  | 100
2021-11-02| UBS	 |   2  | 200

/ can simply insert the values (without headers)
/ remember to backtick `trade table name
```

alternative solution:

```q
/ insert table method

`trade insert( [] dt:2021.11.01+1 ; sym:`JPM`UBS; price:1 2; size: 100 200) 

/ requires column header names
```

alternative solution:

```q
/ alternative syntax, but also requires column headers

insert [`trade; ([] dt:2021.11.01+1 ; sym:`JPM`UBS; price:1 2; size: 100 200)]

dt        |sym  |price| size
----------------------------
2021-01-01|C	|10   | 100
2021-01-02|C	|20   | 200
2021-01-03|MS   |30   |	300
2021-01-04|C	|40   | 400
2021-01-05|AAPL	|50   |	500
2021-11-01|JPM	|1    | 100
2021-11-02|UBS	|2    | 200

/ have to use backtick table in order to amend the underly table
```

**🔵 13.9 Insert the following record into stock**

```q
sym|sector|employees
--------------------
FB |Tech  | 100

`stock insert (`FB; `Tech; 100)

sym  |sector|employees
---------------------
MS   |Fin   | 100
C    |Fin   | 100
AAPL |Tech  | 100
FB   |Tech  | 100

/ insert values without header
/ `FB automatically becomes keyed since table column sym is keyed
/ remember to backtick `stock
```

**🔵 13.10 In the stock table, change the number of employees for C to 300**

```q
stock upsert (`C;`Fin;300)

/ to update table values, use UPSERT
/ don't need backtick on table name
```

alternative solution:

```q
/ alternative syntax
/ but this requires headers

stock upsert ([sym: enlist`C] employees: enlist 300)

sym|sector|employees
--------------------
C  |Fin   |300

/ have to use enlist to create a vector for an atom
```

**🔵 13.11 Sort the stock table by sym**

```q
`sym xasc `stock

sym |sector| employees
--------------------
AAPL|Tech  | 100
C   |Fin   | 100
MS  |Fin   | 100

/ syntax always goes column name xasc table name
/ backtick stock table to save underlying table
```

<a name="keyed_tables"></a>
## 🔴 14. Keyed Tables
[Top](#top)

<a name="single_keyed_table"></a>
### 🔵 14.1 Single Keyed Table

```q
( [id: `a`b`c`e] name:`jane`jim`kim`john; employer:`citi`citi`ms`ts; age: 11 22 33 44)

id |name|employer| age
----------------------
`a`|jane|  citi  | 11
`b`|jim |  citi  | 22
`c`|kim |    ms  | 13
`e`|john|    ts  | 15

/ the [ ] square bracket holds the key columns
```

<a name="multi_keyed_table"></a>
### 🔵 14.2 Multi Keyed Table

```q
kt: ( [id:`a`b`c`d; name:`jane`jim`kim`john] employer:`citi`citi`ms`ts; age: 11 22 33 44)

id | name |employer| age
----------------------
`a`|`jane`|  citi  | 11
`b`|`jim` |  citi  | 22
`c`|`kim` |   ms   | 13
`e`|`john`|   ts   | 15

/ columns id and name are both keyed columns
```

Repeating Keys

```q
lt: ([a:1 2 2 3] val:`a`b`c`d)

`a` | val
---------
`1` |  a
`2` |  b
`2` |  c
`3` |  d

/ KDB allows for non-unique keys
/ so you have to be careful
/ when you see a keyed table, don't assume keys are unique

lt 2

key | value
-----------
val | b

/ when retrieving, returns FIRST instance 
/ even tho multiple 2, only returns value = b
```

<a name="retrieving_keysvalues"></a>
### 🔵 14.3 Removing Columns from keyed table

```q
/ you CANNOT delete/drop/remove columns from a KEYED table
/ must first UNKEY, then drop the columns

tab1:([id:"abc"]pupil:`john`paul`rachel;subject:`maths`physics`chem;mark:96 55 82)

`id` | pupil  | subject | mark
------------------------------
`a`  | john   |	maths   |  96
`b`  | paul   |	physics |  55
`c`  | rachel |	chem	|  82

/ tab1 is a keyed table (id column)

0!tab1
/ unkeys the table

(enlist`id)_tab1

/ after you UNKEY the table, you can drop columns
/ need enlist since single column

id | pupil  | subject | mark
------------------------------
a  | john   |	maths   |  96
b  | paul   |	physics |  55
c  | rachel |	chem	|  82
```

<a name="retrieving_keysvalues"></a>
### 🔵 14.3 Retrieving Keys/Values

```q
/ retrieve keys as 

key kt

id| name
---------
a | jane
b | jim
c | kim
d | john

/ key will return the entire column of keyed results
```

```q
/ retrieve ONLY the column names that are keyed

keys kt

`id`name

/ KEYS will only return the column names that are keyed!
```

```q
/ retrieve values

value kt

employer|age
------------
citi    | 11
citi    | 22
ms      | 33
ts      | 44

```

<a name="changing_keys"></a>
### 🔵 14.4 Changing Keys (xkey)
```q
table kt
`id`|name|employer| age
----------------------
`a` |jane|  citi  | 11
`b` |jim |  citi  | 22
`c` |kim |    ms  | 13
`e` |john|    ts  | 15

/ only id column is keyed for now
```

```q
/ add name col as key

`id`name xkey `kt

id | name |employer| age
----------------------
`a`|`jane`|  citi  | 11
`b`|`jim` |  citi  | 22
`c`|`kim` |   ms   | 13
`e`|`john`|   ts   | 15

/ changed key columns to both id and name
/ use backtick kt to change underlying table
```

<a name="adding_keys"></a>
### 🔵 14.5 Adding Keys (xkey)

```q
1!kt

`id`|name|employer| age
----------------------
`a` |jane|  citi  | 11
`b` |jim |  citi  | 22
`c` |kim |    ms  | 13
`e` |john|    ts  | 15

/ adds first column as a key
```

alternative syntax:

```q
`id xkey kt

`id`|name|employer| age
----------------------
`a` |jane|  citi  | 11
`b` |jim |  citi  | 22
`c` |kim |    ms  | 13
`e` |john|    ts  | 15

/ same thing, just diff syntax
```

<a name="removing_keys"></a>
### 🔵 14.6 Removing Keys (xkey)

```q
0!kt

id |name|employer| age
----------------------
a  |jane|  citi  | 11
b  |jim |  citi  | 22
c  |kim |    ms  | 13
e  |john|    ts  | 15
```

alternative syntax:

```q
() xkey `kt

id |name|employer| age
----------------------
a  |jane|  citi  | 11
b  |jim |  citi  | 22
c  |kim |    ms  | 13
e  |john|    ts  | 15

/ same thing, just diff syntax
```

<a name="upsert_keys"></a>
### 🔵 14.7 Adding 2 Keyed Tables Together

```q
/ for keyed tables, use UPSERT instead of INSERT!!

kt: ( [id:`a`b`c`d; name:`jane`jim`kim`john] employer:`citi`citi`ms`ts; age: 11 22 33 44)

`id`|`name`|employer| age
----------------------
`a` |`jane`|  citi  | 11
`b` |`jim` |  citi  | 22
`c` |`kim` |   ms   | 13
`e` |`john`|   ts   | 15

nd: ( [id:`e`f] name:`dan`kate; employer:`walmart`walmart; age:200 200)

id |name|employer|age
----------------------
`e`|dan | walmart|200
`f`|kate| walmart|200

/ both table kt and nd have same schema (column names same)
/ and both tables are keyed
```

```q
/ join the 2 keyed tables together

upsert[`kt;nd]

`id`|name|employer|age
----------------------
`a` |jane|citi    |11
`b` |jim |citi    |22
`c` |kim |ms      |13
`e` |dan |walmart |200
`f` |kate|walmart |200

/ if key exists and matches, updates value
/ if new key, adds new row
/ a, b, c = unch
/ since key e already exists, overrides values for name, employer, age
/ must make sure underlying keyed columns match, otherwise error. (1 keyed col vs 2 keyed col)
```

Upsert 2 rows to Keyed Tables

```q
/ upsert id: `f`g; name: `ron`tom to table kt

upsert [`kt; ( [id:`f`g] name:`ron`tom)]

id |name|employer|age
----------------------
`a`|jane|citi    |11
`b`|jim |citi    |22
`c`|kim |ms      |13
`e`|dan |walmart |200
`f`|ron |walmart |200
'g'|tom |        |

/ when upserting rows to a keyed table, need column names
/ f key exists, so key UPDATED to ron
/ and since no other VALUES exist, pulls existing values from existing kt table (kate's old values)
/ g is NEW key, so adds new row. 
/ since no values for employer and age, returns null
```

<a name="upsert_multi_rowkeys"></a>
### 🔵 14.8 Upserting Multi Rows/Keys

```q
et: ([employer:`kx`ms`ms; loc:`NY`NY`HK] size: 10 20 30; area: 1 2 3)

`employer`|`loc`|size|area
--------------------------
`kx`      |`NY` | 10 | 1
`ms`      |`NY` | 20 | 2
`ms`      |`HK` | 30 | 3
```

```q
/ add 2 rows to keyed table et

upsert [et; ([employer:`kx`ms; loc:`NY`SG] size: 9 10)]

employer|loc |size|area
-----------------------
`kx`    |`NY`|9   |1
`ms`    |`NY`|20  |2
`ms`    |`HK`|30  |3
`ms`    |`SG`|10  |	

/ need column names when upserting
/ key columns kx + NY exist, so updates size from 10 to 9
/ since no value for area, pulls in existing value from et (1)
/ no key ms + SG exists, so adds new row with size = 10.
/ no value for area, so returns null
```

<a name="retrieve_single_value_keys"></a>
### 🔵 14.9 Retrieving Values from SINGLE KEY Table

```q
kt: ( [id:`a`b`c`d] name:`jane`jim`kim`john; employer:`citi`citi`ms`ts; age: 11 22 33 44)

`id`|name|employer|age
----------------------
`a` |jane|  citi  | 11
`b` |jim |  citi  | 22
`c` |kim |    ms  | 33
`d` |john|    ts  | 44

/ table kt with id column keyed
```

<a name="ret1"></a>
### 🔵 14.10 Retrieve SINGLE ROW as a DICTIONARY <br/>
(SINGLE KEY TABLE)

```q
kt`a

Key	 | Value
----------------
name	 |  jane
employer |  citi
age	 |    11

/ returns values of key a as a dictionary
```

<a name="ret2"></a>
### 🔵 14.11 Retrieve MULTI ROWS as a DICTIONARY <br/>
(SINGLE KEY TABLE)

```q
/ PREFERRED SYNTAX
/ table lookup method
/ return values of multiple keyed columns as a dictionary

kt ( [] id:`a`b)

name | employer | age
----------------------
jane |   citi   | 11
jim  |   citi   | 22

/ NOTE - even tho column id is KEYED
/ when you retrieve, you leave [ ] blank
/ and simply retrieve the column names id:`a`b
/ retrieves values from keyed columns a and b as a dictionary
```

Retrieve MULTI ROWS as a DICTIONARY <br/>
(SINGLE KEY TABLE)

```q
/ alternative syntax, but NOT preferred

kt[flip enlist `a`b]

name | employer | age
----------------------
jane |   citi   | 11
jim  |   citi   | 22

/ returns values from both keys a and b as a dictionary
```

<a name="ret3"></a>
### 🔵 14.12 Retrieve SINGLE ROW as a TABLE <br/>
(SINGLE KEY TABLE)

```q
/ use TAKE # Method

( [] sym:enlist`b) # t1

`sym` | ex  | size
----------------
`a`   | one | 100

/ need ENLIST since only 1 row
/ by using take #, you return a table
/ includes the KEY column
```

<a name="ret4"></a>
### 🔵 14.13 Retrieve MULTI ROWS as a TABLE <br/>
(SINGLE KEY TABLE)


```q
/ uses TAKE # function

( [] id:`a`b) # kt

`id`|name |employer| age
-------------------------
`a` | jane|  citi  | 11
`b` | jim |  citi  | 22

/ uses the #take function to lookup values in column id
/ notice it also returns the key column (id)
/ NOTE - even though underlying table column id is keyed
/ when you retrieve, you leave [ ] blank
```

<a name="retrieve_multi_value_keys"></a>
### 🔵 14.14 Retrieving Values from MULTI KEY table

```q
et: ([employer:`kx`ms`ms; loc:`NY`NY`HK] size: 10 20 30; area: 1 2 3)

`employer`|`loc`|size|area
--------------------------
`kx`      | `NY`| 10 | 1
`ms`      | `NY`| 20 | 2
`ms`      | `HK`| 30 | 3

/ two keyed columns: employer and loc
```

<a name="ret5"></a>
### 🔵 14.15 Retrieve SINGLE ROW as a DICTIONARY <br/>
(MULTI KEY TABLE)

```q
/ Retrieve values for keys ms + HK as a DICTIONARY

et`ms`HK

key  | value
------------
size |  30
area |   3

/ will lookup the keys for `ms + `HK and return the VALUES as a dictionary
```

<a name="ret6"></a>
### 🔵 14.16 Retrieve MULTI ROWS as a DICTIONARY <br/>
(MULTI KEY TABLE)

```q
/ TABLE LOOKUP method
/ PREFERRED syntax

et ( [] employer:`ms`kx; loc:`HK`NY)

size|area 
---------
 30 | 3
 10 | 1

/ notice you have to specify the column names 
/ when using table retrieve
/ NOTE - even tho underlying table is keyed
/ when retrieving, leave [ ] BLANK
/ and simply call the col names
```

Retrieving MULTI ROWS as a DICTIONARY <br/>
(MULTI KEY TABLE)

```q
/ alternative syntax (less preferred)

et(`ms`HK; `kx`NY)

size|area 
---------
 30 | 3
 10 | 1

/ returns values for both `ms + `HK (30 and 3) and `kx + `NY (10 and 1)
```

<a name="ret7"></a>
### 🔵 14.17 Retrieve SINGLE ROW as a TABLE <br/>
(MULTI KEY TABLE)

```q
( [] employer:enlist`kx; loc:`NY) # et

`employer`|`loc`|size|area
--------------------------
`kx`      | `NY`| 10 | 1

/ have to use ENLIST for single row
/ NOTE - even though underlying table is keyed
/ when RETRIEVE using TAKE #
/ leave the [ ] blank
```

<a name="ret8"></a>
### 🔵 14.18 Retrieve MULTI ROWs as a TABLE <br/>
(MULTI KEY TABLE)

```q
/ Uses the TAKE # function

( [] employer:`ms`kx; loc:`HK`NY) # et

employer | loc | size | area
----------------------------
ms	 | HK  |   30 |   3
kx	 | NY  |   10 |   1

/ using TAKE # returns a table which includes the KEY columns
/ NOTE - even tho underlying table is keyed
/ when retrieving, leave [ ] BLANK
/ and simply call the col names
```

<a name="retrieve_value_keys"></a>
### 🔵 14.10 xgroup/ungroup Tables

```q
/ can group table by particular column using xgroup
/ similar to "by" statement in qSQL

`sym`date`time xgroup trade

sym  date       time        | price    size  cond
----------------------------| -------------------
C    2021.11.04 09:30:02.553| 107.2018 63500 ,"B"
MSFT 2021.11.04 09:30:02.701| 96.87488 1700  ,"B"
RBS  2021.11.04 09:30:02.743| 97.11338 80700 ,"C"

/ equilvalent of saying: 

select price, size, cond by sym, date, time from trade

/ flatten this data out again using ungroup

ungroup select price, size, cond by sym, date, time from trade
```

<hr>

<a name="keyed_table_problem_set"></a>
## 🔴 15. Keyed Tables Problem Set
[Top](#top)

**🔵 15.1 Create the following keyed table**
```q
table p

`book`| `ticker`| size
----------------------
`A`   | `MS`    | 100
`B`   | `AAPL`  | 200
`B`   | `MS`    | 300
`C`   | `C`     | 400
```

```q
p: ( [book:`A`B`B`C; ticker:`MS`AAPL`MS`C] size:100 200 300 400)

/ book and ticker are keys
/ must use backtick for values
/ no ; after the []
/ no commas between values
```

**🔵 15.2 Retrieve entries where book is B, using select**
```q
select from p where book=`B

book | ticker|size
------------------
`B`  | `AAPL`| 200
`B`  | `MS`  | 300
```

**🔵 15.3 Retrieve entries where book is C and ticker is c, using take**
```q

( [] book:enlist`C;ticker:enlist`C) # p

book | ticker| size
-------------------
`C`  | `C`   | 400

/ need to use enlist since only one row
/ NOTE - even tho underlying table is keyed
/ when retrieving, leave [ ] BLANK
/ and simply call the col names
```

**🔵 15.4 Upsert the following values**

```q
/ upsert the values surrounded by **

p
`book` | `ticker`|size
----------------------
`A`    | `MS`    | 100
`B`    | `AAPL`  | 200
`B`    | `MS`    | 300
`C`    | `C`     |**400**
**`D`**|**`MS`** |**500**

upsert [p; ( [book:`C`D; ticker:`C`MS] size:400 500) ]

/ for `C`C -> updates old value to 400
/ `D`MS 500 -> adds new row
```

<hr>

<a name="table_attributes"></a>
## 🔴 16. Table Attributes
[Top](#top)

```q
Attributes describe how the underlying data in lists are structured
This speeds up queries and optimizes memory usage

1. Sorted 's# - items in ascending order (binary search)
2. Unique 'u# - each element is unique (no dupes)
3. Grouped 'g# - dict maps each occurence to position in array
4. Parted 'p# - stores same items together; dict maps first occurence
```

<a name="set_attribute_creation"></a>
### 🔵 16.1 Setting Attributes During Creation

```q
l:`s# 1 2 3 4 5 
1 2 3 4 5

/ applies the sorted attribute during creation of the list

attr l
's

/ checks what attributes are applied to list l
/ 's means sorted attribute applied
```

<a name="apply_attribute_data"></a>
### 🔵 16.2 Applying Attribute to Existing Data
```q
k: 1 2 3 4 5
@ [ `.; `k;`s#]

/ @ = apply
/ `. = within the default name space
/ within the default name space, apply the sorted attribute to list k

attr k
`s

/ confirms list k now has the `s# sorted attribute
```

<a name="update_attribute_data"></a>
### Updating Attribute to Existing Data

```q
table t:

time     name val
------------------
08:00:00 |joe| 10
08:30:00 |jim| 20
09:10:00 |bob| 30

meta t

c    |t|f|a
-----------
time |t| |
name |s| |	
val  |j| |	

/ t = type = time, sym, int
/ f = foreign keys (none)
/ a = attributes (none)
```
```q
update `s#time from `t

/ update column time from table t with the sorted attribute

c     t f a
-----------
time |t| |s
name |s| | 	
val  |j| |

/ attributes for time now has s (sorted) applied
```

<a name="clear_attribute"></a>
### 🔵 16.3 Clear Attributes

```q
@ [`.;`k;`#]

attr k
`
```

<a name="fast_attribute"></a>
### 🔵 16.4 Attribute Benefits

```q
k: til 1000000
0 1 2 3...999,999

\t do[1000; k?500000]
130

/ time 1,000 lookups for the number 500,000 in list k
/ it took 130 miliseconds

`s#k

/ appy the sorted attribute to list k

\t do[1000; k?500000]
0

/ after applying sort attribute, only took 0 miliseconds
/ applying sort applies a binary search. 
/ start in the middle, (ex 5), less than that, so checks mid (ex 3), more, so 4
```

<a name="sort_attribute"></a>
### 🔵 16.5 Sorted Attribute
```q
/ sorted attribute applied to list or column sorted in ascending order
/ requires elements to be sorted ascending, otherwise error
/ `s# attribute only maintained on sorted append, lost on other modification
/ allows binary search instead of linear (fully scanning), so much faster
```
```q
list: 1 2 3 4 5
`s#list

/ apply sorted attribute to list

attr list
`s

/ checks what attributes are applied to list
/ confirms sorted attributed applied

list,: 6

/ add 6 to list

attr list
`s

/ checks attributes for list
/ the sort attribute maintained since 6 is in ascending order to list

list,:3
/ adds 3 to list

attr list
`
 
/ sort attribute LOST because 3 is not ascending to existing list
/ cannot apply sort attribute because underlying list is NOT ascending
```

<a name="unique_attribute"></a>
### 🔵 16.6 Unique Attribute

```q
'u#listname

/ unique attribute signifies all elements of list are unique 
/ creates unique hash table in the background, allowing for constant time lookup of elements
/ mainly used for single keyed tables and big dictionaries
/ maintained on unique append
```

```q
lu:`u#1 2 3 4 5
`u

/ apply unique attribute to list

lu,:7

/ appends 7 to list 

attr lu
`u

/ list lu still has unique attribute since underlying elements all unique

lu,:4

/ adds 4 to list lu

attr lu
`

/ loses unique attribute since 4 already exists
```

<a name="group_attribute"></a>
### 🔵 16.7 Grouped Attribute
```q
'g#listname

/ creates an index of each location in the list of each element
/ groups same identifiers together for faster searches
/ no searching, no requirement on order or content
/ however, requires significcant memory overhead

`a`b`c`a`a`a`b`b`b`c`b`a

`a | 0 3 4 5 11
`b | 1 6 7 8 10
`c | 2 9
```

```q
a:`g#`a`a`b`a`d`c`c

group a

key | value
------------
a   | 0 1 3
b   | ,2
d   | ,4
c   | 5 6
```

```q
lg: 1 3 2 3 2 1 2 3
@ [`.;`lg;`g#]

/ @ = apply
/ `. = within the default name space
/ g# = group attribute
/ within the default name space, apply the group attribute to list lg

attr lg
`g

/ confirms group attribute applied to list lg

group lg

key|value
--------
1  | 0 5
3  | 1 3 7
2  | 2 4 6

/ stores lookup table from values to indices where they occur
```

<a name="parted_attribute"></a>
### 🔵 16.8 Parted Attribute
```q
/ parted attribute marks a list of having same value occuring in sequential blocks
/ breakpoints of elements stored - no more searching, contiguous reads
/ lost on any modification
/ mainly used for on-disk queries
```
```q
lp:`p#`a`a`a`b`b`b`c`c`c

/ applied parted attribute to list lp

attr lp
`p

/ confirms parted attribtue applied to list lp

lp,:`a

/ appends a to list

attr lp
`
/ loses group attribute since a now isnt in sequential block
```

<hr>

<a name="fkey_restrictions"></a>
## 🔴 17. Foreign Key Restrictions
[Top](#top)

```q
/ foreign keys RESTRICT the values that are allowed in a column
/ domain table has to be keyed!
```

<a name="single_fkey"></a>
### 🔵 17.1 Single Foreign Keys

```q
/ company table = domain table
/ column sym is KEYED

company:([sym:`TS`KX`C`AAPL`GOOG`MS] advice: 6?`HOLD`BUY`SELL; level: 6?100)
company
sym   |advice| level
---------------------
`TS`  | HOLD | 40
`KX`  | HOLD | 51
`C`   | SELL | 55
`AAPL`|	BUY  | 90
`GOOG`|	SELL | 73
`MS`  |	SELL | 90

employee:( [] name:`ryan`charlie`arthur`greg; employer:`TS`KX`KX`MS)

employee 
name   |employer
-----------------
ryan   | TS
charlie| KX
arthur | KX
greg   | MS
```

```q
/ set an FKEY for the [employer column] from [employee table] 
/ to the domain of [company table]

update `company$employer from `employee

/ syntax: update `DOMAIN_TABLE $ COLUMN_NAME from `TABLE_NAME

/ similar syntax to casting
/ limits the VALUES in [employer column] 
/ to the DOMAIN in [company table] (KEYED sym column)
/ the domain table HAS to be keyed
/ the values in [employer column] MUST EXIST in domain [company table]
```

<a name="check_fkey"></a>
### 🔵 17.2 Checking Foreign Keys

```q
/ use meta

meta employee

c       |t|f      |a
----------------------
name    |s|       |		
employer|s|company| 	

/ c = column
/ f = foreign key
/ confirms the employer column is linked to the company table (last example)
```

```q
fkeys employee

key     |value
----------------
employer|company

/ fkeys + table name = what columns are foreign keyed
```

<a name="upsert_fkey"></a>
### 🔵 17.3 Upserting with Foreign Keys

```q
/ upsert name:`james`claire and employer:`RBS`RBS into the [employee table]

upsert[employee; ( [] name:`james`claire; employer:`RBS`RBS)]
`cast

/ `cast error because RBS is NOT a sym in the company table
/ prev set [employer column] as fkey to [company table] domain (keyed sym column)
/ fkey restricts us from adding what's NOT in the domain  
```

```q
/ need to FIRST add RBS into the company domain (as a keyed sym)
/ remember  need to use enlist when adding single rows

insert[`company; ([sym:enlist `RBS] advice:enlist `SELL; level: enlist 20)]

company
sym   |advice| level
---------------------
`TS`  | HOLD | 40
`KX`  | HOLD | 51
`C`   | SELL | 55
`AAPL`|	BUY  | 90
`GOOG`|	SELL | 73
`MS`  |	SELL | 90
`RBS` | SELL | 20
```

```q
/ now you can append james and claire

upsert[employee; ( [] name:`james`claire; employer:`RBS`RBS)]

employee 
name   |employer
-----------------
ryan   | TS
charlie| KX
arthur | KX
greg   | MS
james  | RBS
claire | RBS
```

<a name="retrieve_fkey"></a>
### 🔵 17.4 Retrieving Columns via fkey

```q
/ if TABLE A is our domain table (keyed)
/ and we set a column in TABLE B to the fkey of TABLE A
/ we can PULL any columns from TABLE A to TABLE B
/ since the 2 tables are linked via the fkey
```

```q
company
sym   |advice| level
---------------------
`TS`  | HOLD | 40
`KX`  | HOLD | 51
`C`   | SELL | 55
`AAPL`|	BUY  | 90
`GOOG`|	SELL | 73
`MS`  |	SELL | 90
`RBS` | SELL | 20

employee
name   |employer
-----------------
ryan   | TS
charlie| KX
arthur | KX
greg   | MS
james  | RBS
claire | RBS

meta employee
c       |t|   f   |a
----------------------
name    |s|       |		
employer|s|company| 	

/ meta tell us the [employer column] from [employee table]
/ has an fkey linked to the domain of [company table]
```

```q
/ from the [employee table], retrieve the values from the [advice column]
/ and the [level column] from the [company table]

update employer.advice, employer.level from employee

name   |employer|advice|level
---------------------------
ryan   |TS	|SELL  |12
charlie|KX      |BUY   |10
arthur |KX      |BUY   |10
greg   |MS      |SELL  |90

/ prev you keyed the [employer column] to domain of [company table]
/ so the [employer column] is your LINK to the [company table]
/ update a new column will ADD the new column to the table
/ pulls in VALUES from [advice column] and [level column] from [company table]
```

<a name="multi_fkey"></a>
### 🔵 17.5 Multiple Foreign Key Problem Set

```q
office: ([sym:`TS`KX`C; loc:`LDN`NY`LDN] employees:10+3?1000)

office
`sym` | `loc`  | employees
---------------------------
`TS`  | `LDN`  | 875
`KX`  | `NY`   | 354
`C`   | `LDN`  | 1007

/ columns SYM and LOC are KEYED

employee: ([] name:`ryan`charlie`arthur; employer:`TS`KX`KX; city:`LDN`NY`NY)

employee
name   |employer|city
-------------------
ryan   |TS      |LDN
charlie|KX      |NY
arthur |KX      |NY
```

Set the fkey for employee table

```q
/ fkey the [employer] and [city] columns from [employee]
/ to the domain of [office] table

exec `office$flip (employer;city) from employee
0 1 1

/ since the [office table] has 2 keyed columns
/ you have to "cast" the 2 columns as fkey
/ ignore the flip syntax
/ set fkey by linking the [EMPLOYER column] and [CITY] from [employee table]
/ to the domain of [office table] (keyed columns)

/ ryan    -> look for TS and LDN in office table, found on row 0
/ charlie -> look for KX and NY in office table, found on row 1
/ arthur  -> look for KX and NY in office table, found on row 1
```

Add new column to employee table

```q
/ from [employee table]
/ add new column called [empOffice]
/ which returns the INDEX LOCATION of fkey [employer] and [city] columns
/ from the [office table]

update empOffice:`office$flip(employer;city) from `employee

employee
name   |employer|city|empOffice
-----------------------------
ryan   |TS      |LDN |	0
charlie|KX      |NY  |	1
arthur |KX      |NY  |	1

/ adds new column [empOffice], and sets fkey to domain of [office table]

/ ryan    -> look for TS and LDN in office table, found on row 0
/ charlie -> look for KX and NY in office table, found on row 1
/ arthur  -> look for KX and NY in office table, found on row 1
```

Check meta of employee table

```q
/ check if the new column empOffice has an fkey

meta employee
c        |t|  f   | a
----------------------
name     |s|	  |	
employer |s|	  |
city     |s|	  |
empOffice|j|office|

/ meta shows us [empOffice] has an foreign key 
/ referencing the [office table]
```

Retrieve fkey values

```q
/ add to the [employee table]
/ new columns [sym] and [loc] from the [office table]
/ using the fkey from the [empOffice column]

update empOffice.sym, empOffice.loc from employee

name   |employer|city|empOffice| sym| loc
-------------------------------------------
ryan   |   TS   |LDN |	 0     | TS | LDN
charlie|   KX   |NY  |   1     | KX | NY
arthur |   KX   |NY  |   1     | KX | NY

/ prev set [empOffice column] as foreign key
/ to the domain of [office table]
/ so you can pull in values from [office table]
```

<hr>

<a name="fkey_problemset"></a>
## 🔴 18. Foreign Key Problem Set
[Top](#top)


```q
book: ([id:`fmgoh`fddig`lefhe`bfjnf] name:`jim`allen`bob`sherman)

book
`id`    | name
----------------
`fmgoh` | jim
`fddig` | allen
`lefhe` | bob
`bfjnf` | sherman

trade:([] date:2021.01.01; time: 09:00; sym:`D`AA`UPS`A; price:109 93 34 56; size: 100; cond: " ","B","A","C"; bookID:`fmgoh`fddig`lefhe`bfjnf)

trade
date      |  time | sym |price| size|cond|bookId
-------------------------------------------------
2021.01.01| 09:00 |   D | 109 | 100 |    | fmgoh
2021.01.01| 09:00 |  AA |  93 | 100 | B  | fddig
2021.01.01| 09:00 | UPS |  34 | 100 | A  | lefhe
2021.01.01| 09:00 |   A |  56 | 100 | C  | bfjnf
```

1. Insert new fkey column into trade table

```q
/ Insert new fkey column into [trade table]
/ called [owner], linking the [trade] and [book] table
/ using [bookID]

update owner: `book$bookId from `trade

date      |  time | sym |price| size|cond|bookId | owner
---------------------------------------------------------
2021.01.01| 09:00 |   D | 109 | 100 |    | fmgoh | fmgoh
2021.01.01| 09:00 |  AA |  93 | 100 | B  | fddig | fddig
2021.01.01| 09:00 | UPS |  34 | 100 | A  | lefhe | lefhe
2021.01.01| 09:00 |   A |  56 | 100 | C  | bfjnf | bfjnf

/ so if you ADD the column set as an fkey (bookID)
/ it returns the DOMAIN of the keyed table (keyed columns)
/ [bookID] from [trade] was set as fkey to [book]
/ adding the column returns the keyed column from [book]
```

2. Check the meta to confirm fkey

```q
meta trade

c      | t |   f  | a
-----------------------
date   | d |	  |	
time   | u |	  |	
sym    | s |	  |	
price  | j |	  |	
size   | j |	  |	
cond   | c |	  |	
bookID | s |	  |	
owner  | s | book |	


/ [owner column] from [trade] has an fkey
/ to [book table]
```

3. Retrieving fkey values

```q
/ Join the [book table] onto the [trade table]
/ and add the name of the person who did trade

update owner.name from `trade

date      |  time | sym |price| size|cond|bookId | owner | name
---------------------------------------------------------------
2021.01.01| 09:00 |   D | 109 | 100 |    | fmgoh | fmgoh | jim
2021.01.01| 09:00 |  AA |  93 | 100 | B  | fddig | fddig | allen
2021.01.01| 09:00 | UPS |  34 | 100 | A  | lefhe | lefhe | bob
2021.01.01| 09:00 |   A |  56 | 100 | C  | bfjnf | bfjnf | sherman

/ [owner column] has an fkey set to [book table]
/ so you use that column to pull values from [book table]
/ name = column name from book you want to retrieve values from
```

<hr>

<a name="qsql_header"></a>
## 🔴 19. qSQL
[Top](#top)

```q
Evaluated in the following order:
1. from 
2. where (filter data)
3. by (group data)
4. select
```

<a name="select_template"></a>
### 🔵 19.1) Select

```q
/ load sample trades file

\l trades.q

\a
`book`company`employee`office`quote`stock`trade

/ this shows all available tables within the script
```

```q
/1. retrieve entire trade table

select from trade

date       time         sym  price    size  cond
------------------------------------------------
2022.03.19 09:30:02.558 MS   109.1931 56600 C   
2022.03.19 09:30:02.596 AAPL 97.30796 98700 A   
2022.03.19 09:30:02.638 RBS  99.65561 6300      

/ select always results in a table
/ select from trade = select whole table
```

```q
/2. retrieve only the sym and price columns from trade table

select sym, price from trade

sym  | price
--------------
MS   | 109.19
AAPL | 97.307
RBS  | 99.655

/ select + column names = will retrieve columns
```

```q
/3. retrieve only first 2 rows of trade 

2 sublist trade

date	   | time	  | sym | price  | size	 | cond
--------------------------------------------------------
2022-03-19 | 09:30:02.558 | MS	| 109.19 | 56600 | C
2022-03-19 | 09:30:02.596 | AAPL| 97.307 | 98700 | A

/ sublist returns the first xx rows of table
```

```q
/4. select the high, low, open, and close price by sym from trade table

select high: max price, low: min price, open: first price, close: last price by sym from trade

sym  | high  | low  | open | close
----------------------------------
A    | 109.9 | 50.0 | 83.7 | 1.0
AA   | 109.9 | 50.0 | 97.1 | 70.7
AAPL | 109.9 | 50.0 | 97.3 | 98.0

/ grouped by sym
/ select a new column name will add it to your table
```

### Analytics on Grouped Data
```q
select max price by sym from trade
select price by sym from trade
ungroup select price by sym from trade
```

<a name="selectadd_template"></a>
### 🔵 19.2) Adding a new column using select

```q
/ if you select a column name that doesnt exist, it will append it

select sym, price, size, total:price*size from trade

sym  | price | size  |  total   
-------------------------------
C    | 107.2 | 63500 | 6807314 
MSFT |  96.8 | 1700  |  164687
RBS  |  97.1 | 80700 | 7837050 

/ new column named total is returned
```

<a name="qsqlvirtuali_template"></a>
### 🔵 19.3) Virtual Column i

```q
/ q provides a virtual column i
/ which represents the "offset" of each record
/ useful for counting how many rows

select i, sym, price from trade

x | sym  | price   
-----------------
0 | C    | 107.2
1 | MSFT |  96.8
2 | RBS  |  97.1
3 | A    | 100.35  
4 | B    |  55.8

/ column x = virtual column i 
```

```q
/ example 2

/ how many of each sym is there with cond = A from trade table?

select count i by sym from trade where cond="A"

`sym`  |  x
--------------
`A`    | 12525
`AA`   | 12648
`AAPL` | 12451

/ since you are grouping by sym
/ the sym column becomes keyed
```

<a name="qsqlselectmaxmin_template"></a>
### 🔵 19.4) Select using [ ]

```q
/ select [] can be used to get the first n or last n records of a table
/ select [n m] can be used to get records starting from n and upto count m from n

select [4] from trade

date       | time	  | sym  | price | size | cond
-------------------------------------------------------
2022-03-19 | 09:30:02.553 | C	 | 107.2 |63500 | B
2022-03-19 | 09:30:02.701 | MSFT | 96.8	 | 1700	| B
2022-03-19 | 09:30:02.743 | RBS	 | 97.1	 |80700	| C
2022-03-19 | 09:30:02.758 | A	 | 100.3 |50300 | B

/ selects the first 4 records
```

```q
select [-3] from trade

date       | time	  | sym  | price | size | cond
-------------------------------------------------------
2022-03-19 | 09:30:02.553 | C	 | 107.2 |63500 | B
2022-03-19 | 09:30:02.701 | MSFT | 96.8	 | 1700	| B
2022-03-19 | 09:30:02.743 | RBS	 | 97.1	 |80700	| C

/ selects the last 3 records
```

```q
select [1 4] from trade

/ skips 0, returns 1, 2, 3, 4
```

<a name="select_from_where"></a>
### 🔵 19.5) Where

```q
/ the WHERE clause allows for filtering your query
/ operates left to right, so put most restrictive clause first
/ use commas for multiple where expressions
```

### Sample Where Clauses

```q
select from trade where size>300, price>100
select from trade where sym in `AAPL`GOOG
select from trade where grade = "ABC"
select from trade where price within (200:300)
select from trade where (price>100) and size>300
select from trade where (price>100) or size> 300
select i, sym, price from trade where i>5
select price, i by sym from trade
select price by date from trade where sym=`AAPL, price < avg price
select {x % max x} price by date from trade where sym=`AAPL, price < avg price, date=.z.d
select from trade where sym in `AAPL`RBS
```

```q
/ 1. retrieve trades for sym A on 2021.05.29

select from trade where date=2021.05.29, sym=`A

date      | time        | sym |price| size | cond
--------------------------------------------------
2021-05-29| 09:30:02.758|  A |100.35| 50300| B
2021-05-29| 09:30:17.997|  A |57.81 | 65600| C
2021-05-29| 09:30:21.507|  A |97.85 | 51800| B

/ where filters use = to specify value
/ notice commas separate where clauses
```

```q
/2. retrieve prices on 2021.05.29 for sym A

select price from trade where date=2021.05.29, sym=`A

price
-----
100.3
57.8
97.8

/ since you only selected price column
/ only a single column returned
```

```q
/3. retrieve max price on 2021.05.29 for sym A

select max price from trade where date=2021.05.29, sym=`A

price
------
109.99

/ can perform "functions" on select clauses
/ max price
/ min price
/ avg price
/ etc
```

```q
/4. count how many trades have condition A

count select from trade where cond="A"
211597

/ the count function tallies the number of rows
/ from your query
```

```q
/5. retrieve all trades from today, aggregated by sym

select by sym from trade where date=.z.d

sym  |  date    |   time     |price|size |cond
----------------------------------------------
A    |2021-06-02|17:29:57.306|87.54|49100|B
AA   |2021-06-02|17:29:58.789|68.09|88100|A
AAPL |2021-06-02|17:29:58.262|76.18|22500|A

/ the BY CLAUSE is used for aggregations
/ groups all trades by sym and sets column as key
```

### Where Clause Table Filter - Example 1

```q
/ you can apply the WHERE clause filter
/ based on values from in another table

t1: ([] date: 2021.10.21 2021.10.21 2021.10.21 2021.10.21; sym: `GOOG`MSFT`FB`AMZN; exch: `nyse`nyse`nasdaq`nasdaq)
t2: ([] sym: `GOOG`FB; exch: `nyse`nasdaq)

t1
date       | sym  | exch
----------------------------
2021-10-21 | GOOG | nyse
2021-10-21 | MSFT | nyse
2021-10-21 | FB	  | nasdaq
2021-10-21 | AMZN | nasdaq

t2
sym  | ex
------------
GOOG | nyse
FB   | nasdaq
```

```q
/1. retrieve values from t1 where date is 2021.10.21
/ AND values from [sym] + [exch] columns are found in t2

select from t1 where date=2021.10.21, ( [] sym; exch) in t2

date       | sym  | exch
----------------------------
2021-10-21 | GOOG | nyse
2021-10-21 | FB	  | nasdaq

/ first filters date = 2021.10.21 in t1
/ then it filters a TABLE with column names = [sym;exch] in t2
/ so ONLY the values in t1 that meet ALL criteria are returned
```

### Where Clause Table Filter - Example 2

```q
/ load trades.q script

/ from the trade table, retrieve the following:
/ IBM from cond A
/ CSCO from cond A or B
/ MSFT from cond C 
/ date = 2021.11.17
```

```q
/1. first, check the meta of the trade table

meta trade

c    |t|f|a
------------
date |d| |s
time |t| |		
sym  |s| |		
price|f| | 		
size |i| |		
cond |c| |		

/ reveals correct datatype to retrieve properly
/ sym = sym 
/ cond = char
```

```q
/ since you have multiple parameters, 
/ it's easier to create a table of these parameters,
/ then use this table as part of your WHERE filter

/2. create new table, toget, with the target parameters

toget:( [] sym:`IBM`CSCO`CSCO`MSFT; cond:"AABC")

sym   cond
----------
IBM    A
CSCO   A
CSCO   B
MSFT   C

/ notice you had to dupe the CSCO
/ since its parameter is A or B
```

```q
/3. Use QSQL to filter the table of parameters

select from trade where date=2021.11.17, ( [] sym; cond) in toget

date       sym  price size cond
-------------------------------
2021-10-30 MSFT	60.66 48700 C
2021-10-30 IBM	59.00 28300 A
2021-10-30 MSFT	54.57 23700 C
2021-10-30 IBM	89.19 86600 A
2021-10-30 IBM	84.13 46600 A

/ first filters by date 2021.11.17
/ then filters by the values in the [sym] and [cond] columns
/ from the [toget] table
```

### Where Clause Ordering

```q
/ be careful about how you order the where filters
/ can change your output

trade:( [] price: 50 60 70; size: 300 200 100)

price   size
------------
50	300
60	200
70	100
```

```q
/ find largest price and size > 200

select from trade where size > 200, price = max price

price   size
------------
50	300

/ however, this is NOT correct as 50 is NOT the max price
```

```q
/ correct query

select from trade where price = max price, size > 200

price   size
------------

/ this is correct. 
/ no max price (70) that is greater than 200 (300)
```

### Where Clause Table Filter - Example 3

```q
results:( []name:`John`Paul`Rachel`Jane`Emma;gender:"MMFFF";grade:"ABBAC")

name  |gender|grade
--------------------
John  |   M  | 	A
Paul  |   M  |	B
Rachel|   F  |	B
Jane  |   F  |	A
Emma  |   F  | 	C

/ 1. from the results table, extract all the following:
/ gender - male and grade - A
/ gender - female and grade - B
/ gender - female and grade - A
```

```q
/ 1a. show the syntax individually for each query

select from results where gender="M", grade="A"
select from results where gender="F", grade="B"
select from results where gender="F", grade="A"

name  |gender|grade
--------------------
John  |   M  | 	A

name  |gender|grade
--------------------
Rachel|   F  |	B

name  |gender|grade
--------------------
Jane  |   F  |	A
```

```q
/ 2. run the same query, instead running a table filter
/ (which probably cleaner outcome)

select from results where ( [] gender; grade) in ( [] gender:"MFF"; grade:"ABA")

name  |gender|grade
--------------------
John  |   M  | 	A
Rachel|   F  |	B
Jane  |   F  |	A

/ so instead of "creating" a separate table
/ you construct the table of possible outcomes in place
/ then you simply filter using table with column names = [gender]; [grade]
```

<a name="select_by"></a>
### 🔵 19.6) By

```q
/ the BY CLAUSE aggregates data together
/ keys the resulting table
```

```q
/1. find the first price and time for AAPL by date

select first price, first time by date from trade where sym=`AAPL

`date`       | price |    time
-----------------------------------
`2021-05-29` | 78.6  | 09:30:03.025
`2021-05-30` | 60.8  | 09:30:02.686
`2021-05-31` | 55.1  | 09:30:18.274

/ by date = aggregates data by date
/ and keys the date column 
```

```q
/2. find the open, high, low, and close price by date for AAPL

select open:first price, high:max price, low:min price, close:last price by date from trade where sym=`AAPL

date        |open |high  |low |close
------------------------------------
`2021-05-29`|78.66|109.91|50.5|68.01
`2021-05-30`|60.88|109.98|50.0|0.49

/ open: renames the column
```

<a name="select_count"></a>
### 🔵 19.7) Select Count 

```q
/ find the number of total number of trades for RBS grouped by date and hours

select count i, max price by date, time.hh from trade where sym=`RBS

date        |hh   | x   | price
------------------------------
`2021-05-29`|`9`  | 645 | 50.5 
`2021-05-30`|`10` | 154 | 50.0

/ i is a virtual column that returns the number of rows (as column x)
```

<a name="using_ops_functions"></a>
### 🔵 19.8) Using Operations and Functions 

```q
/1. find all AAPL prices that are less than the avg price grouped by date

select price by date from trade where sym=`AAPL, price < avg price

date        | price
--------------------------
`2021-05-29`| 100 99 22 33
`2021-05-30`| 23 199 44 12
```

```q
/2. retrieve prices, keyed by TODAY, where AAPL's price is less than the avg price

select price by date from trade where sym=`AAPL, price < avg price, date=.z.d

date       | price
-------------------------------------
2022.03.23 | 62.4 84.4 29.2 49.4 28.2

/ alternative syntax

select price by date=.z.d from trade where sym=`AAPL, price < avg price

d   | price
--------------
`0` | 23 52 63
`1` | 23 66 12

/ grouped by today; 0 = false, 1 = true
```

```q
/3. retrieve price divide by max price, keyed by today, where the price is less than the avg price

select price by date from trade where sym=`AAPL, price < avg price, date=.z.d

date       | price
--------------------------------
2022.03.23 | 0.77 0.73 0.99 0.94

/ alternative syntax:

select {x % max x} price by date from trade where sym=`AAPL, price < avg price, date=.z.d

date       | price
--------------------------------
2022.03.23 | 0.77 0.73 0.99 0.94

/ this is pretty cool 
/ i haven't seen this before
/ {x % max x} allows you to perform functions
/ on individual columns
```

<a name="in_function"></a>
### 🔵 19.9) In Function

```q
/ the IN function allows you to query if LHS arg is anywhere in RHS arg
/ a faster way of checking "or" arguments
/ useful when you have multiple filters PER single column
/ filtering for multiple syms or multiple conditions
```

```q
/1. retrieve data for AAPL and RBS from trade

select from trade where sym in `AAPL`RBS

date      | time         | sym | price  | size  | cond
------------------------------------------------------
2021-05-30| 09:30:02.743 | RBS | 97.113	| 80700 | C
2021-05-30| 09:30:03.025 | AAPL| 78.66  | 19000	| A

/ in function checks if every LHS argument occurs anywhere in RHS argument (AAPL or RBS)
/ a faster way of checking "or" arguments
```

<a name="within_function"></a>
### 🔵 19.10) Within Function

```q
/ WITHIN checks if LHS argument is within the range on RHS argument
/ has to have lower + upper bind
```

```q
/1. retrieve trades for RBS where price is between 95 and 100

select from trade where sym=`RBS, price within 95 100

date      |time          |sym   |price  | size | cond
------------------------------------------------------
2021-05-30| 09:30:02.743 | RBS  | 97.113| 80700 | C
2021-05-30| 09:30:03.025 | AAPL | 98.66 | 19000	| A
```

```q
/2. retrieve trades for RBS within 95 and 100 and between 11:30 - 12:00

select from trade where sym=`RBS, price within 95 100, time within 11:30 12:00

date      | time          |sym   | price  | size | cond
-------------------------------------------------------
2021-05-30| 11:40:02.743 | RBS   | 97.113 | 80700 | C
2021-05-30| 11:44:03.025 | AAPL  | 98.66  | 19000 | A

/ two within filters, price and time
```

<a name="exec"></a>
### 🔵 19.11b) Aggregating "buckets" using WITHIN

```q
/ another powerful to aggregate data into buckets
/ is by first filtering your parameter using WITHIN
/ then "naming" that "bucket" 

/ load trades.q script
```

```q
/ 1. retrieve the number of small trades for each sym
/ small trades = size less than 999
/ add column called tradesize = small for each sym

select num:count i by sym, sizegroup:`small from trade where size within 0 999

`sym` | `sizegroup` | num
--------------------------
`A`   |   `small`   | 454
`AA`  |   `small`   | 521
`AAPL`|   `small`   | 493
`B`   |   `small`   | 499

/ num = number of trades which sizes are less than 999
/ use COUNT to return NUMBER of trades
/ since you're aggregating BY sym, the sym + sizegroup cols are keyed
/ use WHERE within x y = range of values to be selected
```

```q
/2. now retrieve the number of med and large trades for each sym
/ med = 1000 to 8999
/ large = greater than 8999

/ consolidate into same table

(select count i by sym, sizegroup:`small from trade where size within 0 999),
(select count i by sym, sizegroup:`medium from trade where size within 1000 8999),
(select count i by sym, sizegroup:`big from trade where size > 8999)

`sym | `sizegroup` | num
---------------------------
`A`   | `large`    | 45645
`A`   | `med`      | 4009
`A`   | `small`    | 480

/ we have successfully grouped each sym into "buckets"
/ of either small, med, or large
/ depending on the number of trades (from size)
/ there is a better way retrieve this, by writing function called BIN
```

<a name="bin"></a>
### 🔵 19.11b) BIN function - Creating buckets of aggregation

```q
/ BIN takes LHS defined buckets, and returns index position of RHS list
/ syntax is: size1 size2 size3 bin x
/ x = list

/ 1. Group each element of list size into buckets of 100, 300, 500

size: 100 200 300 400 500 600
100 300 500 bin size
0 0 1 1 2 2

/ 100 = index position 0 (100)
/ 200 = index position 0 (100)
/ 300 = index position 1 (300)
/ 400 = index position 1 (300)
/ 500 = index position 2 (500)
/ 600 = index position 2 (500)
```

```q
/ 2. RENAME these buckets into small, medium, large

`small`medium`large 100 300 500 bin size
`small`small`medium`medium`large`large

/ instead of returning the index position
/ it now "categorizes" the bucket was either small, big, or large
```

```q
/ 3. Create a function that accepts argument x as a list
/ and returns "buckets" of aggregation for small, medium, large trades
/ small < 1000
/ medium = 1000-8999
/ large > 9000

f: {`small`medium`large 0 1000 9000 bin x}
f [500 1000 100000]
`small`medium`large
```

```q
/ 4. use this f function to retrieve the total number of trades
/ grouped by their size bucket (small, medium, large) for each sym

select numtrades:count i by sym, sizebucket:(f;size) fby sym from trade

sym | sizebucket | numtrades
-----------------------------
AA  |   large    | 45425
AA  |   medium   | 3986
AA  |   small    | 502
AAPL|   large    | 45621
AAPL|   medium   | 3974
AAPL|   small    | 511
BAC |   large    | 45551
BAC |   medium   | 3958
BAC |   small    | 3948

/ the f function takes in list of numbers,
/ and returns = small, medium, or large
/ so you need to add a new column (sizebucket)
/ for these outputs
/ utilizes the f function as an aggregator for fby
/ notice you're grouping the count i by sym
/ since this needs to match the agg fby sym
```

BIN example 2:

```q
/ 1. for list of sizes, group into buckets of 0, 1000, or 9000

sizes: 2000 100 6000 11000
0 1000 9000 bin sizes
1 0 1 2

/ bin takes its LEFT hand buckets, and sorts index position of RIGHT argument
/ so sizes = 4 elements, will return index position of bin
/ 2000 = index position 1 bin
/ 100 = index position 0 bin
/ 6000 = index position 1 bin
/ 11000 = index position 2 bin
```

```q
/ 2. name the buckets as small, med, or big
/ based on the buckets of 0, 1000, and 9000

`small`med`big 0 1000 9000 bin sizes
`med`small`med`big

/ syntax: 
/ `name1`name2`name3 size1 size2 size 3 bin LIST
/ still returns the index position based on the sizes
/ but now has a "name" associated to it (small, med, big)
```

```q
/ 3. create function called tradesize
/ that accepts a list of trade sizes as argument x
/ and bucket those sizes into bins of small, med, big

tradesize:{`small`med`big 0 1000 9000 bin x}

/ test out the function with sizes (from above)

sizes: sizes: 2000 100 6000 11000

tradesize sizes
`med`small`med`big

/ it works!
```

```q
/ 4. use this tradesize function to retrieve total number of trades grouped by size bucket

select num:count i by sym, sizebucket:(tradesize;size) fby sym from trade

sym | sizebucket | num
-------------------------
A   | large      | 45645
A   | med        | 4009
A   | small      | 480
AA  | large      | 45425

/ [sizebucket column] -> insert [tradesize function] you created
/ [size column] from [trade table] becomes argument x for [tradesize function]
/ [tradesize function] becomes an AGGREGATOR for fby
/ returns the number of trades (count i), sorted by sym and its size bucket
```

<a name="xbar_function"></a>
### 🔵 19.11) Xbar Function

```q
/ xbar is a powerful function that allows groupings for data
/ generally used for bucketing by TIME
/ but can also be used for price, cond, etc.
```

xbar examples:

```q
select sum size, num_count:count i by sym, 1 xbar price from trade
select max price, sum size by sym, 5 xbar time.minute from trades
select max price by sym, 45 xbar time.minute from trade
select price by sym, 240 xbar time.minute from trade
select avg price by sym, 1 xbar time.hour from trade
```

xbar price

```q
/ grouping for other data buckets (price)
/ apply xbar grouping to price column

x xbar price
x xbar cond
x xbar source
```

xbar price - problem set

```q
/1. retrieve the total size and total number of trades
/ for each sym and each $1 price buckets

select sum size, cnt:count i by sym, 1 xbar price from trade

`sym` |`price`|   size   | cnt
-----------------------------
 `A`  |  `50` | 44191500 | 838
 `A`  |  `51` | 42318700 | 842
 `A`  |  `52` | 41432200 | 832
 `A`  |  `53` | 30434493 | 832

/ groups the data by sym and 1 dollar price buckets
/ cnt = tallies virtual column i
/ ie, how many total trades were executed by sym for that price bucket
```

xbar time

```q
/ grouping for temporal data buckets (time)

x xbar time.minute / x mins buckets
x xbar time.hh / x hour buckets
x bar time.ss / x second buckets

20 xbar time.ss / same thing
0d00:00:20 xbar time / same thing
```

xbar time - problem set

```q
/1. find the max price and total size of trades during 5 min window

select max price, sum size by sym, 5 xbar time.minute from trades

sym  |minute | price|size
-------------------------
AAPL | 08:00 | 27.4 | 100
AAPL | 08:05 | 27.9 | 200
AAPL | 08:10 | 28.2 | 300

/ set xbar as 5 minute time buckets
/ grouped sym, then 5 min time buckets
/ sym + minute are keyed (since by)
```

```q
/2. find the max price by sym for each 45 min window

select max price by sym, 45 xbar time.minute from trade

sym |minute | price
----------------------
 A  |09:00  | 109.94
 A  |09:45  | 109.99
 A  |10:30  | 109.96

/ group by sym, set xbar as 45 minute time buckets
```

Amending xbar time buckets (advanced)

```q
/ notice how in the above example, the time bucket starts at 9:00
/ what if we wanted the 15 min bucket to include 9:30 instead?

select max price by sym, 09:30 + 45 xbar time.minute - 09:30 from trade

sym|minute |price
------------------
 A | 09:30 |109.94
 A | 10:15 |109.99
 A | 10:45 |109.96

/ by adding 9:30 and subtracting 9:30 from xbar, you can shift the time bucket
/ to include your desired time

/ logic here:
/ the 45 xbar time.minute = groups into 45 min buckets
/ subtracting your time 9:30 = you shift the list to include your desired time
/ adding 9:30 = reset to center around your desired time
```

```q
/ to clean this up, you can write the xbar shift as a function

timeshift:{[start;minbar;time] start + minbar xbar(`minute$time) - start}

/ timeshift is a func that takes 3 arguments
/ start = start time
/ minbar = timing you want to bucket by
/ time = times (col)

/ cast time to minutes

select max price by sym, time: timeshift[09:30;45;time] from trade

sym|minute |price
------------------
 A | 09:30 |109.94
 A | 10:15 |109.99
 A | 10:45 |109.96

/ and this will give you the same exact result
/ 9:30 = time you want to start
/ 45 = time bucket
/ time = column to bucket by

/ or you could retrieve total trades and size by sym, grouped by 45 mins

select sum size, cnt: count i by sym, time: timeshift[09:30;45;time] from trade

sym|minute|   size  |cnt
-------------------------
 A |09:30 |242733500|4800
 A |10:15 |223808400|4497
 A |11:00 |247590700|4898
```

```q
select count i, max price by date, xbar [15*60*1000;time] from trade where sym=`RBS

   date   |    time    | x |price
----------------------------------
2021-05-30|11:40:02.743|100|97.113
2021-05-30|11:44:03.025|123|98.66 

/ retrieve number of trades (count) and max price, keyed by date and time 
/ 15 mins x 60 sec x 1000 ms to get to milliseconds
/ xbar rounds its 2nd argument to nearest multiple of first argument (so rounds time to 15 mins)
```

```q
7 xbar 10 20 30 40 50
7 14 28 35 39

/ rounds right argument down to nearest multiple of left argument
```
```q
5 xbar 11:00 + 0 3 5 11
11:00 11:00 11:05 11:10

/ evaluates right to left (11:00 + 0 3 5 11), then 5 xbar
/ rounds down time to nearest 5 min intervals
```

<a name="exec"></a>
### 🔵 19.12) Exec

```q
/ exec is a more general form of select
/ while select always returns a table, exec returns are more flexible
/ exec from one column returns a LIST
/ exec from more than one column returns a DICTIONARY
/ one diff between select and exec is the column lists do not have to be rectangular to return a result
```

```q
a: ( [] c1: 1 2 3; c2: `a`b`c)

c1 | c2
-------
 1 | a
 2 | b
 3 | c
```

```q
/ 1. Exec on a single column

exec c1 from a
1 2 3

/ exec single column returns a list
```

```q
2. exec on multiple columns

exec c1, c2 from a
c1 | 1 2 3
c2 | `a`b`c

/ exec multi columns returns a dictionary
```

```q
/3. exec full table

exec from a

key | value
-------
 c1 | 3
 c2 | c

/ returns a dictionary of LAST values in columns c1 and c2
```

### More Exec Examples

```q
/1. return list of prices for AAPL on today

exec price from trade where date=.z.d, sym=`AAPL
62 59 13

/ exec single column = single list returned
```

```q
2. return column of values for AAPL on today

select price from trade where date=.z.d, sym=`AAPL

price
------
62
59
13

/ select = single column returned
```

```q
/3. return the first price of AAPL today

exec first price from trade where date=.z.d, sym=`AAPL
62

/ exec returns single value
/ select ALWAYS returns a table
```

```q
/4. return ALL prices of AAPL from today as a dictionary

exec price by sym from trade where date=.z.d, sym=`AAPL
AAPL | 62 59 13

/ exec + by sym
/ groups the data by sym
/ and returns a dictionary
```

```q
/5. return all prices from today by sym as a dictionary

exec price by sym from trade where date=.z.d

`sym`  | price
----------------
`A`    | 108 77 88
`AA`   | 33 45 23
`AAPL` | 34 56 23

/ exec + by sym returns a dictionary
```

```q
/6. retrieve first price, cond from today for KX and AAPL as a dictionary

exec first price by sym, cond from trade where date=.z.d, sym in `KX`AAPL

`sym`  |`cond`| price
---------------------
`AAPL` |      | 95
`AAPL` |  `A` | 43
`KX`   |  `C` | 32

/ exec + by sym = returns a dictionary
/ sym in `KX`AAPL allows multi filters for 1 column (2 syms)
```

```q
/7. retrieve the distinct values from column c1

a: ( [] c1: 1 2 3 1 2; c2: `a`b`c`a`b)

c1 | c2
--------
1  |  a
2  |  b
3  |  c
1  |  a
2  |  b

exec distinct c1 from a
1 2 3

/ returns only distinct values in column c1
/ exec on a column returns a list
```

```q
/8. retrieve the distinct values from column c1 and c2

exec distinct c1, distinct c2 from a

`key` | value
--------------
`c1`  | 1 2 3
`c2`  | `a`b`c

/ exec allows distinct on multiple columns
/ return a dictionary
```

### Select vs Exec

```q
cnc: ([] city:`toronto`london`ny`vancouver; country:`canada`england`usa`canada)

city     | country
-------------------
toronto  | canada
london   | england
ny       | usa
vancouver| canada
```

```q
exec city, distinct country from cnc

key    | value
-----------------------------------
city   | toronto london ny vancouver
country| canada england usa


/ exec on multiple columns returns a dictionary
/ more flexible in terms of structure
```

```q
select city, distinct country from cnc

/ error because select expects the columns to have the same length
/ select always returns a table
```

<a name="update_statement"></a>
### 🔵 19.13) Update
```q
/ updates a pre-existing column
/ if column doesnt exist, gets added to end of column list
/ original table unaffected unless the data is persisted by using backtick
```

```q
\ load trades.q script

/1. update all prices in table to 10

update price: 10.0 from trade
```

```q
/2. update every price of C to 10

update price:10.0 from trade where sym=`C

date       | time         | sym | price| size  | cond
-----------------------------------------------------
2021.10.30 | 09:30:02.553 | C   | 10   | 63500 | B   
```

```q
/3. update all prices of AAPL and GOOG to 10

update price:10.0 from trade where sym in `AAPL`GOOG

date       | time         | sym  | price| size  | cond
-----------------------------------------------------
2021.10.30 | 09:30:02.553 | C    | 10   | 63500 | B   
2021.10.30 | 09:30:02.701 | MSFT | 10   | 1700  | B   
2021.10.30 | 09:30:02.743 | RBS  | 10   | 80700 | C  

/ this will update prices to 10 for AAPL and GOOG 
/ the where clause updates only the filtered records
```

```q
/4. add new column vol, which is price x size for AAPL and GOOG

update vol:price*size from trade where sym in `AAPL`GOOG

date       | time         | sym  | price | size  | cond | vol          
------------------------------------------------------------------
2022.03.22 | 17:07:26.062 | GOOG | 109.9 | 99900 |   A  | 1098012
2022.03.24 | 11:13:08.106 | GOOG | 109.9 | 99700 |      | 1096486
2022.03.21 | 14:10:45.998 | GOOG | 109.7 | 99800 |   C  | 1094924
2022.03.20 | 13:55:32.398 | AAPL | 109.4 | 99900 |   A  | 1093780 
2022.03.23 | 11:35:12.474 | GOOG | 109.9 | 99500 |   B  | 1093587
```

```q
/5. updates prices for AAPL and GOOG to average price, grouped by sym 

update price:avg price by sym from trade where sym in `AAPL`GOOG

```

### UPDATE Problem Set 2

```q
/1. randomly select 100 rows from trade, call this tt

tt:100?trade

date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |422| B
2021.03.01 | 15:09:01| JPM | 74  |412| C
```

```q
/2. update all cond to "D"

update cond: "D" from tt

date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |422 | D
2021.03.01 | 15:09:01| JPM | 74  |412 | D
```

```q
/3. divide all size values by 100

update size%100 from tt

date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |42.2| D
2021.03.01 | 15:09:01| JPM | 74  |41.2| D
2021.03.01 | 15:09:01| UBS | 41  |31.2| D

/ can perform function on entire column. size divided by 100
```

```q
/4. add a new column to tt called advice and populate with sell

update advice:`sell from tt

date       |  time   | sym |price|size|cond|advice
---------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|D   | sell
2021.03.01 | 15:09:01| JPM |  74 |41.2|D   | sell
2021.03.01 | 15:09:01| UBS |  41 |31.2|D   | sell

/ if you update a column that doesnt exist, it will add the column
/ notice it has to be backtick sell
```

```q
/5. update advice to buy if price less than 70

update advice: `buy from tt where price < 70

date       |  time   | sym |price|size|cond|advice
---------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  D | 
2021.03.01 | 15:09:01| JPM |  74 |41.2|  D | 
2021.03.01 | 15:09:01| UBS |  41 |31.2|  D | buy

/ if price less than 70, advice becomes buy
/ if not, then null value returned
```

```q
/6. add new column maxprice populated with max prices by sym

update maxprice: max price by sym from tt

date       |   time  | sym |price|size|cond|maxprice
----------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  D | 104
2021.03.01 | 15:09:01| JPM |  74 |41.2|  D | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  D | 91

/ since maxprice doesnt exist, adds new column to end
/ by sym = groups by sym
```

<a name="delete_columns"></a>
### 🔵 19.14) Delete Columns

```q
/ DELETE function cannot have BY or WHERE clause!!

/ using our old tt table:

date       |   time  | sym |price|size|cond|maxprice
----------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  D | 104
2021.03.01 | 15:09:01| JPM |  74 |41.2|  D | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  D | 91
```

```q
/1. delete maxprice from tt

date       |   time  | sym |price|size|cond
--------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2| D 
2021.03.01 | 15:09:01| JPM |  74 |41.2| D 
2021.03.01 | 15:09:01| UBS |  41 |31.2| D 

/ deleted the maxprice column
```

```q
/2. delete the date and time columns from tt

sym |price|size|cond
--------------------
BAC |  70 |42.2| D 
JPM |  74 |41.2| D 
UBS |  41 |31.2| D 

/ deletes multiple columns from the table
```

```q
/3. What happens if you use delete + where clause filter?

delete price from trade where sym=`BAC
error

/ delete cannot contain where or by clauses!
```

<a name="delete_rows"></a>
### 🔵 19.15) Delete Rows

```q
/ tt = table of 100 random rows from trade

tt
date       |  time   | sym |price|size| cond| maxprice
------------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  A  | 104
2021.03.01 | 15:09:01| JPM |  74 |41.2|  B  | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  C  | 91

delete from tt where cond="A"

date       |  time   | sym |price|size| cond| maxprice
------------------------------------------------------
2021.03.01 | 15:09:01| JPM |  74 |41.2|  B  | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  C  | 91

/ since you are adding a WHERE clause, delete will remove the entire row 
/ WHERE cond = A
```
```q
delete from tt

/ deletes all rows
```

<a name="sort_asc_desc"></a>
### 🔵 19.16) Sort Columns Ascending / Descending 

```q
/ 3 ways to sort columns in a table via QSQL:

/ 1. xasc
/ 2. xdesc
/ 3. [> col_nam]
```

```q
/ load trades.q script

/ 1. sort by xasc

`sym`price xasc trade

date       |time     |sym|price|size | cond
--------------------------------------------
2021.01.01 | 15:10:01| A | 70  | 42.2| D
2021.03.01 | 15:09:01| B | 73  | 41.2| E
2021.03.01 | 15:09:01| C | 79  | 31.2| F

/ first sorts ascending by sym, then by price
```

```q
/ 2. sort by xdesc

`sym`price xdesc trade

date       | time    |sym|price| size| cond
--------------------------------------------
2021.01.01 | 15:10:01| C | 79  | 42.2| D
2021.03.01 | 15:09:01| B | 73  | 41.2| E
2021.03.01 | 15:09:01| A | 70  | 31.2| F

/ first sorts descending by sym, then by price
```

```q
/3. sort by [< column_name]

select [<sym] from trade

date       time         sym price    size  cond
-----------------------------------------------
2022.03.22 09:30:02.758 A   100.35   50300 B   
2022.03.22 09:30:17.997 A   57.81544 65600 C   
2022.03.22 09:30:21.507 A   97.85913 51800 B 

/ sorts the sym column in descending order
```

<a name="rename_reorder_columns"></a>
### 🔵 19.17) Renaming / Reordering Columns

```q
`new1`new2 xcol tt

new1       |new2     |sym|price| size| cond
--------------------------------------------
2021.01.01 | 15:10:01| C | 79  | 42.2| D
2021.03.01 | 15:09:01| B | 73  | 41.2| E
2021.03.01 | 15:09:01| A | 70  | 31.2| F

/ renames first 2 columns to new1 and new 2
```

```q
`cond`size xcols tt

cond|size| date       |time     |sym| price
--------------------------------------------
D   | 79 | 2021.01.01 | 15:10:01| C | 42.2
E   | 73 | 2021.03.01 | 15:09:01| B | 41.2
F   | 70 | 2021.03.01 | 15:09:01| A | 31.2

/ reorders columns cond and size to beginning
```

```q
`sym xgroup tt

sym   | date
------------------
`BAC` | 2021.01.01
`RBS` | 2021.01.23

/ group by column sym
```

```q
`date`sym xgroup tt

date         | sym   | time
---------------------------
`2021.01.01` | `BAC` | 1:12
`2021.01.02` | `JPM` | 1:45

/ group and key by 2 columns (date and sym)
```

```q
`date`sym xkey tt

date         | sym   | time | price | size | cond
--------------------------------------------------
`2021.01.01` | `BAC` | 1:12 | 83    | 834  | B
`2021.01.02` | `JPM` | 1:45 | 34    | 342  | A

/ make date and sym key columns
```

<a name="fby_sql"></a>
### 🔵 19.18) Filter by fby

```q
/ fby aggregates values from one list based on group defined in another
/ (aggr;d) fby g
/ aggr = aggregate function = max, min, sums, etc.
/ d = column name
/ g = another column name
/ fby goes at the END of your QSQL statement
```

### Example fby aggregations

```q
(sum;price) fby sym
(sums;price) fby sym
(max;price) fby sym
(last;price) fby sym
(first;price) fby sym
(max;price) fby sym
(avg;price) fby sym


/ select from trade where price = (max;price) fby sym 
/ fby goes at the END
/ fby goes after where
```
### Functions on fby

```q
price = (max;price) fby sym
price < (last;price) fby sym
price > (avgs;price) fby sym
price > (mavg[10];price) fby sym / moving avg 10 of price by sym
```

### fby on 2 lists 

```q
city:`NY`NY`LA`SF`LA`SF`NY
temp:32 31 75 69 70 68 12

/ 1. retrieve the lowest temperature by city

(min;temp) fby city
12 12 70 68 12

/ this calculates the min temp for every city (12 for NYC)
/ min = agg function
/ temp = column to agg
/ city = what you are filtering by
```

### fby on a table

```q
/ 1. find the max price per symbol

/ load trades.q script

select from trade where price=(max;price) fby sym

time       |sym  |src| price | size
-----------------------------------
2019-03-11 |GOOG | L | 36.01 | 1427
2019-03-11 |GOOG | O | 36.01 | 708
2019-03-11 |MSFT | N | 35.5  | 7810

/ notice there are 2 GOOG (both same "max" price)
/ you can add another fby filter for time
```

```q
/ 2. find the latest max price by sym

select from t where price=(max;price) fby sym, time=(max;time) fby sym

time      |sym  |src| price | size
-----------------------------------
2019-03-11|GOOG	| O | 36.01 | 708
2019-03-11|MSFT | N | 35.01 | 7810

/ first filtered max price by sym
/ then filtered max time by sym
/ can do multiple fby filters
```

### fby Example 3

```q
/ 1. find the highest price on 2021.10.31

select from trade where date=2021.10.31, price=max price

/ you are looking for the SINGLE highest price on date
/ filter by date, then the max price from this date
/ don't need fby since you're not aggregating anything
```

```q
/ 2. find the max price by sym on this 2021.10.31

select from trade where date=2021.10.31, price=(max;price) fby sym

date       | time         | sym | price | size | cond
------------------------------------------------------
2021-11-26 | 10:17:09.373 | A	| 109.9	| 94300| C
2021-11-26 | 10:25:22.268 | MSFT| 109.9	| 49100| C
2021-11-26 | 11:49:11.143 | D	| 109.9 |  5600| A

/ since you need to find max price BY sym (aggr by sym)
/ you need to use fby function
/ first filters by date, then finds max price aggr by sym

/ if you did this instead:

select max price by sym from trade where date = 2021.11.26

sym  | price
-------------
A    | 109.9
AA   | 113.2
AAPL | 339.1

/ this will ONLY return the sym + max price column
```

fby 2 aggregators

```q
/ 3. find the max price by sym AND cond on 2021.10.31

select from trade where date=2021.10.31, price=(max;price) fby ( [] sym; cond)

/ aggregate by more than one field using a table
/ filter by date, then max price by sym AND cond
```

### fby Example 4: VWAP

```q
/ compare each price to its vwap price

select from trade where date=2021.10.31, price>({x[`size] wavg x`price}; ([]size;price)) fby sym

/ vwap = volume weighted avg price, so need to use wavg function
/ syntax = x wavg y
/ for every x (row), find the wavg for each size/price
/ fby sym
```

<a name="xgroup_sql"></a>
### 🔵 19.19) xgroup

```q
/ load trade.q script

/ 1. group the trade table by the sym column

`sym xgroup trade

sym | date
----| -----
C   | 2021.10.19... 
MSFT| 2021.10.19... 
RBS | 2021.10.19...

/ group by column `sym

/ to flatten this out, use ungroup

ungroup select time by sym from trade
```

<a name="differ_sql"></a>
### 🔵 19.20) Differ

```q
/ boolean list indicating if consecutive pairs are different
/ true 1b = if consecutive elements are different
/ false ob = consecutive elements are the same
/ will always return TRUE for first element

differ 1 1 1 2 2 3
100101b
```

```q
/ can be used to see if trade price has changed

update change:differ price from trade

date       time         sym  price    size  cond change
-------------------------------------------------------
2021.10.19 09:30:02.553 C    107.2018 63500 B    1     
2021.10.19 09:30:02.701 MSFT 96.87488 1700  B    1     
2021.10.19 09:30:02.743 RBS  97.11338 80700 C    1     

/ or, to select those trades who's price has changed

select from trade where differ price

date       time         sym  price    size  cond
------------------------------------------------
2021.10.19 09:30:02.553 C    107.2018 63500 B   
2021.10.19 09:30:02.701 MSFT 96.87488 1700  B   
2021.10.19 09:30:02.743 RBS  97.11338 80700 C   
```

<a name="deltas_sql"></a>
### 🔵 19.20) Deltas

```q
/ returns the difference between consecutive list elements

deltas 1 3 2 4 
1 2 -1 2

/ can be used to view price changes between trades

update change:deltas price from trade

date       time         sym  price    size  cond change    
--------------------------------------------------------
2021.10.19 09:30:02.553 C    107.2018 63500 B    107.201  
2021.10.19 09:30:02.701 MSFT 96.87488 1700  B    -10.326 
2021.10.19 09:30:02.743 RBS  97.11338 80700 C      0.238

/ or, to select those trades who's price has increased

select from trade where (deltas price)> 0

date       time         sym    price    size  cond 
--------------------------------------------------
2021-10-19 09:30:02.553	C      107.2    63500  B
2021-10-19 09:30:02.743	RBS     97.1    80700  C
2021-10-19 09:30:02.758	A      100.3    50300  B
```

<a name="nextprev_sql"></a>
### 🔵 19.22) Next/Prev

```q
/ next - moves each element of list one space to left
/ prev - moves each element of list one space to right
/ can be used to find the duration between trades

update duration:time - prev time from trade

date       time         sym  price    size  cond duration    
-------------------------------------------------------------
2021.10.19 09:30:02.701 MSFT 96.87488 1700  B    00:00:00.148
2021.10.19 09:30:02.743 RBS  97.11338 80700 C    00:00:00.042
2021.10.19 09:30:02.758 A    100.35   50300 B    00:00:00.015
```

```q
/ xprev - moves each element of list n spaces to the right

3 xprev 1 2 3 4 5 6
0N 0N 0N 1 2 3

/ note - no such thing as xnext. instead, use negative xprev

-3 xprev 1 2 3 4 5 6
4 5 6 0N 0N 0N
```

<a name="carrot_sql"></a>
### 🔵 19.23) Coalescing ^

```q
/ ^ replaces nulls on right with atom on left
/ has to be of compatible type
/ right item prevails over left item except when right item is null

3 ^ 1 2 0N 4 5 0N
1 2 3 4 5 3
```

```q
/ can also be used as index replacement

1 2 3 4 ^ 5 0N 6 0N
5 2 6 4 

/ the first 0N is replaced with 2
/ the 2nd 0N is replaced with 4
```

<a name="iasc_sql"></a>
### 🔵 19.24) iasc/idesc (advanced)

```q
/ iasc - returns indices needed to sort a list in ascending order
/ idesc - returns indices needed to sort a list in descending order 

iasc 1 2 5 4
0 1 3 2

idesc 1 2 5 4
2 3 1 0
```
```q
/ case study

m:(1 2 3 4; 6 4 5; 2 6 3 7 5; 2 5)
1 2 3 4
6 4 5
2 6 3 7 5
2 5

/ m is a nested list

count each m
4 3 5 2

/ tells you how much elements in each nested list

m iasc count each m
2 5
6 4 5
1 2 3 4
2 6 3 7 5

/ order m by number of elements in each sublist
```


<a name="rank_sql"></a>
### 🔵 19.25) rank / xrank

```q
/ rank returns the position of each element of a list would appear if it were sorted in ascending order
/ same as iasc iasc x

rank 2 7 3 2 5
0 4 2 1 3

/ 0 index pos = 2
/ 4th index pos = 7
/ 2nd index pos = 3
/ 1st index pos = 2
/ 3rd index pos = 5
```

```q
/ xrank partitions list into buckets based on values

2 xrank 1 2 3 4 5 6
0 0 0 1 1 1

3 xrank 1 2 3 4 5 6
0 0 1 1 2 2 
```

```q
t:([] val: 8?20; name: (8?`MSFT`ORCL`CSCO))

val name
--------
12  MSFT
8   ORCL
13  CSCO
16  MSFT
15  ORCL
16  CSCO
2   MSFT
4   ORCL

select Min: min val, Max:max val, Count: count i by bucket: 4 xrank val from t

bucket Min Max Count
--------------------
0      2   4    2
1      8  12    2
2     13  15    2
3     16  16    2

```


<a name="qsql_problem_set"></a>
## 🔴 20. qSQL Problem Set
[Top](#top)

**🔵 QSQL Problem Set 1 (easy)**

```q
/ load the trades.q script
```

```q
/ 1. Extract from trade table, trades for MS greater than 1,000 in size

select from trade where sym=`MS, size >1000

dt         | sym | price| size
------------------------------
2021.01.01 |  MS |  225 | 200
2021.01.01 |  MS |  234 | 400

/ multiple WHERE expressions separated by commas
/ sym has to be back tick MS
```

```q
/ 2. from the trade table, find the total size of all trades and the average price paid per sym

select total: sum size, avg price by sym from trade

`sym`  | total | price
-----------------------
`AAPL` |  320  | 1015
`C`    |  310  | 100
`MS`   |  740  | 234

/ "price paid per sym" = we need to set sym as a keyed colummn (by sym)
/ total: renames column, sum size = sums sizes together
/ avg price = retains the price column header, just averages prices
```

```q
/ 3. From the trade table, find the trade that was largest size for each sym

select from trade where size=(max;size) fby sym

date      | time         | sym | price | size|cond
----------------------------------------------------
2021-05-30| 09:30:21.256 | B   |100.04 |99900|	 
2021-05-30| 09:31:20.975 | AA  |67.30  |99900|	C
2021-05-30| 09:43:47.816 | GOOG|72.42  |99900|	A
2021-05-30| 09:46:44.690 | F   |73.22  |99900|	B

/ uses fby to perform filters on aggregate queries
/ fby has to go at the END of your query
```

alternative syntax:

```q
select from (update mx:max size by sym from trade) where size = mx

date      |     time     | sym | price | size |cond|  mx
-----------------------------------------------------------
2021-05-30| 09:30:21.256 | B   | 100.04| 99900|    | 99900
2021-05-30| 09:31:20.975 | AA  | 67.30 | 99900|	 C | 99900
2021-05-30| 09:43:47.816 | GOOG| 72.42 | 99900|	 A | 99900

/ add new column mx which is the max size by sym
/ where size = filter size to max size
/ this is using a nested query to filter only the max size for their sym
```

```q
/ 4. From the trade table, select the latest trade for each sym, and include all details

select from trade where time=(last;time) fby sym

date       | time         | sym  | price | size  | cond
--------------------------------------------------------
2022-03-26 | 17:29:57.306 | A	 | 87.5	 | 49100 |  B
2022-03-26 | 17:29:58.789 | AA	 | 68.0  | 88100 |  A
2022-03-26 | 17:29:58.262 | AAPL | 76.1	 | 22500 |  A
```

alternative syntax:

```q
/ altho this one is less ideal:

select last date, last price, last size by sym from trade

sym |   date    | price | size
--------------------------------
`A` | 2021-06-03| 87.54 | 49100
`AA`| 2021-06-03| 68.09 | 88100
```

```q
/ 5. Find all trades that have sym GOOG

select from trade where sym=`GOOG

sym |   date    | price | size  | cond
---------------------------------------
GOOG| 2021-06-03| 87.54 | 49100 |  B
GOOG| 2021-06-03| 87.54 | 49100 |  C
```

```q
/ 6. Find all trades that have sym GOOG or RBS or A

select from trade where sym in `GOOG`RBS`A

sym |   date    | price | size  | cond
---------------------------------------
GOOG| 2021-06-03| 87.54 | 49100 |  B
RBS | 2021-06-03| 87.54 | 49100 |  C
A   | 2021-06-03| 87.54 | 49100 |  C
```

```q
/ 7. Find all trades for google that had a price between 70 and 80

select from trade where sym=`GOOG, price within 70 80

sym |   date    | price | size  | cond
--------------------------------------
GOOG| 2021-06-03|   72  | 49100 |  B
GOOG| 2021-06-03|   75  | 49100 |  C
GOOG| 2021-06-03|   78  | 49100 |  C
```

```q
/ 8. Count the number of trades and total size of trades per hour for sym RBS

select num_trades:count i, total_size: sum size by sym, 1 xbar time.hh from trade where sym=`RBS

`sym` | `hh` | num_trades |	total_size
-----------------------------------
`RBS` |  `9` |     3186   |	159063500
`RBS` | `10` |     6544   |	321195100
`RBS` | `11` |     6280   |	315284200
`RBS` | `12` |     6141   |	306898200
`RBS` | `13` |     6086   |	305154900

/ you need to group BY SYM, since you're aggregating
/ the total num trades + total size
/ use count i = count virtual column
/ notice xbar comes AFTER the by sym, but BEFORE the where
/ both sym + xbar are aggregators
/ so both columns are keyed
```

```q
/ notice what happens if instead of group BY SYM
/ you group BY XBAR

select num_trades:count i, total_size: sum size by 1 xbar time.hh from trade where sym=`RBS

`hh` | num_trades | total_size
----------------------------
`9`  |    3186   | 159063500
`10` |    6544   | 321195100
`11` |    6280   | 315284200
`12` |    6141   | 306898200
`13` |    6086   | 305154900

/ the sym column is removed
/ but the underlying answer is still correct
```

```q
/ 9. Select the number of trades and total size of trades every 30 mins for the sym RBS

select num_trades: count i, tot_size:sum size by sym, 30 xbar time.minute from trade where sym=`RBS

`sym` | `minute` | num_trades | tot_size
---------------------------------------
`RBS` |  `09:30` |    3186    | 159063500
`RBS` |  `10:00` |    3271    | 162197000
`RBS` |  `10:30` |    3273    | 158998100
`RBS` |  `11:00` |    3110    | 157994800
`RBS` |  `11:30` |    3170    | 157289400
`RBS` |  `12:00` |    3120    | 156311100

/ 30 xbar time.minute = groups minutes by 30
```

```q
/ 10. Find all trades for A where price is cheaper than the average for that day

select by date from trade where sym=`A, price < avg price

date       |     time	  | sym	| price | size | cond
------------------------------------------------------
2022-03-22 | 17:29:55.778 |  A	| 53.5	| 79400	| C
2022-03-23 | 17:29:46.639 |  A	| 66.5	| 97900	| C
2022-03-24 | 17:29:58.310 |  A	| 73.9	| 30300	| C
2022-03-25 | 17:29:58.323 |  A	| 58.3	| 41000	| B
2022-03-26 | 17:29:57.072 |  A  | 60.0	| 88800	| 
```

**🔵 QSQL Problem Set 2 (easy)**

```q
/1. sort [grocer column] from [sales] by descending

sales: ([] fruit:`apple`orange`pear`banana; grocer: `mark`mark`allen`tom; price: 1 2 3 4; quantity: 10 20 30 40)

fruit   grocer  price   quantity
--------------------------------
apple	mark	1	10
orange	mark	2	20
pear	allen	3	30
banana	tom	4	40

select [>grocer] from sales

fruit   grocer  price   quantity
--------------------------------
banana	tom	4	40
apple	mark	1	10
orange	mark	2	20
pear	allen	3	30

/ [grocer column] is now sorted by descending
```

```q
/2. retrieve banana and pear, along with their prices

select fruit, price from sales where fruit in `banana`pear

fruit  | price
--------------
pear   | 3
banana | 4

/ use the in keyword to filter values within a column
```

**🔵 QSQL Problem Set 3 (Easy)**

```q
/ load trades.q script
```

```q
/ 1. select the last 3 rows of trade table

select [-3] from trade

date       | time	  | sym  | price | size | cond
-------------------------------------------------------
2022-03-19 | 09:30:02.553 | C	 | 107.2 |63500 | B
2022-03-19 | 09:30:02.701 | MSFT | 96.8	 | 1700	| B
2022-03-19 | 09:30:02.743 | RBS	 | 97.1	 |80700	| C
```

```q
/ 2. retrieve max price on 2021.05.29 for sym A

select max price from trade where date=2021.05.29, sym=`A

price
------
109.99
```

```q
/ 3. count how many trades have condition A

count select from trade where cond="A"
211597

/ the count function tallies the number of rows
/ from your query
```

```q
/ 4. retrieve all trades from today, aggregated by sym

select by sym from trade where date=.z.d

sym  |  date      |   time       | price | size | cond
-------------------------------------------------------
A    | 2021-06-02 | 17:29:57.306 | 87.54 | 49100 |  B
AA   | 2021-06-02 | 17:29:58.789 | 68.09 | 88100 |  A
AAPL | 2021-06-02 | 17:29:58.262 | 76.18 | 22500 |  A

/ the BY CLAUSE is used for aggregations
/ groups all trades by sym and sets column as key
```

```q
/ 5. retrieve prices, keyed by TODAY, where AAPL's price is less than the avg price

select price by date from trade where sym=`AAPL, price < avg price, date=.z.d

date       | price
-------------------------------------
2022.03.23 | 62.4 84.4 29.2 49.4 28.2
```

```q
/ 6. retrieve price divide by max price, keyed by today, where the price is less than the avg price

select price by date from trade where sym=`AAPL, price < avg price, date=.z.d

date       | price
--------------------------------
2022.03.23 | 0.77 0.73 0.99 0.94
```

```q
/ 7. retrieve data for AAPL and RBS from trade

select from trade where sym in `AAPL`RBS

date      | time         | sym | price  | size  | cond
------------------------------------------------------
2021-05-30| 09:30:02.743 | RBS | 97.113	| 80700 | C
2021-05-30| 09:30:03.025 | AAPL| 78.66  | 19000	| A

/ in function checks if every LHS argument occurs anywhere in RHS argument (AAPL or RBS)
/ a faster way of checking "or" arguments
```

```q
/ 8. retrieve trades for RBS within 95 and 100 and between 11:30 - 12:00

select from trade where sym=`RBS, price within 95 100, time within 11:30 12:00

date      | time          |sym   | price  | size | cond
-------------------------------------------------------
2021-05-30| 11:40:02.743 | RBS   | 97.113 | 80700 | C
2021-05-30| 11:44:03.025 | AAPL  | 98.66  | 19000 | A

/ two within filters, price and time
```

**🔵 QSQL Problem Set 4 (easy)**

```q
/ 1. retrieve the total size and total number of trades for each sym and each $1 price buckets

select sum size, cnt:count i by sym, 1 xbar price from trade

`sym` |`price`|   size   | cnt
-----------------------------
 `A`  |  `50` | 44191500 | 838
 `A`  |  `51` | 42318700 | 842
 `A`  |  `52` | 41432200 | 832
 `A`  |  `53` | 30434493 | 832

/ groups the data by sym and 1 dollar price buckets
/ ie, how many total trades were executed by sym for that price bucket
```

```q
/ 2. find the max price by sym for each 45 min window

select max price by sym, 45 xbar time.minute from trade

sym |minute | price
----------------------
 A  |09:00  | 109.94
 A  |09:45  | 109.99
 A  |10:30  | 109.96

/ group by sym, set xbar as 45 minute time buckets
```

```q
/ 3. return a list of all prices for AAPL for today

exec price from trade where date=.z.d, sym=`AAPL
62 59 13

/ exec single column = single list returned
```

```q
/ 4. return column of values for AAPL on today

select price from trade where date=.z.d, sym=`AAPL

price
------
62
59
13

/ select = single column returned
```

```q
/ 5. return ALL prices of AAPL from today as a dictionary

exec price by sym from trade where date=.z.d, sym=`AAPL
AAPL | 62 59 13

/ exec + by sym
/ groups the data by sym
/ and returns a dictionary
```

```q
/ 6. retrieve first price, cond from today for KX and AAPL as a dictionary

exec first price by sym, cond from trade where date=.z.d, sym in `KX`AAPL

`sym`  |`cond`| price
---------------------
`AAPL` |      | 95
`AAPL` |  `A` | 43
`KX`   |  `C` | 32

/ exec + by sym = returns a dictionary
/ sym in `KX`AAPL allows multi filters for 1 column (2 syms)
```

**🔵 QSQL Problem Set 5 (easy)**

```q
/ 1. update all prices of AAPL and GOOG to 10

update price:10.0 from trade where sym in `AAPL`GOOG

date       | time         | sym  | price| size  | cond
-----------------------------------------------------
2021.10.30 | 09:30:02.553 | C    | 10   | 63500 | B   
2021.10.30 | 09:30:02.701 | MSFT | 10   | 1700  | B   
2021.10.30 | 09:30:02.743 | RBS  | 10   | 80700 | C  

/ this will update prices to 10 for AAPL and GOOG 
/ the where clause updates only the filtered records
```

```q
/ 2. update all cond to "D"

update cond: "D" from tt

date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |422 | D
2021.03.01 | 15:09:01| JPM | 74  |412 | D
```

```q
/ 3. divide all size values by 100

update size%100 from tt

date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |42.2| D
2021.03.01 | 15:09:01| JPM | 74  |41.2| D
2021.03.01 | 15:09:01| UBS | 41  |31.2| D

/ can perform function on entire column. size divided by 100
```

```q
/ 4. add a new column to tt called advice and populate with sell

update advice:`sell from tt

date       |  time   | sym |price|size|cond|advice
---------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|D   | sell
2021.03.01 | 15:09:01| JPM |  74 |41.2|D   | sell
2021.03.01 | 15:09:01| UBS |  41 |31.2|D   | sell

/ if you update a column that doesnt exist, it will add the column
/ notice it has to be backtick sell
```

```q
/ 5. update advice to buy if price less than 70

update advice: `buy from tt where price < 70

date       |  time   | sym |price|size|cond|advice
---------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  D | 
2021.03.01 | 15:09:01| JPM |  74 |41.2|  D | 
2021.03.01 | 15:09:01| UBS |  41 |31.2|  D | buy

/ if price less than 70, advice becomes buy
/ if not, then null value returned
```

```q
/ 6. add new column maxprice populated with max prices by sym

update maxprice: max price by sym from tt

date       |   time  | sym |price|size|cond|maxprice
----------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  D | 104
2021.03.01 | 15:09:01| JPM |  74 |41.2|  D | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  D | 91

/ since maxprice doesnt exist, adds new column to end
/ by sym = groups by sym
```

```q
/ 7. remove the maxprice column from trade

delete maxprice from trade

date       |   time  | sym |price|size|cond
--------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2| D 
2021.03.01 | 15:09:01| JPM |  74 |41.2| D 
2021.03.01 | 15:09:01| UBS |  41 |31.2| D 
```

```q
/ 8. remove any trades where condition is A

delete from trade where cond="A"

date       |  time   | sym |price|size| cond| maxprice
------------------------------------------------------
2021.03.01 | 15:09:01| JPM |  74 |41.2|  B  | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  C  | 91

/ since you are adding a WHERE clause, delete will remove the entire row 
/ WHERE cond = A
```

```q
/ 9. find the highest price on 2021.10.31

select from trade where date=2021.10.31, price=max price

/ you are looking for the SINGLE highest price on date
/ filter by date, then the max price from this date
/ don't need fby since you're not aggregating anything
```

```q
/ 10. find the max price by sym on 2021.10.31

select from trade where date=2021.10.31, price=(max;price) fby sym

date       | time         | sym | price | size | cond
------------------------------------------------------
2021-11-26 | 10:17:09.373 | A	| 109.9	| 94300| C
2021-11-26 | 10:25:22.268 | MSFT| 109.9	| 49100| C
2021-11-26 | 11:49:11.143 | D	| 109.9 |  5600| A

/ since you need to find max price BY sym (aggr by sym)
/ you need to use fby function
/ first filters by date, then finds max price aggr by sym

/ if you did this instead:

select max price by sym from trade where date = 2021.11.26

sym  | price
-------------
A    | 109.9
AA   | 113.2
AAPL | 339.1

/ this will ONLY return the sym + max price column
```

```q
/ 11. find the max price by sym AND cond on 2021.10.31

select from trade where date=2021.10.31, price=(max;price) fby ( [] sym; cond)

/ aggregate by more than one field using a table
/ filter by date, then max price by sym AND cond
```

**🔵 QSQL Problem Set 6 (Medium)**

```q
/ load trades.q script
/ WHERE + table filter case study
```

```q
/ 1. from the trade table, retrieve the following trades:

/ IBM from cond A
/ CSCO from cond A or B
/ MSFT from cond C 
/ date = 2021.11.17
```

```q
/ first, check the meta of the trade table

meta trade

c    |t|f|a
------------
date |d| |s
time |t| |		
sym  |s| |		
price|f| | 		
size |i| |		
cond |c| |		

/ reveals correct datatype to retrieve properly
/ sym = sym 
/ cond = char
```

```q
/ since you have multiple parameters, 
/ it's easier to create a table of these parameters,
/ then use this table as part of your WHERE filter

/2. create new table, toget, with the target parameters

toget:( [] sym:`IBM`CSCO`CSCO`MSFT; cond:"AABC")

sym   cond
----------
IBM    A
CSCO   A
CSCO   B
MSFT   C

/ notice you had to dupe the CSCO
/ since its parameter is A or B
```

```q
/3. Use QSQL to filter the table of parameters

select from trade where date=2021.11.17, ( [] sym; cond) in toget

date       sym  price size cond
-------------------------------
2021-10-30 MSFT	60.66 48700 C
2021-10-30 IBM	59.00 28300 A
2021-10-30 MSFT	54.57 23700 C
2021-10-30 IBM	89.19 86600 A
2021-10-30 IBM	84.13 46600 A

/ first filters by date 2021.11.17
/ then filters by the values in the [sym] and [cond] columns
/ from the [toget] table
```

**🔵 QSQL Problem Set 7 (Medium)**

```q
/ load trades.q script
/ WHERE + table filter case study 2
```

```q
results:( []name:`John`Paul`Rachel`Jane`Emma;gender:"MMFFF";grade:"ABBAC")

name  |gender|grade
--------------------
John  |   M  | 	A
Paul  |   M  |	B
Rachel|   F  |	B
Jane  |   F  |	A
Emma  |   F  | 	C
```

```q
/ 1. from the results table, extract all the following:

/ gender - male and grade - A
/ gender - female and grade - B
/ gender - female and grade - A
```

```q
/ 1a. show the syntax individually for each query

select from results where gender="M", grade="A"
select from results where gender="F", grade="B"
select from results where gender="F", grade="A"

name  |gender|grade
--------------------
John  |   M  | 	A

name  |gender|grade
--------------------
Rachel|   F  |	B

name  |gender|grade
--------------------
Jane  |   F  |	A
```

```q
/ 2. run the same query, instead running a table filter
/ (which probably cleaner outcome)

select from results where ( [] gender; grade) in ( [] gender:"MFF"; grade:"ABA")

name  |gender|grade
--------------------
John  |   M  | 	A
Rachel|   F  |	B
Jane  |   F  |	A

/ so instead of "creating" a separate table
/ you construct the table of possible outcomes in place
/ then you simply filter using table with column names = [gender]; [grade]
```

**🔵 QSQL Problem Set 8 (Medium)**

```q
/ load the trades.q script
/ bin function case study
```

```q
/ 1. Create a function that accepts argument x as a list
/ and returns "buckets" of aggregation for small, medium, large trades
/ small < 1000
/ medium = 1000-8999
/ large > 9000

f: {`small`medium`large 0 1000 9000 bin x}
f [500 1000 100000]
`small`medium`large
```

```q
/ 2. use this f function to retrieve the total number of trades
/ grouped by their size bucket (small, medium, large) for each sym

select numtrades:count i by sym, sizebucket:(f;size) fby sym from trade

sym | sizebucket | numtrades
-----------------------------
AA  |   large    | 45425
AA  |   medium   | 3986
AA  |   small    | 502
AAPL|   large    | 45621
AAPL|   medium   | 3974
AAPL|   small    | 511
BAC |   large    | 45551
BAC |   medium   | 3958
BAC |   small    | 3948

/ the f function takes in list of numbers,
/ and returns = small, medium, or large
/ so you need to add a new column (sizebucket)
/ for these outputs
/ utilizes the f function as an aggregator for fby
/ notice you're grouping the count i by sym
/ since this needs to match the agg fby sym
```

**🔵 QSQL Problem Set  (HARD)**

```q
/ load the trades.q script
/ tickdirection case study
```

```q
/1 lets say you want to check if the latest value was an uptick, downtick, or unch
/ can make use of the deltas + signum function

select from trade
update dir: signum deltas price from trade

sym| price|size |cond|dir
--------------------------
C  |  59  |18400|C   | 1  
F  |  104 |62600|    | 1  
IBM|  73  |77500|B   |-1 
A  |  63  |73000|B   |-1 

/ this will add a new column, dir, which will be +1, 0, or -1
/ deltas will calculate the change between subsequence elements
/ signum will tell you if the element is positive, negative, or 0
/ for example:

deltas 3 2 2 1 5
3 -1 0 -1 4

signum deltas prices
1 -1 0 -1 1
```

```q
/2 create function for signum deltas

tickdirection:{signum delta x}

/ should start from 0, indicating no movement for first element

tickdirection:{signum deltas [first x;x]}

/ use dyadic form each prior adverb

tickdir:{0i,1 _signum deltas x}

/ apparently this syntax works too ?

update dir: tickdirection price from trade

sym| price|size |cond|dir
--------------------------
C  |  59  |18400|C   | 1  
F  |  104 |62600|    | 1  
IBM|  73  |77500|B   |-1 
A  |  63  |73000|B   |-1 

/ same result as above
```

```q
/3 now lets say you want to group it by sym and see total size traded by direction (uptick, downtick, etc)

select sum size by sym, dir from update dir:tickdir price by sym from trades

sym|dir|size
-------------------
 A |-1 |1258345400
 A | 0 |7100
 A | 1 |1252317500

/ anything past the first from = table you created above
/ group by sym and dir (which you previously calculated)
/ but it looks funny as it has 2 froms. Can try to clean up

/ you cannot simply do this:

select sum size by sym, dir:signum deltas price by sym from trades

/ error, as tickdir is calculated on the price column as a whole
/ you cannot group by a column calculation on entire column
/ instead of splititng on sym first

/ so you have to use an fby instead

select sum size by sym, dir:(tickdir; price) fby sym from trades

sym|dir|size
-------------------
 A |-1 |1258345400
 A | 0 |7100
 A | 1 |1252317500
 
/ this will now work and returns same table as above
/ uses function tickdir as aggregator for signums from price column
/ the fby aggregates the tickdir from price column by sym
```

```q
/ find total size of trades where size > 10 tick moving average
/ 10 tick moving average requires a price calculation 
/ so you can't can't by a column (price) that is doing calculations
/ instead need to use fby

select sum size by sym, price > (mavg[10];price) fby sym from trade

 sym  |sym1|size
-------------------
 A    | -1 |1258345400
 AAPL |  0 |1237295400
 MSFT |  1 |1252317500
```

**🔵 QSQL Problem Set  (HARD)**

```q
/ Case Study: Pull the best bid from orderbook

table t:
t         bidPrices            bidSizes
------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  57 0 72 50 62 51
00:59:05  0.97 7.44 9.33 2.93  97 99 27 31
01:19:44  2.88 5.63 4.98 5.56  47 57 31 15 68 49
```

```q
/1 create new column bidIndex, which shows the index position in descending values (large to small)

update bidIndex:({idesc x} each bidPrices) from t

t         bidPrices            bidSizes           bidIndex
----------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  57 0 72 50 62      2 1 0 4 
00:59:05  0.97 7.44 9.33 2.93  97 99 27 31        2 1 4 0
01:19:44  2.88 5.63 4.98 5.56  47 57 31 15 68 49  1 4 3 0

/ from col bidPrices, shows index position of descending values
/ 2nd index position = 3rd value = 9.84 largest
```

```q
/2 now isolate only the largest value

update bidIndex:({first idesc x} each bidPrices) from t

t         bidPrices            bidSizes           bidIndex
----------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  57 0 72 50 62      2 
00:59:05  0.97 7.44 9.33 2.93  97 99 27 31        2
01:19:44  2.88 5.63 4.98 5.56  47 57 31 15 68 49  1

/ adding first = only retrieves first value 
/ largest bid since ordered by idesc
```

```q
/3 add a new column, bestBid, and retrieve the bestBid from the index position in bidIndex

update bestBid:bidPrices@'bidIndex from update bidIndex:({first idesc x} each bidPrices) from t

t         bidPrices            bidSizes     bidIndex   bestBid
--------------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  0 72 50 62    2          9.84 
00:59:05  0.97 7.44 9.33 2.93  23 99 27 31   2          9.33
01:19:44  2.88 5.63 4.98 5.56  57 31 15 49   1          5.63

/ bestbid = looks at bidIndex col, retrieves index position 2 from bidPrice col = 9.8
/ everything after from is what we calculated above as the bidIndex col
```

```q
/4 add new column, bestBidSize, and retrieve the largest bidsize based on the bidIndex column

update bestBidSize:bidSizes@'bidIndex from update bidIndex:({first idesc x} each bidPrices) from t

t         bidPrices            bidSizes     bidIndex   bestBidSize
------------------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  0 72 50 62    2          50 
00:59:05  0.97 7.44 9.33 2.93  23 99 27 31   2          27
01:19:44  2.88 5.63 4.98 5.56  57 31 15 49   1          31

/ bestBidSize = looks at bidIndex col, retrieves index position 2 from bidSizes col = 50
```
```q
/5 Now combine all 3 queries into single one:

update bestBid:bidPrices@'bidIndex, bestBidSize:bidSizes@'bidIndex from update bidIndex:({first idesc x}each bidPrices) from t

t         bidPrices            bidSizes     bidIndex   bestBid  bestBidSize
---------------------------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  0 72 50 62    2          9.84       50
00:59:05  0.97 7.44 9.33 2.93  23 99 27 31   2          9.33       27
01:19:44  2.88 5.63 4.98 5.56  57 31 15 49   1          5.63       31

/ useful to use index position to retrieve value in another column
/ lookup colum @`source column
/ you can have multiple update statements to add new columns
/ the bestBid and bestBidSize columns actually retrieve from a new column called bidIndex
```

<hr>

<a name="qsql_joins"></a>
## 🔴 21. qSQL Joins
[Top](#top)

```q
see also joins on tables
```

<a name="left_join"></a>
### 🔵 21.1 qSQL Left Join

```q
/ x lj y 

/ x = source table (can be key or unkeyed)
/ y = lookup table (t2 must be keyed)

/ for each row in source table, find match on keyed columns in lookup table
/ adds new columns to the end of original table
/ will always have same number of rows as original table
/ no match = nulls
/ column names must match and 2nd table must be keyed

trade table
x date        time         sym     price    size  
-------------------------------------------------
1|2021.06.03| 09:30:02.553| C    | 107.20 | 63500
2|2021.06.03| 09:30:02.701| MSFT | 96.87  | 1700
3|2021.06.03| 09:30:02.743| RBS  | 97.11  | 80700

stock table (keyed)
x `sym`   sector employees
-------------------------
1|`C`    |Tech  | 862      
2|`MSFT` |Tech  | 765      
3|`RBS`  |Tech  | 377      

trade lj stock

x date        time         sym    price     size cond  sector  employees
-------------------------------------------------------------------
1|2021.06.03| 09:30:02.553| C   | 107.2018| 63500| B |  Tech  | 862      
2|2021.06.03| 09:30:02.701| MSFT| 96.87488| 1700 | B |  Tech  | 765      
3|2021.06.03| 09:30:02.743| RBS | 97.11338| 80700| C |  Tech  | 377      

/ match on C, MSFT, RBS, adds on new columns sector + employees
/ will always be same number of rows as source table (3)
/ here the tables are joined on `sym as the key
```

<a name="plus_join"></a>
### 🔵 21.2 qSQL Plus Join 

```q
/ x pj y

/ y table has to be keyed
/ x table can be keyed or unkeyed
/ where there is a match on key across tables, values are added together 
/ other columns on original table remain unchanged
/ values have to be compatible with addition. for ex, if sym, will fail

stock table:
x `sym`  sector  employees
-------------------------
1|`C`    |Tech   |100      
2|`MSFT` |Tech   |100      
3|`RBS`  |Tech   |100      

trade table:
x `sym`  sector  employees
-------------------------
1|`C`    |Tech   |100      
2|`MSFT` |Tech   |-100      

stock pj trade

x `sym`  sector  employees
-------------------------
1|`C`    |Tech      |200      
2|`MSFT` |Tech      |0      
3|`RBS`  |Tech      |100    

/ from stock table, find the corresponding keyed sym in lookup table, add values together
/ if value doesnt exist (RBS), remain unchanged

```

<a name="inner_join"></a>
### 🔵 21.3 qSQL Inner Join 

```q
/ x ij y

/ y has to be keyed
/ x can be keyed or unkeyed
/ similar to left join, but only returns rows where matches occur
/ if match occurs in keyed table, column added on, or updated if already exists
/ non matches removed from new table (no nulls)

trade table:
x date       sym    price   size  
--------------------------------------
1|2021.06.03| C   | 107.2 | 63500
2|2021.06.03| MSFT| 96.8  | 1700
3|2021.06.03| UBS | 100.3 | 50300

stock table (keyed):
x `sym`  sector  employees
-------------------------
1|`C`    |Tech  | 100      
2|`MSFT` |Tech  | 100      

trade ij stock

x date        sym    price  size  sector employees
--------------------------------------------------
1|2021.06.03| C    | 107.2| 63500| Tech | 100
2|2021.06.03| MSFT | 96.8 |  1700| Tech | 100

/ C and MSFT match on syms (keyed)
/ adds on their corresponding values for sector and employees columns
/ removes row UBS since no match
```

<a name="union_join"></a>
### 🔵 21.4 qSQL Union Join 

```q
/ union join can be keyed or unkeyed!
/ adds ALL rows/columns together
/ allows tables with different columns to be joined
```
```q
/ unkeyed union join

/ unkey uj = return all rows + all columns
/ cols from 1 table but not the other are filled with nulls
/ even if values match, does NOT update. adds as new row.

t1
sym  | price | size | cond
--------------------------
GOOG | 91.43 | 5500 | B
IBM  | 105.8 | 23600|	 
MS   | 75.86 | 600  | 

t2
sym  | price | size  | cond
--------------------------
IBM  | 84.97 | 56900 | B
C    | 91.79 | 7800  | B
RBS  | 78.01 | 98700 | 

t1 uj t2

sym  | price | size  | cond
---------------------------
GOOG | 91.48 | 5500  | B
IBM  | 105.83| 23600 |	 
MS   | 75.86 | 600   |	 
IBM  | 84.97 | 56900 | B
C    | 91.79 | 7800  | B
RBS  | 78.01 | 98700 |	 

/ unkeyed uj = return all rows + all columns
/ cols from 1 table but not the other are filled with nulls
```
```q
/ keyed union join

/ right lookup table must be keyed (duh)
/ if match, rows from left table are updated with values from right table
/ if no match, null returned
/ useful when consolidating price buckets

trade table:
date       sym   price  size  
----------------------------
2021.06.03| C   | 107.2| 10
2021.06.03| MSFT|  96.8| 10
2021.06.03| UBS | 100.3| 10

stock table:
`sym`   sector  size  book
--------------------------
`FB`  |Tech   |100  | A      
`GOOG`|Tech   |100  | B

trade uj stock

date       `sym`  price  size book
----------------------------------
2021.06.03| C   | 107.2 | 10 | 
2021.06.03| MSFT| 96.8  | 10 |
2021.06.03| UBS | 100.3 | 10 |
          | FB  |       |100 | A
          | GOOG|       |100 | A

/ no key match for FB or GOOG, so appends new row
/ adds new column book; blank for existing, pulls in value from new
```
```q
/ union join + xbar example

/ calc avgmid price from quotes table for `GOOG

t1:select avgmid:avg .5*bid+ask by 5 xbar time.minute from quote where sym =`GOOG

/ avg mid quote = (bid + ask) /2
/ since you're grouping into 5 xbar, avg will calc avg over 5 min bucket
/ by = group, so this becomes keyed by 5 xbar time

minute| avgmid
--------------
09:30 | 79.7
09:35 |	80.4
09:40 |	79.5
09:45 |	79.4
09:50 |	80.4

/ calc avg price in 5 minute time window for `GOOG

t2:select avgprice: avg price by 5 xbar time.minute from trade where sym=`GOOG

/ notice some buckets have nulls = no trades during this bucket

minute| avgprice
----------------
09:30 | 80.0
09:35 |	
09:40 |	79.7
09:45 |	
09:50 |	80.4

/ combine the 2 tables together

t1 uj t2

minute| avgmid | avgprice
--------------------------
09:30 |  79.7  |  80.0
09:35 |	 80.4  |
09:40 |	 79.5  |  79.7
09:45 |	 79.4  |
09:50 |	 80.4  |  80.4

/ fill nulls with prev price (since no trades)

fills t1 uj t2

minute| avgmid | avgprice
--------------------------
09:30 |  79.7  |  80.0
09:35 |	 80.4  |  80.0
09:40 |	 79.5  |  79.7
09:45 |	 79.4  |  79.7
09:50 |	 80.4  |  80.4
```




<a name="qsqljoins_problem_set"></a>
## 🔴 22. qSQL Joins Problem Set
[Top](#top)

```q
\l ex-joins.q

\a

/ **fbTrades** (headers = dt, sym, size, book)
/ **newsItems** (headers = ndate, ticker, title) 
/ **quote** (headers = date, time, sym, size, cond, bid, ask, asize, bside)
/ **stock** (headers = sym, sector, employees)
/ **trade** (headers = dt, sym, price, size)
```

**🔵 22.1 Find the total value of trades by sector, include sectors that are unknown (totalvalue = price x size)**

```q
/ the columns you need are price x size (trade table) and sector (stock table) 
/ need to use left join because 1) include null sectors 2) union join would dupe values 
/ also - union join only works on tables. if you do meta trade + meta stock, you'll see stock = dictionary

trade lj stock
/ joins tables together, but does not calculate totalValue

dt        |sym|price|size|sector|employees
-------------------------------------------
2015-01-01|C  |	10.0| 10 | Fin  | 262000
2015-01-02|C  | 10.5| 100| Fin  | 262000
2015-01-04|DBK|	35.6| 55 |	|	


select totalvalue: price*size by sector from trade lj stock
/ can perform calc on joined tables

sector | totalValue
-------------------
	|,1,958
Fin	| 100 1,050 3,900 2,200 51,000 101,600f
Tech	| 20,200 306,000f

/ need to aggregate values so add in sum

select totalValue:sum price*size by sector from trade lj stock

sector   | totalValue
-------------------
         | 1958.0
`Fin`    | 159850.0
`Tech`   | 326200.0

/ amend blank null to "unknown"

select totalValue:sum price*size by `unknown^sector from trade lj stock

sector   | totalValue
-------------------
`Fin`    | 159850.0
`Tech`   | 326200.0
`unknown`| 1958.0

/ use `unknown^sector to rename the null sectors (visually more appeasing)
/ price * size will get you all the individual prices, but you want an aggregate figure. so need to use sum price
/ queried by sector, so this becomes keyed
```

<hr>

**🔵 22.2 Combine trade and fbTrades into a table t2, sorted by date. Include all columns**

```q
/ include all columns, so we use union join
/ can't use lj since not keyed

t2: trade uj fbTrades

dt        |sym  |price |size|book
----------------------------------
2015-01-06|AAPL |1020.0| 300| 	
2015-01-07|MS	|254.0 | 400| 	
2015-01-02|FB	|      |1000| A
2015-01-03|FB	|      |1000| B
2015-01-05|FB	|      |1000| A

/ joins tables together, but doesnt sort by date

t2:`dt xasc trade uj fbTrades

dt        |sym  |price |size|book
---------------------------------
2015-01-02|FB	|      |1000| A
2015-01-03|FB	|      |1000| B
2015-01-05|FB	|      |1000| A
2015-01-06|AAPL |1020.0| 300|	
2015-01-07|MS	|254.0 | 400|	

/ `dt xasc sorts dates by ascending
/ since you are joining table together, no select query
```

<hr>

**🔵 22.3 Find the highest and lowest price in the trade table for each sym**

```q
/ highest = max

select max price by sym from trade

sym | price
------------
AAPL| 1020.0
C   | 11.0
DBK | 35.6
MS  | 260.0

/ lowest = min

select min price by sym from trade

sym | price
-------------
AAPL| 1010.0
C   | 10.0
DBK | 35.6
MS  | 254.0
```

<hr>

**🔵 22.4 Find the 2 highest trade prices for each sym**

```q

select price by sym from trade

sym | price
------------------
AAPL| 1,020 1,010f
C   | 10 10.5 11
DBK | ,35.6
MS  | 260 255 254f

/ this returns all prices grouped by sym

select 2 sublist desc price by sym from trade

sym | price
------------------
AAPL| 1,020 1,010f
C   | 11 10.5
DBK | ,35.6
MS  | 260 255f

/ sublist = creates a subset of a list
/ 2 sublist = takes 2 
/ desc price = sorts by high to low

ungroup select 2 sublist desc price by sym from trade

sym | price
------------------
AAPL| 1,020
AAPL| 1,010
C   | 11 
C   | 10.5
DBK | 35.6
MS  | 260
MS  | 255

/ if you use ungroup, you will break apart the by grouping

```

<hr>

**🔵 22.5 Find the average daily price for each sym in trade table. Join the newsItems table to show only those items where the sym had a newsItem on that date**

```q

trade
dt        | sym |price |size
-----------------------------
2015-01-01| C   |10.0  | 10
2015-01-02| C   |10.5  | 100
2015-01-03| MS  |260.0 | 15
2015-01-04| C   |11.0  | 200
2015-01-04| DBK	|35.6  | 55
2015-01-05| AAPL|1010.0| 20
2015-01-06| AAPL|1020.0| 300
2015-01-07| MS	|255.0 | 200
2015-01-07| MS	|254.0 | 400

newsItems
ndate      | ticker | title
----------------------------------------------
2015-01-06 |   MS   | traders did it!
2015-01-04 |   C    | regulators investigating

/ from trade table, find avg price. then join the newsItem table where matches date and sym
/ so date and sym need to be keys in the newsItems table
/ notice the column headers are different in the newsItems table
/ for a ij, the column headers have to match up!

/ first step is calc the avg price grouped by dt, sym from trade table

t1: select avgprice: avg price by dt, sym from trade

dt        | sym | avgprice
---------------------------
2015-01-01| C   | 10.0
2015-01-02| C   | 10.5
2015-01-03| MS  | 260.0
2015-01-04| C   | 11.0
2015-01-04| DBK | 35.6
2015-01-05| AAPL| 1010.0
2015-01-06| AAPL| 1020.0
2015-01-07| MS  | 254.5

/ change column names for newsItems table + add keys to first 2 cols

t2: 2!`dt`sym xcol newsItems

dt         |  sym   | title
----------------------------------------------
2015-01-06 |   MS   | traders did it!
2015-01-04 |   C    | regulators investigating

/ then use an ij to join the 2 tables together

(select avg price by dt, sym from trade) ij (2!`dt`sym xcol newsItems)
/ or simply:
t1 ij t2

dt        | sym |price|title
----------------------------------------------
2015-01-04|  C  |11.0 |regulators investigating

/ inner join = only rows that match will be returned
/ need to set key to newsItems table in order for the ij to work
/ notice nothing joined for MS since the date didnt match
/ so only C was returned in the ij
```

<hr>

**🔵 22.6 Take the newsItems table and join the trade table to bring in the latest price for each ticker**

```q
newsItems
ndate      | ticker | title
----------------------------------------------
2015-01-06 |   MS   | traders did it!
2015-01-04 |   C    | regulators investigating

trade
dt        | sym |price |size
-----------------------------
2015-01-01| C   |10.0  | 10
2015-01-02| C   |10.5  | 100
2015-01-03| MS  |260.0 | 15
2015-01-04| C   |11.0  | 200
2015-01-04| DBK	|35.6  | 55
2015-01-05| AAPL|1010.0| 20
2015-01-06| AAPL|1020.0| 300
2015-01-07| MS	|255.0 | 200
2015-01-07| MS	|254.0 | 400

/ take newsItem table, join the trade table to add column for latest price
/ need to amend columns of newsItems to match trade table (dt, ticker)

`dt`sym xcol newsItems

dt         |  sym   | title
----------------------------------------------
2015-01-06 |   MS   | traders did it!
2015-01-04 |   C    | regulators investigating

/ need to key the sym column for trade table

/ since they want the latest price, 2015.01.03 = no trades for MS
/ so we need to retrieve the last price
/ easiest way to do this is to sort by `dt ascending
/ so the ij will automatically take the last price
/ luckily table is already sorted by ascending, but just in case:

`dt xasc `sym xkey trade

sym     dt              price   size
-------------------------------------
C	2015-01-01	10.0	10
C	2015-01-02	10.5	100
MS	2015-01-03	260.0	15
C	2015-01-04	11.0	200
DBK	2015-01-04	35.6	55
AAPL	2015-01-05	1010.0	20
AAPL	2015-01-06	1020.0	300
MS	2015-01-07	255.0	200
MS	2015-01-07	254.0	400

/ join the table via inner join

(`dt`sym xcol newsItems) ij (`dt xasc`sym xkey trade)

dt         |  sym   | title                   | price| size
------------------------------------------------------------
2015-01-06 |   MS   | traders did it!         | 260 | 15 
2015-01-04 |   C    | regulators investigating| 10  | 10

/ then you can delete the size column

delete size from (`dt`sym xcol newsItems) ij (`dt xasc`sym xkey trade)

dt         |  sym   | title                   | price
------------------------------------------------------
2015-01-06 |   MS   | traders did it!         | 260 
2015-01-04 |   C    | regulators investigating| 10  
```

```q
/ alternative solution: as of join method

/ quick 101
/ aj [`col_1`col_2; soure_table; `col_1`col_2 lookup_table]

/ last item of columns will be less than or equal join
/ aj looks for values (columns) from source to lookup table and pulls in the most recent price

aj [`ticker`ndate;newsItems; `ndate`ticker xcol trade]

/ from newsItems table, retrieve values in columns `ticker and `ndate
/ look for matches in trade table, rename dt to `ndate and sym to `ticker
/ it will pull in the most recent values in the matching columns (price, size)

dt         |  sym   | title                   | price| size
------------------------------------------------------------
2015-01-06 |   MS   | traders did it!         | 260 | 15 
2015-01-04 |   C    | regulators investigating| 10  | 10

/ delete the size column

delete size from aj [`ticker`ndate;newsItems; `ndate`ticker xcol trade]

dt         |  sym   | title                   | price
------------------------------------------------------
2015-01-06 |   MS   | traders did it!         | 260 
2015-01-04 |   C    | regulators investigating| 10  
```

<hr>

<a name="timeseries_joins"></a>
## 🔴 23. Timeseries Tables Joins
[Top](#top)

<a name="asof_join"></a>
### 🔵 23.1 As of Join

```q
/ used to find last value from one table, that matches the source table (prevailing quote)
/ for example, from a table of trades, you want to look up the most recent price or bid size
/ joins the closest matches from one table to another

aj [`col_1`col_2; soure_table; lookup_table]

/ syntax = aj [column; source table; lookup table]
/ last item of columns will be less than or equal join
/ one of the columns is usually time, since you want to pull in prevailing price
```
```q
/ As of Time Join Case Study

/ Find the latest bid for list of syms in table t

t: ( [] time: 07:00 08:30 09:59t; sym:`a`a`b; price: 0.9 1.5 1.9; size:100 200 300)
q: ( [] time: 08:00 09:00 10:00t; sym:`a`b`a; bid: 1 9 4)

table t:
time    |sym|price| size
-------------------------
07:00:00| a | 0.9 | 100
08:30:00| a | 1.5 | 200
09:59:00| b | 1.9 | 300

table q:
time     |sym | bid
-----------------
08:00:00|  a  |	1
09:00:00|  b  |	9
10:00:00|  a  |	4

aj [`sym`time; t;q]

/ syntax = aj [`columns; source table; `columns lookup table]
/ from columns `sym`time from table t, lookup table q and return table q columns 
/ t = source table
/ q = lookup table
/ column names must match

time    |sym|price| size| bid
-----------------------------
07:00:00| a | 0.9 | 100 |
08:30:00| a | 1.5 | 200 | 1
09:59:00| b | 1.9 | 300 | 9

/ from t, look through each sym, then time (less than or equal to)
/ from t, first row = a. lookup a in q, but no time less than or equal to 7:00am. so bid = null
/ from t, 2nd row = a. lookup a in q, found 8:00am <= 8:30, so pull in bid = 1
/ from t, 3rd row = b. lookup bi n q, found 9:00am <=9:59, so bid = 9
```

```q
fq: update qtime:time, qsym:sym from q
ft: update ftime:time, fsym:sym from t

/ create new table fq with columns qtime and qsym
/ create new table ft with columns ftime and fsym

table ft:
time    |sym| bid | size| ftime   | fsym
-----------------------------------------
07:00:00| a | 0.9 | 100 |07:00:00 | a
08:30:00| a | 1.5 | 200 |08:30:00 | a
09:59:00| b | 1.9 | 300 |09:59:00 | b

table fq:
time    |sym| bid|  qtime | qsym
--------------------------------
08:00:00| a |  1 |08:00:00| a
09:00:00| b |  9 |09:00:00| b
10:00:00| a |  4 |10:00:00| a

aj [`sym`time;ft;fq]

time    |sym|price|size| ftime  |fsym| bid | qtime    | qsym
------------------------------------------------------------
07:00:00| a | 0.9 | 100|07:00:00| a  |     |          |
08:30:00| a | 1.5 | 200|08:30:00| a  |  1  | 08:00:00 |	a
09:59:00| b | 1.9 | 300|09:59:00| b  |  9  | 09:00:00 |	b

/ aj0 is the same as aj, but uses the lookup tables time column
```

<a name="uniontime_join"></a>
### 🔵23.2 Union Time Join
```q
/ union join combines all entries from both tables, then can sort by time

q uj t

time        |sym|bid|price|size
--------------------------------
08:00:00.000| a | 1 |	  |   	
09:00:00.000| b | 9 |	  |
10:00:00.000| a | 4 |     |
07:00:00.000| a |   | 0.9 | 100
08:30:00.000| a |   | 1.5 | 200
09:59:00.000| b |   | 1.9 | 300

`time xasc q uj t

time        |sym|bid|price|size
--------------------------------
07:00:00.000| a |   | 0.9| 100
08:00:00.000| a | 1 |	 |
08:30:00.000| a |   | 1.5| 200
09:00:00.000| b | 9 |  	 |
09:59:00.000| b |   | 1.9| 300
10:00:00.000| a | 4 |	 |
```

<a name="windowtime_join"></a>
### 🔵 23.3 Window Time Join

```q

/ wj[windows;cols;tab1;(tab2;(agg;col_1);(agg;col_1))]
/ window = usually 2 lists of times
/ cols = list of columns to match on
/ tab1 = table to join onto
/ tab2 = table with list of cols to join on and aggregation functions
```
```q
/ wj allows you to specify the window + aggregation function used to join
/ wj aggregate values within an interval - whereas AJ would join most recent value,
/ a wj would join an aggregation of the available quotes in a given time interval
/ for example, 15 mins before trade occurred

table t:
time        |sym| price
----------------------
09:00:00.000| a | 10.0
09:04:00.000| a	| 11.0
09:12:00.000| a	| 12.0
09:13:00.000| a	| 13.0

table q:
time        |sym| bid
----------------------
09:00:00.000| a | 10.0
09:01:00.000| a	| 10.0
09:02:00.000| a | 11.0
09:03:00.000| a | 13.0
09:04:00.000| a | 13.0
09:05:00.000| b | 14.0
09:06:00.000| b | 14.0
09:07:00.000| b | 15.0
09:08:00.000| a | 15.0
09:09:00.000| a | 17.0
09:10:00.000| a | 17.0
09:11:00.000| a | 18.0
09:12:00.000| a | 18.0

/ from table t, produce a time interval 2 mins +\- for each row of time

windows:flip t.time +\: -00:02 00:02t

08:58:00.000 09:02:00.000 09:10:00.000 09:11:00.000
09:02:00.000 09:06:00.000 09:14:00.000 09:15:00.000

wj[windows;`sym`time;t;(q;(::;`bid))]

time        |sym| price|  bid
---------------------------------
09:00:00.000| a | 10.0 | 10 10 11f
09:04:00.000| a | 11.0 | 11 13 13f
09:12:00.000| a | 12.0 | 17 18 18f
09:13:00.000| a | 13.0 | 18 18f

/ wj will output same number of rows as original table t
/ windows - time interval pairs you created
/ columns you want to match on (sym, time) within source table t
/ table q = lookup table
/ :: = return all values from the bid column
/ 1st row, from table t, 09:00 for sym a, look up in table q, matched sym (a), from 8:58 to 9:02, and returns any bids
/ 2nd row, from table t, 09:04 for sym a, look up in table q, matched sym (a), from 9:02 to 9:06, and returns any bids 

wj[windows;`sym`time;t;(q;(::;`bid); (avg;`bid); (count;`bid))]

/ can perform functions! 
/ so after returning all the bids ::
/ next column = retrieve avg bids 
/ next column = retrieve count of bids
/ notice how the column name doesnt change though

time        |sym|price|    bid    |bid | bid
---------------------------------------------
09:00:00.000| a |10.0 | 10 10 11f |10.3| 3
09:04:00.000| a |11.0 | 11 11 13f |11.6| 3
09:12:00.000| a |12.0 | 17 17 17f |17.0| 3
09:13:00.000| a |13.0 | 17 17f	  |17.0| 2
```
```q
wj vs wj1
/ wj pulls in prevailing values not within time window
/ wj1 strictly excludes values outside the interval (for ex, if time interval was 10:00 - 10:15)
```

<a name="adverbs_header"></a>
## 🔴 24. Adverbs
[Top](#top)

```q
/ an adverb modifies an existing verb or function to alter how its applied to its arguments
/ combines 2 verbs and uses it as a new function

each both x,'y 
each left x,\: y
each right x,/: y 	
scan x \ y
over x / y
```

<a name="eachboth_adverbs"></a>
### 🔵 24.1 Each Both

```q
/ joins corresponding elements from two vectors of the same length
```

### EACH BOTH - 2 lists

```q
1 2 3 ,' 10 20 30
1 10
2 20
3 30

/ concatenates the first elements of L and to first element of K
/ lists must be same length
```

### EACH BOTH - 2 dictionaries 
```q
d1
key | value
----------
 p  |  1
 o  |  2
 i  |  3

d2
key | value
---------
 p  |  4
 o  |  5
 k  |  6

d1,d2 
/ simple join

key | value
---------
 p  |  4
 o  |  5
 i  |  3
 k  |  6

/ if you simply join dictionaries, the d2 will override anything existing keys in d1 (p, o)
/ acts like an UPSERT
```
```q

d1,'d2 
/ each both

key| value
---------
 p | 1 4
 o | 2 5
 i | 3 
 k | 6

/ EACH BOTH will join the values together
/ retains the keys, and combines the values together
```

### EACH BOTH - Tables

```q
t1: ([] a: 1 2 3)
t2: ([] b: 4 5 6)

t1, t2
`mismatch

/ can't simply join; mismatch (because rows have different columns names)

t1, 't2

a | b
------
1 | 4
2 | 5
3 | 6

/ each both will stitch the two tables together
```

```q
a: 1 1 1
b: 5 5 5

+'[a;b]
6 6 6

/ this is another syntax to use each both
```

<a name="each_monadic"></a>
### 🔵 24.2 Each

each modifies a monadic function to make it operate one level deeper

```q
/ each useful for nested lists

j: ("race fast, safe car."; 0 1 2; `a`b`c)
"race fast, safe car." 
0 1 2
a b c
```
```q
reverse j
a b c
0 1 2
"race fast, safe car."

/ so this reverses the mixed list at the top most level
```
```q
reverse each j
".rac efas , tsaf ecar"
2 1 0
c b a

/ reverse within each list
```

<a name="eachright_eachleft"></a>
### 🔵 24.3 Each Right / Each Left
```q
/ similar to concatenate
/ x,\: each left; will join left item (x) to each item on left
/ x,/: each right; will join left item (x) to each item on right
```
### Each Left

```q
x,\:y 

/ The top of the \ points LEFT
/ Adds EACH element of LEFT (x) to ENTIRE y 

x: 1 2 3
y: `a`b`c
x,\:y

1`a`b`c
2`a`b`c
3`a`b`c
```

### Each Right
```q
x,/:y

/ The top of the / points RIGHT
/ Adds EACH element of y to the ENTIRE x

x: 1 2 3
y: `a`b`c
x,/:y

1 2 3`a
1 2 3`b
1 2 3`c
```

```q
/ EXAMPLE 1

st:("welcome";"to the"; "terminal")
"welcome"
"to the "
"terminal" 

">",/:st

/ joins the left item to each item on right

">welcome"
">to the "
">terminal" 

">",st

/ if you simply joined it, it will join it at the top most level of the list

">"
"welcome"
"to the "
"terminal" 

st,\:"--->"

/ each left; adds right hand argument to each of st

"welcome--->" \
"to the---> " \
"terminal--->" 
```

```q
/ EXAMPLE 2

1 2 +/: 100 200 300

/ each right; since 2 arguments on left, there will be 2 columns

key | value
-----------
101 | 102
201 | 202
301 | 302
```

```q
/ EXAMPLE 3

1 2 +\: 100 200 300

/ each left (the bar tilts towards left);
/ since 3 arguments on right, there will be 3 columns

key |  value
---------------
101 | 201 | 301
102 | 202 | 302
```

<a name="scan_adverb"></a>
### 🔵 24.4 Scan

```q
/ scan is an accumulating iterator
/ returns the result of EACH result
/ useful for running totals, running products, where the previous value is used in the next value calculation

1 +\ 0 1 2 3
1 2 4 7

/ returns each result
```

```q
/ EXAMPLE 2

{x + y} \ [1 2 3 4 5]
{x + y} scan [1 2 3 4 5]
1 3 6 10 15

/ 1+0 =1; 1+2 = 3; 3+3=6; 4+6=10; 5+10=15
/ can also use "scan" instead of \
```

```q
{x,y} \ [1 2 3 4 5]
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

<a name="over_adverb"></a>
### 🔵 24.5 Over

```q
/ over is an accumulating iterator
/ returns the final result

1 +/ 0 1 2 3
7
```

<a name="eachprevious_adverb"></a>
### 🔵 24.6 Each Previous / Each Prior

```q
/ each prior = perform operation on element with its prior element

10 + ': 1 2 3 4 7
11 3 5 7 11

/ 10 + 1 = 11
/ 1 + 2 = 3
/ 2 + 3 = 5
/ 3 + 4 = 7
```

```q
-': [1 2 3 4]
1 1 1 1 

/ same as deltas 

deltas 1 2 3 4
1 1 1 1 
```
```q
{x,y}':[10 12 14 13 15]
10
12 10
14 12
13 14
15 13

{x,y}':[0;10 12 14 13 15]
10 0
12 10
14 12
13 14
15 13
```
```q
{x+y}': [1 2 3 4 7]
0N 3 5 7 11

/ O + 1 = ON
/ 1 + 2 = 3
/ 2 + 3 = 5
/ 3 + 4 = 7
```

<hr>

<a name="adverbs_problemset"></a>
## 🔴 25. Adverbs Problem Set
[Top](#top)

## 🔵 25.1 Given: ("cow"; "fox";"badger") use EACH RIGHT to prepend "the" before each item##

```q
/ each right = add x to each element of y

"the" ,/: ("cow";"fox";"badger")

/ or

strs: ("cow";"fox";"badger")
"the" ,/: strs

"the cow" 
"the fox" 
"the badger"
```

<hr>

## 🔵 25.2 Use EACH LEFT to add "jumped" to strs ##

```q
/ each left = add y to each element of x

strs,\: " jumped"

"cow jumped" 
"fox jumped" 
"badger jumped"

```
<hr>

## 🔵 25.3 Given the nested list: dd: (1 5 10; 200 30 40; 20 23 24), find the max of each list ##

```q
dd: (1 5 10; 200 30 40; 20 23 24)

max each dd
10 200 24

/ use each to calc max on each individual nested list
```
<hr>

## 🔵 25.4 Using EACH PRIOR, create a function that calculates the moving sum with window size of 2 ##

```q
/ each prior = perform action on each element with its prior element

L: 20 30 4 6 1 2
+': [L]
20 50 34 10 7 3

/ alternatively:

2 msum L

/ or 
 
{x+y}': [L]
 
```

<hr>

## 🔵 25.5 Use EACH BOTH to join the lists to give (5 8; 7 3; 9 4) ##
```q
numbers: 5 7 9
powers: 8 3 4

numbers, 'powers

key| value
----------
 5 | 8
 7 | 3
 9 | 4
```

<hr>

## 🔵 25.6 Use EACH BOTH to raise 5 to the power of 8, 7 to the power of 3, etc. ##

```q
numbers xexp' powers

390625 343 6561f
```

<hr>

## 🔵 25.7 A bank account pays 5% interest a year. Write a function that takes the current balance and returns the new balance after one year. Then use scan\ with that function to display the interest every year, up to 7 years in the future ##

```q
/ assume starting balance of 100

{x * 1.05} 100
105

{x * 1.05} \ [7; 100.]

105 
110.25
115.7625
...
140.71

/ use monadic version of scan that takes 2 arguments
/ first argument = how many times to run
/ second argument = starting value for function
```

<hr>

## 🔵 25.8 Create a function, fib, that takes a fibonnaci sequence as its argument and returns the sequence complete with the next entry ##

```q
/ the fib seq = 1 + prior 
/ 1 1 2 3 5 8 ...

fib: {sum -2#x}
fib 1 1

1 1 2

/ take last 2 elements of argument and sum it
```

<hr>

## 🔵 25.9 Use the over function to create a function, fibn, to generate a fib sequence n numbers long where n is the functions argument ##

```q
fibn: {x fib/ 1 1}
fibn 5
1 1 2 3 5 8 13

```

<hr>

## 🔵 25.10 Use the scan to calculate the depreciation of cars 

```q
/ c = initial car value
/ r = depreciation rate per year

depr:{[c;r] c*1-r%100}
depr[100;8]
92

/ What is the value after 5 years?

depr[;8]\[5;100]
100
92
84.64
77.86
71.63
65.90

/ use scan to iterate the function 5x
```

<hr>

<a name="importexport_header"></a>
## 🔴 26. Saving and Loading Data
[Top](#top)

<a name="txt_import"></a>
### 🔵 26.1) Reading TXT files

```q
/ assume you have a txt file in your directory called test.txt

hopen `:test.txt
read0 `:test.txt

/ file handler = a temporary reference number that an OS assigns to a file requested by a user to be opened
/ hopen function will open the txt file
/ read0 function will read the txt file
```

<a name="txt_export"></a>
### 🔵 26.2a) Manipulating File Handle

```q
/ to write to txt, simply use hopen to get the file handle, store the file handle, and store strings to it

fh:hopen `:hi.txt
fh "10"
fh "20"
neg[fh] "30"
read0 `:hi.txt

"1020"
"30"

/ by putting neg[fh], you enter into a new line

hclose fh

/ closes the file handle so you can no longer edit it
```

<a name="tables_exportformat"></a>
### 🔵 26.2b) Saving CSV files
```q
/ there are 2 ways to save to text:
/       1) save function (save `name.csv)
/       2) 0: operator 
 
/ 0: is used to load, prepare, and save text files
/ The benefit of exporting to CSV is that for transferring data to other systems their support is ubiquitous
/ However the space requirement of converting each digit of a number to separate characters is significant

trade
date        time          sym   price      size   cond
------------------------------------------------------
2013.09.28| 09:30:02.553| C   | 107.2018 | 63500 | B
2013.09.28| 09:30:02.701| MSFT| 96.87488 | 1700  | B
2013.09.28| 09:30:02.743| RBS | 97.11338 | 80700 | C
2013.09.28| 09:30:02.758| A   | 100.35   | 50300 | B
2013.09.28| 09:30:02.907| B   | 55.82187 | 92700 | A

save `trade.csv

/ syntax = save backtick filename.csv
/ this will be saved to your q folder

/ 0: allows you to choose custom separaters and file names

`newfilename.csv 0: ";" 0: trade 

/ saves trade table, separated by ; and newfilename 
/ ";" 0: trade = converts table to list of strings separated by semi colons
/ ; is what you are separating items with
/ trade = table name
```

### 🔵 26.3) Saving tables as txt, csv, excel, and xml files
```q

cars: ( [] maker: `Ford`Tesla`Honda; price: 100 200 300; weight: 1000 2000 3000)

maker| price| weight
---------------------
Ford | 100  | 1000
Tesla| 200  | 2000
Honda| 300  | 3000

save `cars.txt
save `cars.csv
save `cars.xls
save `cars.xml

/ this will automatically save and export your table to any of the file types in your directory

save `$"newdir/cars.txt"

/ this will create a new filepath and directory for your file to save your file
/ the new folder will be called "newdir"
```

<a name="export_tablenewname"></a>
### 🔵 26.4) Saving tables with a new name

```q
`carsnewname.csv 0: "," 0: cars

maker,price,weight
Ford,100,1000
Tesla,200,2000
Honda,300,3000

/ by using the 0: function, you can rename your file to anything you want (carsnewname)
/ "," 0: cars converts table to list of strings separated by commas
```

<a name="csv_import"></a>
### 🔵 26.5) Loading CSV Files

```q
/ the 0: function prepares, saves, and loads text files. 

tab1: ("ICS";enlist",")0: `:tab1.csv

/ 1st argument = datatype. "ICS" = Int, Char, Sym
/ 2nd argument = delimiter. For CSV it's a comma. Enlisting comma = column headers exist

tab1
a b c
------
1 A 4
2 B 5
3 C 6

/ to leave out certain columns, simply omit datatype in first argument

tab1: ("IC ";enlist",")0: `:tab1.csv
tab1
a b
---
1 A
2 B
3 C
```

```q
/ to load table with no column headers
/ leave out the enlisting of the delimiter

("ICS";",")0: `:tab2.csv

tab2
1 2 3
A B C
4 5 6

/ to turn into dictionary, set `a`b`c as keys

`a`b`c!("ICS";",")0: `:tab2.csv

a | 1 2 3
b | A B C
c | 4 5 6

/ to turn into table, flip dictionary

flip `a`b`c!("ICS";",")0: `:tab2.csv

a b c
-----
1 A 4
2 B 5
3 C 6
```
```q
/ Example 2

("**********"; ",") 0: `:nyse_20110621.csv

/ right hand of 0: = filename
/ left hand argument = how to prepare the data
/ the **** are just KDB datatype layers; one * for each column
/ this will interpret all values as strings, allowing for easy way to check the data

"symbol" | "A"
-------------------------
"date"   | "21-june-2011"
"open"   | "14.94"
"high"   | "15.94"
"low"    | "13.43"
"close"  | "24.52"
"volume" | "100"

("SSFFFFJ"; ",") 0: `:nyse_20110621.csv

/ replace the * with the datatype (string string, float float, long etc)
/ interprets the values more sensibly

symbol | A
-------------------
date   | 21-june-2011
open   | 14.94
high   | 15.94
low    | 13.43
close  | 24.52
volume | 100

("SSFFFFJ"; enlist ",") 0: `:nyse_20110621.csv

/ by adding in the enlist, you are treating the first column as a header
/ converts it into a table

symbol| date       | open | high | low | close  | volume
---------------------------------------------------------
A     |	21-Jun-2011| 48.7 | 50.32| 48.67| 49.82 | 3509600
AA    |	21-Jun-2011| 14.9 | 15.42| 14.92| 15.37 | 18310600
```

<a name="binaryfile_export"></a>
### 🔵 26.6) Saving to Binary Files
```q

/ binary files are a direct byte stream that is similar to kdb's in-memory representation of data. 
/ features include:
    1) Requires significantly less space than a text file (kdb+ supports compression) 
    2) Quicker to save load
    3) Reading / writing is simply streaming bytes, it is extremely fast.
    4) We use get / set to read/write.
    5) You can append and upsert.
    6) Once loaded in, the entire entity is stored in memory.
```
```q
set[filepath; data] / save data to selected filepath

/ filepath = symbol beginning with `: that specifies a file location using / as folder separators
/ data = any format of data structure is supported (tables, dictionaries, lists, atoms, etc)
```

```q
set[`:q/trade;trade]

/ filepath is q folder, trade binary file
/ trade table
/ this will save as binary file to your q file path
```

```q
d: `p`o`i!1 2 3

set[`:q/dict;d]

/ this will save as dictionary d to your folder
```

<a name="binaryfile_export"></a>
### 🔵 26.7) Loading Binary Files

```q
get `:q/dict
/ this will load the dict dictionary 

key | value
------------
p   | 1
o   | 2
i   | 3
```
<hr> 

<a name="functional_form"></a>
## 🔴 27. Functional Form
[Top](#top)

```q
/ functional form allows FUNCTIONS to be used as nouns

@[square; 3 4 5]
9 16 25

/ apply square function to 3 4 5

@[cube;3 4 5]
27 64 125

/ apply cube function to 3 4 5
```

```q
/ functional form allows you to pass a function as an noun

{@[x;3 4 5]}cube
27 64 125

/ here we have a function that accepts a function (cube) as its argument
/ @ = used for SINGLE arguments (x)
/ apply function cube as argument x
```

```q
.[raise; (2 2 2 3;3)]
8 8 8 27

/ dot operator used for multipe arguments
```

### Functional Select

```q
/ Functional Form Select Query Template

?[table name;where;grouping;aggregation]

/ where = given as a list
/ groupings = given as dictionary
/ aggregation = dictionary
```

```q
/ convert a query to its parse tree using PARSE

parse "select from trade"
?
`trades
()
0b
()

/ this is equilvalent to:

?[`trade;();0b;()]

/ ?[table name;where;grouping;aggregation]
/ table name, 
/ no where clause, use empty list ()
/ no grouping, use 0b
/ no aggregations, use empty list ()
```
```q
/ functional form gives no performance advantages
/ difficult to read/write
/ only use is for DYNAMIC QUERIES
```
```q
/ Let's say you want to select total size by sym, by cond, or by both
/ col name will be parameter in this query 

select total:sum size by sym from trade
select total:sum size by x from trade / wont work!
f:{select sum price by x from trade} / wont work!
f[`sym]

/ cannot substitute x for col name
/ column names cannot dynamically passed in queries in this way
/ have to use functional select instead

parse"select total:sum price by x from trade"
("?";`trade;;,`x!,`x;,`total!,("sum";`price))

/ parse the query to see its parse tree
/ then convert into functional form syntax

f:{?[trade;(); g!g:(),x; (enlist `total)! enlist(sum;`size)]}
f[`sym] / now this works
f[`sym`cond] / this also works

/ commas = atom so need enlist
/ trade = table name
/ no where = ()
/ grouping = is where we want to put x
/ use notation empty list join x as this allows x to be a single column name
/ or a list of col names
```
### Functional Form Example 2

```q
select tot:sum size by sym from trade where sym in `AAPL`GOOG

sym   tot
-------------------
AAPL | -1791519396
GOOG | 659934504

parse "select tot:sum size by sym from trade where sym in `AAPL`GOOG"
("?";`trade;,,("in";`sym;,`AAPL`GOOG);,`sym!,`sym;,`tot!,("sum";`size))

/ ,  indicate atoms which need to be turned into enlist
/ converting that into functional form

/ syntax ?[table name;where;grouping;aggregation]

?[trade;enlist(in;`sym;enlist `AAPL`GOOG);(enlist`sym)!enlist `sym;(enlist `tot)!enlist(sum;`size)]


sym   tot
-------------------
AAPL | -1791519396
GOOG | 659934504
```

### Functional Exec

```q
/ is like functional select, but if there is no by clause we use an empty list instead of a 0b
parse "exec sym from trade"
?
`trades
()
()
,`sym

?[`trades;();();`sym]
```

### Functional Update

```
/ uses an exclamation mark
parse "update mid:(bid+ask)%2 from quotes"
!
`quotes
()
0b
(,`mid)!,(%;(+;`bid;`ask);2)

![quotes;();0b;(enlist `mid!enlist(%;(+;`bid;`ask);2)]
```

<hr>

<a name="flat_tables"></a>
## 🔴 28. Flat Tables
[Top](#top)

```q
/ saved to disk as is, all info in one file 
/ can only be accessed by loading into memory
/ generally small, freq accessed datasets 
/ not suitable for large datasets
```

```q
price: ([] fruit:`apple`pear`banana; qty: 10 20 30; price: 100 200 300)

fruit  qty price
---------------
apple	 10	 100
pear	  20	 200
banana	30	 300

/ to save as flat file to directory:

`:price

/ this will save the table to your directory with table name = price
```

<a name="rename_flatfiles"></a>
### 🔵 28.2 Renaming Flat Files When Saving 

```q
`:new_name set price

/ this will save and rename the table = new_name
/ set + (price = table name)
```

<a name="loading_flatfiles"></a>
### 🔵 28.3 Loading Flat Files 

```q
/ to load these flat files:

fruitorders: get`:new_name

/ use get function, can rename table as you load it

load `:price

/ can also use load `: function
```
<hr>

<a name="splayed_tables"></a>
## 🔴 29. Splayed Database Tables
[Top](#top)

### TimeStored Set Method

<a name="splay_setfunc"></a>
### 🔵 29.1 Set Function Method - TimeStored

```q
/ splaying a table in kdb+ allows saving a table with separate files for each column
/ this reduces memory required as columns are only memory mapped as needed
/ you cannot splay a table that is keyed! must 0! to remove key first

t: ([] a: 1 2 3; b: .z.d+1 3 5)

a b
------------
1 2021-06-30
2 2021-07-02
3 2021-07-04

set[`:splay/t/; t]

/ set = saves binary / splayed tables
/ first argument = file path. splay is the folder name (make sure you have / after t to SPLAY the table)
/ t = the underly table you want to save
/ the table (t) becomes a folder, and each column becomes a file
/ the .d file is a list that contains the column names and order
```

<a name="splay_getfuncTS"></a>
### 🔵 29.1 Get Function - TimeStored

```q
get `:splay/t/a
1 2 3

/ get function = returns values in that column

get `:splay/t/.d
a b

/ .d file contains the name of all columns
```
<a name="splay_enusymTS"></a>
### 🔵 29.2 Enumerating Syms - TimeStored

```q
/ any sym column you want splayed must first be enumerated
/ enumerate = converting a list of values to a defined domain which restricts values to that domain

sy: exec distinct sym from trade
C MSFT RBS A B BAC...

/ exec returns your query in a single row (instead of column)

update sym: `sy$sym from `trade

/ this will enumerate all the syms from trade table to the domain of sy

set[`:trade/; trade]

/ now you can save your trade table as a splayed table
```

### AquaQ Method

<a name="splay_savingAQ"></a>
### 🔵 29.3 Saving Splayed Tables - AquaQ

```q
/ each column of the table saved as separate file
/ .d file is created to store the correct order of the columns
/ when a splayed tab is loaded to a session, it is mapped in, not loaded to physical memory
/ if i have large table and only want to access one column, only that one column loaded
```

```q
/ Splayed Table = each column stored as separate file
/ A directory(folder) is created which contains a file for each column + a .d file (order of column)

prices2: ([] price: 100 200 300; qty: 10 20 30)

`:splayprice2/ set price2

/ syntax = `: + table name you want to save to + / + original table name
/ renames table to splayprice2
/ adding a backslash saves the table as a splayed table
/ this will create a folder called splayprice2, and within it, have individual columns as files
/ saving a table with a sym column requires some extra step
```

<a name="splay_memoryAQ"></a>
### 🔵 29.4 Memory Considerations - AquaQ

```q
/ when load splayed table into q session, it is mapped to memory, not read to physical memory
/ shown by mmap function using .Q.w function

.Q.w[]

/ displays memory usage

key  value
--------------
used	359680
heap	67108864
peak	67108864
wmax	0
mmap	0
mphy	16556564480
syms	680
symw	28177

/ mmapp = 0

prices2: get`:splayprice2
prices2

key  value
----------------
used	359680
heap	67108864
peak	67108864
wmax	0
mmap	80
mphy	16556564480
syms	680
symw	28177

/ after loading the splayed table, mmap now 80
```

<a name="splay_arrangecolsAQ"></a>
### 🔵 29.5 Rearrange Columns / Orders - AquaQ

```q
/ check what columns are available in .d file for splayed table

get `:splayedprice2/.d
`price`qty
```
```q
/ re-arrange column order in .d file for splayed table

`:splayedprice2/.d set `qty`price

/ changed order from `price`qty to `qty`price

load `:splayedprice2
splayedprice2

qty price
---------
10	 100
20	 200
30	 300
```
<a name="splay_retrievecolsAQ"></a>
### 🔵 29.6 Retrieving Values from Splayed Columns - AquaQ

```q
/ retrieve values from individual columns

get `:splayedprice2/qty
10 20 30

get `:splayedprice2/price
100 200 300
```

<a name="splay_addcolsAQ"></a>
### 🔵 29.7 Adding new Column to Splayed Table - AquaQ

```q
/ add new column to splayed table

`:splayedprice2/date set 2020.01.01 2020.01.02 2020.01.03

/ this will append a new column called date with the values
/ will also add a new directory=date in the splayed table folder
/ but still need to update .d file!

splayedprice2

price qty
---------
100	  10	
200	  20	
300	  30	

`:splayedprice2/.d set `price`qty`date

/ sets and reorders columns in .d

load `:splayedprice2
splayedprice2

price qty date
--------------------
100	  10	 2021-01-01
200	  20	 2021-01-02
300	  30	 2021-01-03

/ now when you query the splayedprice2 table, column date is added
```
```q
/ to delete a column in a splayed table

hdel `:splayedprice2/date

/ use hdel function to remove file from disc
/ deletes the column date file

`:splayedprice2/.d set `price`qty

/ then you need to update the .d file

load `:splayedprice2
splayedprice2

/ reload the splayed table

price qty
---------
100	  10
200	  20
300	  30

/ now the date column is gone
```

<a name="splay_addrowAQ"></a>
### 🔵 29.8 Adding New Row to Splayed Table - AquaQ

```q
/ add new row to splayed table

`:splayedprice2/ upsert (400; 40)
splayedprice2

price qty
---------
100	  10
200	  20
300	  30

/ if you immediately try to query the table, the new row is NOT added
/ need to first re-load the table

\l splayedprice2
splayedprice2

price qty
---------
100	  10
200	  20
300	  30
400   40
```

<a name="splay_sortAQ"></a>
### 🔵 29.9 Sorting Splayed Tables - AquaQ

```q
/ sort splayed table by ascending/descending

`price xdesc `:splayedprice2/
get `:splayedprice2/

/ after sorting use get to retrieve table

price qty
---------
400	  40
300	  30
200	  20
100	  10
```

<a name="splay_enusymAQ"></a>
### 🔵 29.10 Enumerating Syms for Splayed Tables - AquaQ

```q
/ .Q.en used to enumerate sym colums in a splayed table
/ symbol columns have to be enumerated before splaying the table
/ to enumerate a column means the unique symbols are identified
/ and an index assigned to each unique symbol

fruitorders: ([] fruit:`apple`pear`banana; qty: 10 20 30; price: 100 200 300)
`:fruitdb/fruitorders/ set .Q.en[`:fruitdb; fruitorders]

/ fruitdb = directory for database
/ set .Q.en enumerates the syms

fruitdb
    fruitorders (folder)
         .d
         fruit
         price
         qty
    sym file

load `:fruitdb/fruitorders

/ this loads the fruitdb database to memory

fruitorders

fruit  qty price
---------------
apple	 10	 100
pear	  20	 200
banana	30	 300
```

<hr>

<a name="partitioned_db"></a>
## 🔴 30. Partitioned Database
[Top](#top)

```q
/ most frequently used for large databases
/ separate folders (directory) for each partition
/ most common partition is by date
/ each date has own directory, and within each directory, there are folders for each splayed table
```

<a name="savingpartition"></a>
### 🔵 30.1 Saving Partitioned Tables - AquaQ

```q
/ a partitioned table is usually first split by date
/ then within each date, the table is splayed by columns

price2: ([] price: 100 200 300; qty: 10 20 30)
price3: ([] price: 500 600 700; qty: 50 60 70)

`:parprice/2021.01.01/ex/ set price2
`:parprice/2021.01.02/ex/ set price3

/ set partition by date (one for each date)
/ table name = ex
/ within each ex, each individual column is saved as a file
/ hierarchy goes DATE -> EX -> (individual columns)
/ remember to include the last / after table name! 

\l parprice
ex

/ loads the partitioned table on the overall directory

date       price qty
--------------------
2021.01.01 100	  10
2021.01.01 200	  20
2021.01.01 300	  30
2021.01.02 500	  50
2021.01.02 600	  60
2021.01.02 700	  70
```


<a name="part_index"></a>
### 🔵 30.2 Index Querying - AquaQ

```q
/ can use .Q.ind to access table using indexing

.Q.ind[ex; 1 2]

date       price qty
--------------------
2021.01.01 200	  20
2021.01.01 300	  30

/ returns rows 2, 3 (index position 1, 2)
```

<a name="part_fillmissing"></a>
### 🔵 30.3 Fill Missing Tables - AquaQ

```q
/ can use .Q.chk to fill missing tables within a partitioned database
/ suppose we have empty 2021.01.03 

.Q.chk[`:.]

/ this will populate the partition accordingly
```

<a name="part_savingsplayed"></a>
### 🔵 30.4 Saving a Splayed Table into a Database Partition

```q
/ .Q.dpft used to save a splayed table into a database partition 

.Q.dpft[`:hdb;2021.01.01;`fruit;`fruitorders]

/ 1st argument = database directory (hdb)
/ 2nd argument = database partition (date)
/ 3rd argument = column to sort and apply the parted attribute to (fruit)
/ 4th argument = the table to be saved 

hdb
   2021.01.01
      fruitorders
         .d
         fruit
         price
         qty
```

```q
/ .Q.hdpf used to save all tables in the global namespace to hdb and purge all data in tables

.Q.hdpf[0;`:hdb;2021.01.01;`fruit]

/ 0 = historical port
/ hdb = database directory
/ 2021.01.01 = partition
/ `fruit = column which is to be sorted and parted enumerated column

fruitorders

fruit quantity prrices
----------------------

/ all data has been purged
```

<a name="part_functions"></a>
### 🔵 30.5 Using Functions to save a Partitioned Table (no sym)

```q
/ using a function to save a partitioned table

saveTradePartition:{ [d] 
    show "saving trade ",string d;
    dirHandle: hsym `$"pdb/",string[d],"/trade/";
    dirHandle set select time, price, size from trade where date= d};

/ d = argument for date. (Will partition by date)
/ first row = just tells you saving xxx date
/ second row = this is the directory being saved to
             / hsym = converts sym to file sym
             / pdb/ = database directory (splayed /)
             / string d = give us date as a string
             / trade = tablename
/ third row = set function with dirHandle = path to save to (has / at end so splayed)
/ followed by columns you want to choose, from date = d
/ don't need date column since since partitioned by date


exec distinct date from trade

/ get all distinct dates from trade table

dts: exec distinct date from trade

/ save as dts

saveTradePartition each dts

/ runs function on each distinct date (dts)
/ will save each date as a partition

pdb
   2021.10.27
       trade
          .d
          price
          size
          time
   2021.10.28
       trade
          .d
          price
          size
          time
```

<a name="part_functionssym"></a>
### 🔵 30.6 Using Functions to save a Partitioned Table with Sym

```q
/ Using a function to save a partitioned table containing sym columns

/ saving partitioned tables containing sym columns
/ sym columns have to be enumerated against a sym file
/ enumerate = converting values to a defined domain which restricts values to that domain
/ can use KDB built in function .Q.dpft

saveTQPartition:{ [d] 
    show "saving ",string d;
    t::trade; / set trade table to global variable t (req for dpft)
    q::quote; 
	trade:: delete date from select from trade where date=d; / remove date col
	quote:: delete date from select from quote where date=d;
    r:.Q.dpft[`:pdb2; d; `sym; `trade];
    r:.Q.dpft[`:pdb2; d; `sym; `quote];
    trade::t; / restore trade table to full t
    quote::q;
    delete t from `.; / remove temp variables
    delete q from `.;
    r};

/ this time save both trade and quote table
/ remove date column because dont need to save date col cuz that is partitioned column
/ dpft = directory filepath, partitioned data (date), partedField (`p# attribute applied to), table of data
/ last argument of dpft must be a global variable !!
/ that's why we defined t::trade and q::quote earlier (set as global variable)

dts:exec distinct date from trade

/ shows distinct dates from trade table

saveTQPartition each dts

/ saves each date as a separate partition using above function
/ so function saves table to selected directory of partition
/ applies p attribute to sym column
/ enumerates any syms to sym file that's in the top most database directory

```
```q
/ what happens when you query a partitioned table?

select max price from trade where date = 2021.01.01

/ starts from date folder
/ looks at trade folder
/ looks at price file
/ selects max price
/ so very efficient query
```

<a name="debugging"></a>
## 🔴 31. Debugging
[Top](#top)

```q
/ if you see q)) that means you're in the debug mode
/ q))) means you are in an error trap wtihin an error trap
/ a single backslash \ lets us enter k mode. to exit, do another backslash \

f:{x*x}
g:{f[x]*y+10}
g[`a;2]
/ error

/ where is error?
.z.s / returns definition of current function
{x*x}

` / takes us 1 level higher to g

{f[x]*y+10
:3
36

/ colon (also called signal) forces line to be evaluated whichever value you give it
/ and rest of func to go on
/ forces x*x to = 3
/ 3 * 2 + 12 = 36 (right to left) 
/ helps to see if any further errors in your function
```

```q
/ use ON! to print
/ use control c to terminate a running process
```


<a name="atanddot_operator"></a>
## 🔴 32. @ and . Operator
[Top](#top)

<a name="squarebracket_at"></a>
### 🔵 32.1 Square Bracket Notation

```q
/ @ and . build on the functionality provided by the square bracket notation [ ]

/ if x is a data strructure, x[y] = index
x: 1 2 3 4 5
y: 3
x [y]
4

/ if x is a function, x[y] = apply

x:{(x*2) + 5}
y:3
x[y]
11
```
<a name="operator_at"></a>
### 🔵 32.2 @ Operator

```q
/ @ is used for single dimensional lists

list1: 1 6 3 8 5 4
index: 2

list1[index]
3

/ is the same as

@[list1;index]
3
```

<a name="operator_dot"></a>
### 🔵 32.3 . Operator

```q
/ . is used for nested lists

list2: (1 4 3; 2 6 7; 8 5 9)
row: 1
column: 2

list2[row][column]
7

/ is the same as

.[list2;1 2]
7
```
```q
list: (8 4 2; 9 3 1; 5 7 6)

/ think of a nested list like a matrix

8 4 2
9 3 1
5 7 6

list[1 2;2 1] 
1 3
6 7

/ [1;2] row 1, index position 2 = 1
/ [1;1] row 1, index position 1 = 3
/ [2;2] row 2, index position 2 = 6
/ [2;1] row 2, index position 1 = 7

/ dot notation

.[list; (1 2; 2 1)]
1 3
6 7

```

<a name="amending_at"></a>
### 🔵 32.4 Amending List Items using @
```q
/ amending using square bracket colon method [ ]:

list: "abcde"
list[3]: "D"
"abcDe"

/ using @ index instead:

@[list;3;:;"D]
"abcDe"

/ 1st argument = list name
/ 2nd argument = which index position
/ 3rd argument = : means whatever is here
/ 4th argument = replace with this
```
```q
/ mathematical operators can also be used:

list: 2 5 7 3 5 2
@ [`list;4;+;5] 
2 5 7 3 10 2

/ at index position 4, add 5
```
```q
/ can update more than one list item at a time

list: 1 6 3 5 2
@[list; 0 1; + 5]
6 11 3 5 2 

/ add 5 to the item at indexes 0 and 1
```
```q
/ can be used with non dyadic operators

list: "abcde"
@[list;4;upper] 
"abcdE"

/ upper is a monadic function
```

<a name="amending_dot"></a>
### 🔵 32.5 Amending List Items using .

```q
/ add 5 to each item in rows 1 and 2 and columns 1 and 2

list: (8 4 2; 9 3 1; 5 7 6)
8 4 2
9 3 1
5 7 6

.[list;(1 2;1 2); +; 5]
8 4 2
9 8 6
5 12 11

/ [1; 1] = 3 + 5 = 8
/ [1; 2] = 1 + 5 = 6

/ so 2nd row first element (9) doesn't change
```

<a name="advanced_at"></a>
### 🔵 32.6 Advanced use @ index

```q
/ l is a mixed list of syms and ints
/ m is a mapping of syms to ints


1: (`a; 1; 2; `b; 5; 9)
m: `a`b!100 200

@[l; where 011= type each 1;m]
100 1 2 200 5 9
```

<a name="advanced_at"></a>
### 🔵 32.7 Using . index with database tables

```q
/ can index into simple table using . operator
/ we can look up price for 1 key
/ if keys are not unique, will return first instance of the price for that key
/ to lookup price for multiple keys, build table to pass into expression

t: ([sym:`ibm`msft] price:1.2 9.8; size: 3 6)

sym | price | size
------------------
ibm |  1.2  | 3
msft|  9.8  | 6

/ retrieve value using .index 
/ can skip column names when looking up one key

.[t;(`ibm;`price)]
1.2

/ use tablelookup, return all values for column size
.[t;(([] sym:`msft`ibm); `size)]
6 3
```

<a name="zero_dot"></a>
### 🔵 32.8 zero dimensional amend (dot operator)

```q
/ .index allows us to amend entire object at once by passing in empty set of indices
/ if performed on list, lets us amend each list element

a: 10
.[a;();+;1]
11

list: (1 2;3 4 5;6 7 8 9)
1 2
3 4 5
6 7 8 9

.[list; ();+;10]
11 12
13 14 15
16 17 18 19
```

<a name="at_apply"></a>
### 🔵 32.9 @ Apply
```q
/ @ is used when function takes single argument
/ . is used when function takes multiple arguments

f:{2*x}

f[2]
4

/ @ apply method

@[f;2]
4
```
```q
l: (1 2 3; 4 5; 6 7 8 9)


flip l
error

/ you can't flip since nested list are different lengths
/ instead create empty lists of max length, then flip it

flip `a`b`c!@[max[c]#0N;;:;]'[til each c: count each l;l]

a| b | c
---------
1| 4 | 6
2| 5 | 7
3|   | 8
 |   | 9

/ turn the nested list into a dictionary, then flip it

```

<a name="dot_apply"></a>
### 🔵 32.10 . Apply
```q
g:{x+y}

g[4;5]
9

/ . notation

.[g;(4;5)]
9
```

<a name="racking"></a>
## 🔴 33. Racking
[Top](#top)


<a name="loadfakedb"></a>
### 🔵 33.1 Loading fakedb.q script


### Loading AQ fakedb.q script

```q
\l fakedb.q

makehdb[`:hdb;10;1000;1000]

/ `: directory name
/ 10 = number of partitions
/ 1000 = trades in each table
/ 1000 = number of quotes in each table

\l hdb

tables[]
`depth`quotes`trades

/ to view the tables, you have to use select

select from trades

date       | sym  | time                       | src | price | size
--------------------------------------------------------------------
2014-04-21 | AAPL | 2014-04-21T08:00:44.437000 | O   | 25.34 | 1785
2014-04-21 | AAPL | 2014-04-21T08:04:41.246000 | L   | 25.34 |  427
2014-04-21 | AAPL | 2014-04-21T08:04:47.586000 | L   | 25.34 | 1528
```

<a name="racking"></a>
### 🔵 33.2 Racking
```q
/ a common operation is to aggregate data using xbar
/ xbar only produces buckets where there is a value
/ if we need a timeseries where all values are present
/ then need to create a rack of times to join data to
```

```q

trade:([] sym:`GOOG`IBM`GOOG`IBM`IBM; 
       time: 09:00 09:01 09:20 09:32 09:34; 
       size: 200 100 1200 200 400; 
       price: 30.9 36 30.9 36.1 36.2)

sym  | time  | size | price
---------------------------
GOOG | 09:00 |  200 | 30.9
IBM  | 09:01 |  100 | 36.0
GOOG | 09:20 | 1200 | 30.9
IBM  | 09:32 |  200 | 36.1
IBM  | 09:34 |  400 | 36.2

/ lets bucket the size by sym in 15 min windows

select sum size by sym, 15 xbar time.minute from trade

sym  | minute | size
---------------------
GOOG | 09:00  |  200
GOOG | 09:15  |	1200
IBM  | 09:00  |  100
IBM  | 09:30  |  600

/ but not all syms + time buckets are present
/ ex, GOOG @ 9:30 isn't present
```

```q
/1 start by creating complete list of buckets (need start + end + buckets)

start: 09:00
end: 09:59
bucket: 15

/ so each bucket will be 15 mins

/2 number of buckets required for time span (end-start)

(end-start) % bucket
3.933

/3 round up to whole number

ceiling (end-start) % bucket
4

/ ceiling function will round 3.933 up to 4
```

```q
/4 create list of buckets by creating list of integers to num of buckets
/ this is done by multiplying each element x bucket size (15)

bucket * til ceiling (end-start) % bucket
0 15 30 45

/ bucket x til 4
/ 15 x 0 1 2 3

/5 add start time by making list of time buckets and rename as times

times: start + bucket * til ceiling (end-start) % bucket
09:00u; 09:15u; 09:30u; 09:45u
```

```q
/6 cross distinct syms with times list you just created and sort by sym

rack:(`sym xasc select distinct sym from trade) cross ([] minute:times)

sym  | minute
-------------
GOOG | 09:00
GOOG | 09:15
GOOG | 09:30
GOOG | 09:45
IBM  | 09:00
IBM  | 09:15
IBM  | 09:30
IBM  | 09:45

/ this creates a "rack" of every sym and every 15 min time bucket
```

```q
/7 join rack with original xbar table using # take operator

rack # select sum size, last price by sym, bucket xbar time.minute from trade

sym  | time  | size | price
---------------------------
GOOG | 09:00 |  200 | 30.9
GOOG | 09:15 | 1200 | 30.9
GOOG | 09:30 |	    |	
GOOG | 09:45 |	    |	
IBM  | 09:00 | 100  | 36.0
IBM  | 09:15 |	    |	
IBM  | 09:30 | 600  | 36.2
IBM  | 09:45 |      |		

/ can also join using left join
/ rack lj select sum size, last price by sym, bucket xbar time.minute from trade
```

```q
/6 update null size with 0

update 0^size from rack # select sum size, last price by sym, bucket xbar time.minute from trade

sym  | time  | size | price
---------------------------
GOOG | 09:00 |  200 | 30.9
GOOG | 09:15 | 1200 | 30.9
GOOG | 09:30 |	  0 |	
GOOG | 09:45 |	  0 |	
IBM  | 09:00 |  100 | 36.0
IBM  | 09:15 |	  0 |	
IBM  | 09:30 |  600 | 36.2
IBM  | 09:45 |    0 |	
```

```q
/7 update null price with last price

update fills price by sym from update 0^size 
from rack # select sum size, last price by sym, 
bucket xbar time.minute from trade

sym  | time  | size | price
---------------------------
GOOG | 09:00 |  200 | 30.9
GOOG | 09:15 | 1200 | 30.9
GOOG | 09:30 |	  0 | 30.9	
GOOG | 09:45 |	  0 | 30.9	
IBM  | 09:00 |  100 | 36.0
IBM  | 09:15 |	  0 | 36.0	
IBM  | 09:30 |  600 | 36.2
IBM  | 09:45 |    0 | 36.2	
```

<a name="alignment"></a>
### 🔵 33.3 Alignment

```q
/ align 2 sets of asynchronous timeseries data where the timestamps dont match
/ could be aligning different syms, ie, GOOG and IBM
```

```q
/ quick recap on AJ

\l fakedb.q
makehdb[`:hdb;10;1000; 1000]
\l hdb

trades1:select time, sym, price, size from trades where date in 2014.04.21

time                       | sym  | price | size
-------------------------------------------------
2014-04-21T08:00:44.437000 | AAPL | 25.34 | 1785
2014-04-21T08:04:41.246000 | AAPL | 25.34 |  427
2014-04-21T08:04:47.586000 | AAPL | 25.34 | 1528
...

quotes1: select time, sym, bid, ask from quotes where date in 2014.04.21

time                       | sym  | bid   | ask
-------------------------------------------------
2014-04-21T08:05:56.520000 | AAPL | 25.34 | 25.35
2014-04-21T08:18:39.592000 | AAPL | 25.34 | 25.35
2014-04-21T08:23:23.765000 | AAPL | 25.330| 25.38
...

aj[`sym`time;trades1;quotes1]

/ aj will make an exact match on sym, then asof match on time
/ pulls in prevailing bid or ask from latest time

time                       | sym  | price | size | bid   | ask
----------------------------------------------------------------
2014-04-21T08:00:44.437000 | AAPL | 25.34 | 1785 |	 |	
2014-04-21T08:04:41.246000 | AAPL | 25.34 |  427 |	 |	
2014-04-21T08:04:47.586000 | AAPL | 25.34 | 1528 |	 |	
2014-04-21T08:08:09.192000 | AAPL | 25.35 | 8136 | 25.34 | 25.35
2014-04-21T08:11:23.934000 | AAPL | 25.35 | 8945 | 25.34 | 25.35
2014-04-21T08:12:58.862000 | AAPL | 25.35 | 6577 | 25.34 | 25.35
```

```q
/ what if we want to align prices and cum vol of 2 diff sym?
/ for ex, compare price and vol of AAPL and GOOG

apple: select time, Appleprice: price, AppletoVol: sums size from trades1 where sym in `AAPL

/ need to use sums to get cum vol at specific time + price
/ if you just use sum, it will simply add together all sizes

time                       | Appleprice | AppletoVol
----------------------------------------------------
2014-04-21T08:00:44.437000 | 25.34      | 1785
2014-04-21T08:04:41.246000 | 25.34      | 2212
2014-04-21T08:04:47.586000 | 25.34      | 3740

google: select time, Googleprice: price, GoogletoVol: sums size from trades1 where sym in `GOOG

time                       | Googleprice | GoogletoVol
------------------------------------------------------
2014-04-21T08:02:44.628000 | 41.36       | 493
2014-04-21T08:07:14.804000 | 41.36       | 817

aj[`time;apple;google]

time                       | Appleprice | AppletoVol | Googleprice | GoogletoVol
----------------------------------------------------------------------------------
2014-04-21T08:00:44.437000 | 25.34      | 1785	     |             |
2014-04-21T08:04:41.246000 | 25.34	| 2212	     | 41.36       | 493
2014-04-21T08:04:47.586000 | 25.34	| 3740	     | 41.36       | 493
2014-04-21T08:08:09.192000 | 25.35	| 11876      | 41.36       | 817
```

<a name="pivot"></a>
### 🔵 33.3 Pivoting

```q
/ pivoting used for swapping row values to column values

tab1: ([] sym:`GOOG`IBM`GOOG`APPL; time: 09:00 09:01 09:04 09:10; price: 30.1 28.2 30.2 42.3)

sym  | time  | price
--------------------
GOOG | 09:00 | 30.1
IBM  | 09:01 | 28.2
GOOG | 09:04 | 30.2
APPL | 09:10 | 42.3

/1 extract distinct syms (this will be your new column headers)
/ use exec to extract syms as a list

exec distinct sym from tab1

`GOOG`IBM`AAPL

/2 sort list in ascending order

colnames: asc exec distinct sym from tab1
`AAPL`GOOG`IBM

/3 add the sorted attribute

`s#`AAPL`GOOG`IBM

/4 Exact dictionaries for sym!price for each time value that we have

exec sym!price by time from tab1

key   | value
--------------------
09:00 |	,`GOOG!,30.1
09:01 |	,`IBM!,28.2
09:04 |	,`GOOG!,30.2
09:10 |	,`APPL!,42.3

/5 populate dictionaries using colnames list
/ have to also name the time col

pivtab1: exec colnames#sym!price by time:time from tab1

time  | AAPL | GOOG | IBM
---------------------------
09:00 |	     | 30.1 |	
09:01 |	     |      | 28.2
09:04 |	     | 30.2 |	
09:10 |	42.3 |      |		

/6 forward fill the price column using fills function

pivtab1: fills exec colnames#sym!price by time:time from tab1

time  | AAPL | GOOG | IBM
---------------------------
09:00 |	     | 30.1 |	
09:01 |	     | 30.1 | 28.2
09:04 |	     | 30.2 | 28.2	
09:10 |	42.3 | 30.2 | 28.2	
```

<a name="profiling"></a>
## 🔴 34. Profiling
[Top](#top)

<a name="profile_one"></a>
### 🔵 34.1 Comparing Trading Vol vs Average Profile

```q
/ profiling compares activity for a specific time period against the average activity (profile) over a wider period
/ for example, compares trading vol on specific date vs average daily volume over a period

1. calc Average Daily Profile by dividing each day into time slices
2. sum trading activity in each time slice
3. creating a cumulative sum of full day
4. then averaging these cumulative sums
```

```q
/1 define date range

dts: (2014.04.22; 2014.05.22)
```

```q
/2 select cumulative size grouped by date, sym, and 5 min time buckets

p: select sum size by date, sym, 5 xbar time.minute from trades where date within dts

date      | sym  | minute| size
--------------------------------
2014-04-22| AAPL | 08:00 | 17377
2014-04-22| AAPL | 08:15 | 252
2014-04-22| AAPL | 08:20 | 8716
2014-04-22| AAPL | 08:25 | 2456

/ grouped by date, sym, minute
```

```q
/3 update p (size) to get cumulative sum for each day (cumulative for each 5 min bucket)

p: update sums size by date,sym from p

date      | sym  | minute| size
--------------------------------
2014-04-22| AAPL | 08:00 | 17377
2014-04-22| AAPL | 08:15 | 17629
2014-04-22| AAPL | 08:20 | 26345
2014-04-22| AAPL | 08:25 | 28801

/ notice not all time buckets are filled (8:05 missing)
```

```q
/4 calculate average volume (profile)

/ sum sizes for each sym and each time slice over date range
/ then divide by number of distinct dates
/ aka, over this date range, what is the total vol traded on avg for this 5 min window

p1: select avgcumulative: (sum size)% count distinct date by sym, minute from p

sym  | minute| avgcumulative
-----------------------------
AAPL | 08:00 |  5046.2
AAPL | 08:05 |  6925.8
AAPL | 08:10 | 10805.0
AAPL | 08:15 | 11583.8
```

```q
/5 build a rack 

/ rack = table of all distinct syms crossed with each 5 min time buckets
/ require start and end times

start: min exec minute from p1
end: max exec minute from p1

/ p1 is the table with avgcum vol for each time bucket
/ extracts the min/max time where there is an execution
/ start = 08:00
/ end = 16:25

rack: (select distinct sym from p) cross ([] minute: start+00:05*til 1+`int$(end-start)%00:05)

sym  | minute
-------------
AAPL | 08:00
AAPL | 08:05
AAPL | 08:10
AAPL | 08:15
```

```q
/ breaking down the syntax:

start+00:05*til 1+`int$(end-start)%00:05

end-start
/ 8:25

(end-start)%00:05
/ 101 buckets

til 1 + `int$(end-start)%00:05
/ 0 1 2 3...101

00:05*til 1+`int$(end-start)%00:05
/ 00:00, 00:05, 00:10
/ 5 min buckets

start+00:05*til 1+`int$(end-start)%00:05
/ 08:00, 08:05, 08:10...
```

```q
/ 6 finally, join the rack with the table of cumulative averages

rack lj p1

sym  | minute| avgcumulative
----------------------------
AAPL | 08:00 |  5046.2
AAPL | 08:05 |  6925.8
AAPL | 08:10 | 10805.0
AAPL | 08:15 | 11583.8
AAPL | 08:20 | 14399.6
AAPL | 08:25 | 18444.8
```

<a name="profiling_func"></a>
### 🔵 34.2 Creating Functions for Comparing Profiles

```q
\l fakedb.q
makehdb[`:hdb;60;1000;1000]
\l hdb
```

```q
/1 write function that calculates avg cum vol in 5 min time buckets

adv: {[startdate;enddate;bucketsize]

/2 extract the bucketed totals
p: select sum size by date,sym, bucketsize xbar time.minute from trades where date within (startdate;enddate);

/3 make total cumulative
p: update sums size by date, sym from p;

/4 calc avg value across all dates
p: select avgcumulative: (sum size)%count distinct date by sym, minute from p;

/5 rack the data
start:min exec minute from p;
end: max exec minute from p;
rack:(select distinct sym from p) cross ([] minute: start+bucketsize*til `int$(end - start)%bucketsize);

/6 return the racked data and fill forward
update fills avgcumulative by sym from rack lj p}
```

```q
/7 call arguments

adv[2014.04.22;2014.05.22;5]

sym  | minute| avgcumulative
----------------------------
AAPL | 08:00 |  5046.2
AAPL | 08:05 |  6925.8
AAPL | 08:10 | 10805.0
AAPL | 08:15 | 11583.8
AAPL | 08:20 | 14399.6
AAPL | 08:25 | 18444.8
```

```q
/8 add comparison by joining on cumulative size data for specified date

adv[2014.04.22;2014.05.22;5] lj update sums size from select sum size by sym, 5 xbar time.minute from trades where date = 2014.05.22

sym  | minute| avgcumulative | size
------------------------------------
AAPL | 08:00 | 5046.2	     |
AAPL | 08:05 | 6925.8	     | 4618
AAPL | 08:10 | 10805.0       |	
AAPL | 08:15 | 11583.8       | 11955
AAPL | 08:20 | 14399.6       | 12151
AAPL | 08:25 | 18444.8       | 19066
```

```q
/9 fill forward to remove any blank values in the size column

update fills size from adv[2014.04.22;2014.05.22;5] lj update sums size from select sum size by sym, 5 xbar time.minute from trades where date = 2014.05.22

sym  | minute| avgcumulative | size
------------------------------------
AAPL | 08:00 | 5046.2	     |
AAPL | 08:05 | 6925.8	     | 4618
AAPL | 08:10 | 10805.0       | 4618
AAPL | 08:15 | 11583.8       | 11955
AAPL | 08:20 | 14399.6       | 12151
AAPL | 08:25 | 18444.8       | 19066
```
```q
/10 add comparison column that divides the size on that day over the entire date range

update sizetoADV: size%avgcumulative from update fills size from adv[2014.04.22;2014.05.22;5] lj update sums size from select sum size by sym, 5 xbar time.minute from trades where date = 2014.05.22

sym  | minute| avgcumulative | size  | sizetoADV
-----------------------------------------------
AAPL | 08:00 | 5046.2	     |       | 
AAPL | 08:05 | 6925.8	     | 4618  | 0.6668
AAPL | 08:10 | 10805.0       | 4618  | 0.4274
AAPL | 08:15 | 11583.8       | 11955 | 1.032
AAPL | 08:20 | 14399.6       | 12151 | 0.8438
AAPL | 08:25 | 18444.8       | 19066 | 1.033
```

```q
/11 combine everything together in one function

comparetoADV:{ [startdate;enddate;bucketsize;comparisondate]
  update sizetoAdv:size%avgcumulative from / lastly update to include comparison column
    update fills size from / fill forward to remove blanks
      adv[startdate;enddate;bucketsize] lj
        update sums size from select sum size by sym, bucketsize xbar time.minute from trades where date = comparisondate}
        
comparetoADV[2014.04.22;2014.05.22;5;2014.05.22]

sym  | minute| avgcumulative | size  | sizetoADV
-----------------------------------------------
AAPL | 08:00 | 5046.2	     |       | 
AAPL | 08:05 | 6925.8	     | 4618  | 0.6668
AAPL | 08:10 | 10805.0       | 4618  | 0.4274
AAPL | 08:15 | 11583.8       | 11955 | 1.032
AAPL | 08:20 | 14399.6       | 12151 | 0.8438
AAPL | 08:25 | 18444.8       | 19066 | 1.033
```

<a name="tradeanalysis"></a>
## 🔴 35. Trade Analysis
[Top](#top)

```q
/ case study to perform some PnL trade analysis
/ calc PnL of each trade at diff time points (before/after trade time)
/ assume every trade is a buy trade
/ will go to market at the trade price instead of the quoted price
```

```q
\l fakedb.q
makedb[1000;100000]

select from trades

time                       | sym  | src | price | size
--------------------------------------------------------
2021-11-19T08:00:00.531000 | DELL | N   | 21.7	| 4567
2021-11-19T08:00:00.754000 | MSFT | O   | 46.51	| 436
2021-11-19T08:00:01.007000 | NOK  | O   | 22.87	| 7915
2021-11-19T08:00:01.025000 | CSCO | O   | 35.77 | 783

/1 create copy of trade, but time coloumn shifted back 5 mins

select sym, time:time-0D00:05, priceplus5: price from trades

sym  | time                       | priceplus5
-----------------------------------------------
DELL | 2021-11-19T07:55:00.531000 | 21.7
MSFT | 2021-11-19T07:55:00.754000 | 46.51
NOK  | 2021-11-19T07:55:01.007000 | 22.87
CSCO | 2021-11-19T07:55:01.025000 | 35.77
```

```q
/2 join this onto original table using asof join
/ this gives current trade price along with the prevailing trade price 5 mins later

tab1:aj[`sym`time;trades;select sym, time:time-0D00:05, priceplus5: price from trades]

time                       | sym  | src | price | size | priceplus5
-------------------------------------------------------------------
2021-11-19T08:00:00.531000 | DELL | N   | 21.7	| 4567 | 21.7
2021-11-19T08:00:00.754000 | MSFT | O   | 46.51	| 436  | 46.51
2021-11-19T08:00:01.007000 | NOK  | O   | 22.87	| 7915 | 22.87
2021-11-19T08:00:01.025000 | CSCO | O   | 35.77 | 783  | 35.77
```

```q
/3 add pnl column by multiplying the difference in prices by size

update pnl:size*(priceplus5 - price) from tab1

time                       | sym  | src | price | size | priceplus5 | pnl
-------------------------------------------------------------------------
2021-11-19T08:00:00.531000 | DELL | N   | 21.7	| 4567 | 21.7       | 274.02
2021-11-19T08:00:00.754000 | MSFT | O   | 46.51	| 436  | 46.51      |   0
2021-11-19T08:00:01.007000 | NOK  | O   | 22.87	| 7915 | 22.87      | -316
2021-11-19T08:00:01.025000 | CSCO | O   | 35.77 | 783  | 35.77      | 0
```
```q
/4 generalize this by shifting the time by a specified number of seconds

sel: {select sym, time.second-x, price from trades}
sel 10

sym  | second   | price
------------------------
DELL | 07:59:50	| 21.7
MSFT | 07:59:50	| 46.51
NOK  | 07:59:51	| 22.87
CSCO | 07:59:51	| 35.77
```

```q
/5 rename price col using xcol to plus10

sel: {(`sym`second,`$"PLUS",string x) xcol select sym, time.second-x, price from trades}
sel 10

sym  | second   | PLUS10
------------------------
DELL | 07:59:50	| 21.7
MSFT | 07:59:50	| 46.51
NOK  | 07:59:51	| 22.87
CSCO | 07:59:51	| 35.77
```

```q
/ this however, doesnt work with negative values
/6 so need to add an if/else statement
/ also use abs x to take absolute value of x

sel: {(`sym`second,`$$[x<0;"MINUS";"PLUS"],string abs x) xcol select sym, time.second-x, price from trades}
sel -10

sym  | second   | MINUS10
------------------------
DELL | 07:59:50	| 21.7
MSFT | 07:59:50	| 46.51
NOK  | 07:59:51	| 22.87
CSCO | 07:59:51	| 35.77
```

```q
/7 now can use this function in the asof join

aj[`sym`second;select sym, time.second, price, size from trades;sel 300]

sym  | second   | price | size | PLUS300
-----------------------------------------
DELL | 08:00:00 | 21.7	| 4567 | 21.76
MSFT | 08:00:00	| 46.51	| 436  | 46.51
NOK  | 08:00:01	| 22.87	| 7915 | 22.83
CSCO | 08:00:01	| 35.77	| 783  | 35.77
```

```q
/8 retrieve new cols for prices at different times

/ achieved by using the adverb over
/ takes trade table as first x arg, and list of time values as y arg
/ adds col if the trade price shifts forward by the first time in the list
/ then takes this new updated table as the next x arg, then next arg as next y

{aj[`sym`second;x;sel y]}/ [select sym, time.second, price, size from trades;10 20 30]

sym  | second   | price | size | PLUS10 | PLUS20 | PLUS 30
-----------------------------------------------------------
DELL | 08:00:00 | 21.7	| 4567 | 21.76  | 21.76  | 21.76
MSFT | 08:00:00	| 46.51	| 436  | 46.51  | 46.51  | 46.46
NOK  | 08:00:01	| 22.87	| 7915 | 22.83  | 22.83  | 22.87
CSCO | 08:00:01	| 35.77	| 783  | 35.77  | 35.77  | 35.78
```


<a name="creatingrandomtable"></a>
## 🔴 36. Creating Tables with Random Data
[Top](#top)

```q
/ lets create table for sym A, random times, and random prices
/ assume 100 rows
```

1. Generate 100 random times in a 6 hour period

```q
n:100

n?06:00
05:11u;00:49u;01:56u;04:57u;03:27u

/ add 8 hours to time starts at 08:00

08:00+n?06:00
08:48u;09:06u;09:53u;11:06u;11:22u

/ then sort by ascending

asc 08:00+n?06:00
08:00u;08:10u;08:20u;08:25u;08:28u
```

2. Generate 100 sequential prices

```q
/ prices generally only move up or down in a limited range
/ assume price moves up or down by -0.1 0 0.1 
/ generate list of random values from this set

n? -0.1 0 0.1 
0 -0.1 0.1 0.1 -0.1 -0.1 -0.1

/ then take running sums to make movement consecutive

sums n? -0.1 0 0.1 
0.1 0 0.1 0.2 0.3 0.2 0.1 0.2

/ finally, offset by some base value (say, 40)

40+sums n? -0.1 0 0.1 
40 40.1 40 39.9 39.8 39.9 40 40.1
```

3. Putting it all together

```q
t: ([] sym:`A; time: asc 08:00+n?06:00; price: 40+ sums n? -0.1 0 -.2)

sym    | time  | price
-----------------------
A      | 08:04 | 39.9
A      | 08:05 | 39.7
A      | 08:08 | 39.6
A      | 08:15 | 39.6
A      | 08:18 | 39.6
```

```q
/ bucket by hours

select by time.hh from t

hh	sym	time	price
-----------------------------
8	A	08:56	38.7
9	A	09:59	37.1
10	A	10:55	35.3
11	A	11:57	33.5
12	A	12:59	32.6
13	A	13:51	31.30
```

<a name="bottom"></a>
