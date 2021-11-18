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

## 5. [Lists Problem Set](#list_problemset)

## 6. [Primitive Operations](#primitive_header)
1. [Addition](#add_list)
2. [Comparing Lists](#compare_lists)
3. [Equal and Match Differences](#match_diff)
4. [Basic Operations](#basic_operations)
5. [Division Remainders Mod](#mod_operations)
6. [Running Sums/Moving Windows](#running_sums)
7. [Contain](#contain_ops)
8. [Except](#except_ops)
9. [Inter](#inter_ops)
10. [Distinct](#distinct_ops)
11. [Reverse](#reverse_ops)
12. [Upper/Lowercase](#uppercase_ops)

## 7. [Primitive Operations Problem Set](#primitive_problemset)

## 8. [Dictionary](#dict_header)
1. [Constructing a Dictionary from Lists](#dict_from_list)
2. [Retrieving values](#retrieve_dict)
3. [Index Retrieve](#index_retrieve_dict)
4. [Take](#take_dict)
5. [Drop](#drop_dict)
6. [Upsert](#upsert_dict)
7. [Multi Key Dictionaries](#multi_key_dict)
8. [Repeat Keys](#repeat_key_dict)
9. [Find Operator](#find_dict)
10. [Dictionary Operators](#dict_opt)

## 9. [Dictionary Problem Set](#dict_problemset)

## 10. [Functions](#functions_header)
1. [Defining & Calling Functions](#define_func)
2. [Anonymous Function](#anon_function)
3. [Implicit Argument](#implicit_argu)
4. [Local vs Global Variables](#local_global_variables)
5. [Projected Functions](#projected_func)
6. [If True Statements](#iftrue_state)
7. [If True/Else Statements](#iftrue_else_state)
9. [Adding Conditional Branch Pair](#add_cond_branch)
10. [Do Loops](#do_loop)
11. [While_Loops](#while_loop)
12. [Multi Condition While Loops](#multi_cond_while_loop)

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
9. [Retrieving Values from Keyed Table](#retrieve_value_keys)

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
0 +/ 1 2 3
```
1 2 3
* / means over
* execute "over" entire list

```q
(*/) 2 # 5
```
25
* take 2 values from 5 = 5 5
* multiply 5 x 5 = 25

<a name="scan_intro"></a>
### 🔵 1.9 Scan
* scan is similar to over /, but instead of returning the final result, returns all values

```q
(+\) 1 + 0 1 2 3
```
1 3 6 10

<a name="larger_intro"></a>
### 🔵 1.10 Larger

```q
4 | 5
```
5
* | is called style or bar
* returns the larger of the two operants

```q
(|/) til 10
```
9
* find the largest value over the list

```q
max 10 20 30
```
30
* return the largest value over the list

<a name="smaller_intro"></a>
### 🔵 1.11 Smaller

```q
10 & 2
```
2
* the & is called amper
* chooses the lesser of the 2

```q
(&/) til 10
```
0
* return the smallest value over the list

```q
min 10 20 30
```
10
* return the smallest value  in this list

<a name="count_intro"></a>
### 🔵 1.12 Count

```q
count (til 6; 10 20 30)
```
2
* counted 2 lists

```q
count each (til 6; 10 20 30)
```
6 3
* count each will count the number of values in each list

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
```Q

k: 1 2 3 4

2_k
3 4

/ dropS the first 2 values from list k

-2_k
1 2

/ drops the last 2 values from list k

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

3 cut l
(1 2 3; 4 5 6)

/ cuts list into elements of 3

1 4 cut l
(2 3 4; 5 6)

/ first element = drop all elements from this and before (1)
/ 2nd element = cut after this (4)

2 3 cut l
(3; 4 5 6)

/ drop all elements from 2 and before (1, 2)
/ cut after 3
```


<a name="pluscolon"></a>
### 🔵 1.15 +:

```q
x+:1
/ is the same as
x:x+1
```

```q
x*:3
/ is the same as
x:x*3
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
### 🔵 1.17 Signum

```q
/ Signum conveys whether a value is positive, negative, or 0

prices: 3 2 2 1 5
deltas prices
3 -1 0 -1 4

/ deltas = difference between each element

signum deltas prices
1 -1 0 -1 1

/ signum shows if element is positive, negative or 0

tickdirection: {signum deltas[first x;x]}
tickdirection prices

```

<a name="cross_operator"></a>
### 🔵 1.18 Cross 

```q
x cross y
/ cross returns all possible combinations of x and y
/ note - does NOT multiply or add

1 cross 3 4
1 3
1 4

/ x(1) to y(3)
/ x(1) to y(4)
  
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
/ also works on tables

s:`IBM`MSFT`AAPL
v: 1 2

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
```q
/ casting strings to sym

"S" $ "a","b","c"
`abc

/ use capital "S" to cast to sym
/ or can also use `
```

```q
/ Converting syms to strings 

string `abc
"abc"

/ sym to string, simply use "string" function
```

```q
/ casting int to dates

`date$2
2000-01-03d

/ 2nd day of the millennia
```

```q
/ casting int to time

`time$2
00:00:00.002t

/ 2 + 00:00:00.000
```

```q
/ casting int to month

`month$2
2000.03m

/ KDB time starts at 2000.01.01 
/ 2 + 2000.01.01
```

```q
/ casting int to minute

`minute$2
00:02

/ takes 2 + 00:00
```

```q
/ casting int to seconds

`seconds$2
00:00:02
```

```q
/ casting to booleans

`boolean$9
1b

/ casting a boolean will always be true (1b), unless its 0

`boolean$0
0b
```
```q
/ converting list of syms to string

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
### 🔵 4.8 Nested Lists

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

NL [ 0 2]
10 20 30 40 50
`pp`qq`rr

/ So think of list NL as 3 separate lists.
/ Retrieve index location 0 and 2, so returned the first and 3rd list

NL [0][0]
10

/ retrieves index position 0 (first list = list L) 
/ and the first value from that list (index location 0)
```

<a name="matrix_list"></a>
### 🔵 4.9 Matrix

m: (10 20 30; 40 50 60; 70 80 90)

0|1|2
-|-|-
10| 20| 30
40| 50| 60
70| 80| 90

* when retrieving in a matrix, always go ROW, then COLUMN

```q
m[1; ]
```
40 50 60
* takes index 1 location (2nd row)

```q
m[ ; 1]
```
20 50 80
* ignores row (blank), retrieves index 1 location for column (2nd column)


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

raze t:(1 2; 3 4 5)
1 2 3 4 5 

/ collapses 1 level of nesting and joins all items together
```

```q
b: (1 2; (3 4; 5 6); 7; 8)
1 2
3 4
5 6
7
8

raze/[b]
1 2 3 4 5 6 7 8

/ using raze/[x] will flatten all levels
```

```q
string `a`b`c
"a","b","c"

raze string `a`b`c
"abc"
```

<a name="raze_intro"></a>
### 🔵 4.15 Union Lists

```q
1 2 3 union 3 4 5
1 2 3 4 5 

/ union returns only the distinct elements in both lists
```

<a name="raze_intro"></a>
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

p: 100 200 300 400 500 600
t: "say hello world to bob"
m: (1 2 3; 10 20 30; 100 200 300)

**Retrieve first 3 items from p**
```q
3#p
100 200 300
```

<hr>

**🔵 5.4 From t, retrieve the list "sold"**

```q
t[0 8 6 14]
"sold"

/ you are retrieving characters from their index position
```

<hr>

**🔵 5.5 Create the nested list ("shoot";"bob") by indexing into t**

```q
t?"shoot"
0 4 8 8 16
```

```q
t? "bob"
19 8 19
```
```q
t(0 4 8 8 16; 19 8 19)
("shoot";"bob")

/ you are finding the index locations of those chars from list t
/ then retrieving those index positions (letters) to spell out 
```

<hr>

**🔵 5.6 Change the last number in p to 1000**

```q
p[5]: 1000

/ upsert. find index location 5, replace value with 1000
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
3 msum 1

/ moving window sum of 3
```
```q
3 mmax l

/ moving window max of 3
```

<a name="contain_ops"></a>
### 🔵 6.7 Contain

```q
5 in 1 2 3 4
0000b

/ is x in y? no, so 0
```

<a name="except_ops"></a>
### 🔵 6.8 Except

```q
1 2 3 4 except 3
1 2 4

/ return the list except 3
```

<a name="inter_ops"></a>
### 🔵 6.9 Inter

```q
1 2 3 inter 2 3 4
2 3

/ inter returns values occuring in both lists
```

<a name="distinct_ops"></a>
### 🔵 6.10 Distinct

```q
distinct `a`a`b`b`c`c
a b c

/ distinct only returns distinct values
```

<a name="reverse_ops"></a>
### 🔵 6.11 Reverse
```q
reverse 1 2 3
3 2 1
```

<a name="uppercase_ops"></a>
### 🔵 6.12 Upper/Lowercase

```q
upper "adsf"
lower "ADSF"

ADSF
adsf
```

<a name="uppercase_ops"></a>
### 🔵 6.13 Timing and Performance
```q

n: 1000000

a:n?100f
b:n?100f

/ a and b are lists of a million floats

\t r1:a+b
1

/ time took less than 1 millisecond

\t:100 r1:a+b
120

/ run it 100x
/ time still only 120 ms
```

<hr>

<a name="primitive_problemset"></a>
## 🔴 7. Primitive Operations Problem Set
[Top](#top)

**🔵 7.1 Find index location for a string of chars**

```q
"hello ryan where is ryan" ss "ryan"
6 20

/ ss = finds the index location
```

<hr>

**🔵 7.2 replace "ryan" with "john"**

```q
ssr["hello ryan where is ryan";"ryan";"john"]
hello johhn where is john

/ this is similar to excel search and replace function
```

<hr>

**🔵 7.3 Find the number of days in 2004**
```
2005.01.01-2004.01.01
366

```

<hr>

**🔵 7.4 Given list L and K, find the common numbers in both lists**
l: 7 5 13 20 19 17 30
k: 7 17 200 300 400 1000

```q
l inter k
7 17
```

<hr>

**🔵 7.5 Find the sum of the first 5 numbers in l**
```q
sum 5#l
64
```

<hr>

**🔵 7.6 Find the result whhen you remove the last 2 items from k**
```q
-2_k
7 17 200 300
```

<hr>

**🔵 7.7 Return only numbers in l that are wholly divisible by 5**
```q
l mod 5
2 0 3 0 4 2 0
```

```q
l where 0 = l mod 5
5 20 30

/ show list l where l divide by 5 = 0
```

<hr>

**🔵 7.8 Subtract the average of list l from max value in list k**
```q
max[k] - avg [l] 
984.14
```

<hr>

**🔵 7.9 Generate list p of 1000 random integers between 0 and 100. Find all values in p that are square numbers**
```q
p: 1000?100
a: sqrt p

/ a will contain both ints and floats
```

```q
a = `int$a

/ cast a as an integer (whole number)
```
```q
p where a=`int$a

/ return value in p where a = whole number
```
```q
count p where a=`int$a

/ count the number of times p is a whole number
```

<hr>

<a name="dict_header"></a>
## 🔴 8. Dictionary
[Top](#top)

```q
/ A dictionary is a mapping between a list of keys and a list of values of the same length
/ left of ! = list of keys
/ right of ! = list of values
```

<a name="dict_from_list"></a>
### 🔵 8.1 Constructing a Dictionary from Lists
```q
k:`apple`plum
v:`green`purple
d:k!v

key  | value
--------------
apple| green
plum | purple
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

/ all 3 syntax work for retrieving values in a dictionary
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
(enlist`a)#d
1

/ have to use enlist when retrieving a single item from dictionary
```

<a name="drop_dict"></a>
### 🔵 8.5 Drop

```q
/ drop used to delete key/values in dictionaries

2_d

key | value
-----------
C   | 3

/ drop first 2 rows from dictionary d
```

```q
d: `a`b`c ! 1 2 3

key | value
----------
a   | 1
b   | 2
c   | 3

`b _ d

/ drop key `b and its value 3 from dict

key | value
----------
a   | 1
c   | 3

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

/ adding new row via join

dict,(`delta`echo)!(10 11 12;13 14 15)

/ however, to update the underlying table, need to use join assign ,:

dict,:(`delta`echo)!(10 11 12;13 14 15)

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 7 8 9
delta   | 10 11 12
echo    | 13 14 15

/ amending key/values via indexing

dict[`charlie]: 100 200 300

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 100 200 300
delta   | 10 11 12
echo    | 13 14 15

/ to add a single row (need to use enlist!)

dict,:(enlist `golf)! enlist 10

key     | value
---------------
alpha	| 1 2 3
bravo	| 4 5 6
charlie | 100 200 300
delta   | 10 11 12
echo    | 13 14 15
golf    | 100

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
### 🔵 8.9 Find Operator ?

```q
dict: `a`b`c`d!1 5 8 12

dict?12
`d

/ ? find operator
/ lookup value 12, returns key
```

<a name="dict_opt"></a>
### 🔵 8.10 Dictionary Operators
```q
d: `a`b`c ! 1 2 3

sum d
6

avg d
2

neg d
key|value
--------
a  | -1
b  | -2
c  | -3

/ turns all values negative

d%100
key|value
---------
a  |0.01
b  |0.02
c  |0.03

/ divides all values by 100
```
```q
Adding / Joining Dictionaries

d1:`a`b`c!1 2 3
d2:`a`b`c!1 2 3

d1+d2
d1,d2

key|value
--------
a  | 2
b  | 4
c  | 6
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

**🔵 4. Create dictionary d2, only containing values of p q r from dictionary d**
```q
d2:`p`q`r#d

key|value
---------
p  | 2
q  | 20
r  | 40

/ use # take function to take values of p q r from dictionary d
```

**🔵 5. Add common elements in d2 and d, only return common keys and values**
```q
d+d2

key|value
---------
p  | 4
q  | 40
r  | 80
s  | 100
u  | 200

/ adds all values together where there is a match in keys

d inter d2
2 20 40

/ dict inter dict will return values occuring in both dicts

key[d] inter k[d2]
`p`q`r

/ have to use key[dict_name] inter key[dict2_name] to return keys in both dict

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

/ dictionary + condition = examines values as booleans, returns as true/false

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
f: { [a] a * a}
f [3]
9

/ [a] = defines the argument
/ f[3] or f@3 calls the function with a=3
```

```q
add: { [a;b] a + b}
add [3;5]
8

/ multi argument function
/ [a;b] = defines first, second argument
/ a+b = statement
```
```q
/ the answer returned is the LAST expression evaluated in function

f:{[arg1;arg2;arg3] t:arg1*arg2*arg3; t*2}
t[1;2;3]
12

/ 1*2*3 = 6
/ 6*2 = 12
```
```q
/ can supress the function by adding ; to end 

f:{[arg1;arg2;arg3] t:arg1*arg2*arg3; t*2;}
t[1;2;3]
-

/ nothing returned
```
```q
/ can force an output by adding semi colon :

f:{[arg1;arg2;arg3] t:arg1*arg2*arg3; :t*2; t+3}
t[1;2;3]
12

/ semi colon in front of 2nd expression so it will force that output
/ colon halts everything after 

/ built in plus operator

+[1;2]
3

```

### 🔵 10.2 Types of Functions

```q
/ niladic (accept no arguments)

f:{[] 1+2+3}
f[]
6

/ monadic (accepts 1 argument)

f:{[arg1] arg1+10}
f[2]
12

/ implicit (up to 3 arguments)

f:{x+10}
f[2]
12

/ don't need to declare argument; x will be first parameter passed through function

/ diadic (accepts 2 arguments)

f:{[a;b] a*b}
f[2;4]
8

/ alternatively can be implicit:

f:{x*y}
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
{[a] a*a}6
36

/ you dont assign variable 
/ simply call the argument outside the function { } 
```

<a name="implicit_argu"></a>
### 🔵 10.3 Implicit Argument

```q
{x*x}5
25

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

/ error because you can't skip the y. if only 2 implicit arguments, need to use x, y
```

<a name="local_global_variables"></a>
### 🔵 10.4 Local vs Global Variables
```q
{a:1; b:2; a+b*x} [12]
25

/ calling in x = 12 (implicit argument)
/ 1 + 2 * 12 
/ a and b are locally defined variables within the function
/ will NOT work if you try to recall variable a or b outside the function
```

```q
d:10
f:{d+x}
f [1]
11

/ assign global variable D to 10 (outside the function)
/ f[1] calls in 1 for x (implicit argument)
/ = 10 + 1 = 11
```

```q
d: 10
g: {d:20; d+x}
g [1]
21

/ d:20 is a locally defined variable
/ local takes priority over global variable of 10
/ = 20 + 1 = 21
```

<a name="projected_func"></a>
### 🔵 10.5 Projected Functions
```q
raise: {x xexp y}
raise [10; 2 3 4]
100 1000 1000f

/ calls x = 10 and y = 2 3 4
```

```q
g: raise [10; ]
g 1 2 3
10 100 1000

/ creates a projection of the original raise function
```
```q
f:{x*y}
f[4;5]

/ let's assume y will always stay as 5 and only x will change

g:f[;5]
g[3]
15

/ set y = 5
/ now when you call g[3], x=3 while y stays the same
/ g becomes a nomaic parameter

g
{x*y}[;5]

/ if you call g, you'll see it contains original expression
/ and the set parameters are shown in [ ]
```



<a name="iftrue_state"></a>
### 🔵 10.6 If Statements

```q
if [10>3; a:11; show a*10]
110

/ since the first condition is true, execute all statements that follow
```

```q
if[10>3; a:11; show a*10; show "hello"]
110
"hello"

/ as long as the first condition is true, execute all following statements
```

```q
if[10; show "true"]
"true"

/ integers default to TRUE (1b)
/ 0 default to FALSE (0b)
/ since 10 is an int, and int will default to 1b (true)

```

```q
if[count(); show "true"]

/ nothing shows, since count empty list = 0, hence false
```

<a name="iftrue_else_state"></a>
### 🔵 10.7 If/Else Statements

```q
$[1b; show "true"; show "false"]
true

/ always starts with $[ ] 
/ if first condition true, then show second condition. else, show third condition
/ here the first condition is the false boolean
```

```q
$[100>1; [show "message"; `a];`b]
"message"
`a

/ since true, show everythign  in the [ ]
```

<a name="add_cond_branch"></a>
### 🔵 10.8 Adding Conditional Branch Pair
```q

/ $[condition1; expr1;[cond2;expr2; ..];...;falseexpr

/ if condition is true, evaluate all the following expressions
/ finishes with condition to be executed if all conditions are false

/ if true condition encountered, no further condition evaluated

a:5
$[a<2; 1; a<4; 2; a<6; 3; a<8; 4; 20]
3

/ once 5 < 6; returns 3, then stops evaluating rest of function

/ multiple expressions

$[a<2; [b:10; c:11]; [b:98; c:99]]

/ if cond true, then evaluate first expression
/ otherwlse evaluate last condition
```

```q
{$[x < 0; `negative; x=0; `zero; `positive]}0
`zero

/ using implicit argument x =0
/ 0 doesnt equal 0, so false. goes to 2nd condition, x=0
/ x = 0 this begins another conditional branch
/ since x-0 is true, returns first condition (zero)
```

```q
{$[x < 0; `negative; x=0; `zero; `positive]}2
`posititve

/ 2 = x and since 2 isnt less than 0, false. 
/ 2 does NOT equal x=0, so false again
/ skips first condition, returns second condition (positive)
```

<a name="do_loop"></a>
### 🔵 10.9 Do Loops
```q
do[3;show "hi"]
hi
hi
hi

/ repeats loop x number of times
```

```q
f:{avg x xexp 1000?2}
\t do[1000;f]
0

/ time the loop 1000x on function f
```

<a name="while_loop"></a>
### 🔵 10.10 While Loops
```q
/ while will execute a statement x number of times until statement is no longer true
```
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

```q
a:1
b:2
while[(a<10); a:a+1; b:b+1; show enlist b,a]

key|value
----------
3  | 2
4  | 3
5  | 4
6  | 5

/ a = 1; a becomes 1+1(2)
/ b = 2; b becomes 2+1(3)
/ show enlist shows b and a in a clean list
/ stop running this loop when first condition becomes false
```

<a name="multi_cond_while_loop"></a>
### 🔵 10.11 Multi Condition While Loops

```q
/ sum all values > 100 using while loop

d: 100?100
i: 0
r1: 0

/ d = list of 100 random numbers
/ i = iterative counter (goes from 0-100)
/ r1 = result of while loop

while [i<count d; if [d[i]>50;r1+:d[i]]; i+:1]

/ while i is less than the count of the list (d)
/ if value of list at index i is greater than 100
/ then add this to the value of the result (r1)
/ then go onto next iteration (i+1)
/ remember, WHILE LOOPS -> if first argument is TRUE, execute all arguments that follow

HOWEVER, much faster using vector operations:

r2: sum d where d > 50

/ so use vector operations whenever possible
/ also a lot more flexible:

max sum d where d>50
min sum d where d>50
avg sum d where d>50

```

```q
a:1
b:2
while[(a<10) and (b<3); a:a+1; b:b+1; show enlist b,a]

/ if you have 2 conditions, must use ( ) as KDB reads right to left
/ 2 < 3, yes. 1< 10, yes
/ so a = 1+1 = 2 and b=2+1 = 3
/ shows 3 2
/ 3 is not < 3, so false. stops running
```

```q
isprime:{if[x<2; 0b]; a:2; while[a<x; if[(x mod a)=0;0b]; a+:1]; 1b}

/ if x = 1
/ x(1) < (2) (TRUE) so returns 0b (not prime)\

/ if x = 4
/ x(4)< 2 (FALSE), skip 0b statement, moves onto a:2
/ a(2) < x(4)? (TRUE), x mod a = 4 mod 2 = 0 (no remainders if you divide 4 by 2). (TRUE), so returns 0b (not prime)\

/ if x = 7
/ x(7) < 2 (FALSE), skip 0b
/ a(2) < x(7) (TRUE), x mod a = 7 mod 2 = 1 (FALSE), so returns 1b (TRUE)
```

```q
findprime: { [n] r:(); a:1; while [a<n; if[isprime[a];r,:a]; a:a+1];r}
findprime 10 

2 3 5 7
/ n = single argument
/ r () = empty list
/ a starts from 1, if a (1) < n (10) TRUE, append a to list r
/ go through every value of a, and add to list r
```

### 🔵 10.12 Function within a Function LAMBDA 

```q

f:{x*x}
g:{10+f[x]}
g[2]
14

/ 2 becomes x, 10 + 4 = 14

/ can define a function within a function inline

z:{f:{x*x};f[x] + 10}
z[2]
14

/ but doesn't need to be defined

{{x*x}[x] + 10}

/ this is called a lambda
/ lambda = a pair of curly brackets enclosing optional argument expressions separated by semicolons

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
```q
/ create a function that converts sym `welcome to a string and replaces me with ME

{ssr[string x;y;z]}[;"me";"ME"] `welcome
"welcoME"

/ this function converts all syms to strings 
/ then ssr string search replace the "me" with capital "ME"

/ do the same with list of syms

{ssr[string x;y;z]}[;"me";"ME"] each `welcome`home`mermaid
"welcoME"
"hoME"
"MErmaid"

/ need the adverb EACH to iterate through each sym

/ can also be done by defining function

f:{ssr[string x;y;z]}
f[;"me";"ME"] each `welcome`home`mermaid
"welcoME"
"hoME"
"MErmaid"
```

<hr>

<a name="func_problem_set"></a>
## 🔴 11. Functions Problem Set
[Top](#top)

**🔵 11.1 Create a function volc that accepts 2 arguments (r and h), that returns the volume of the given volc [2;3]**

```q
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

**🔵 11.2 Write function sph that takes radius and returns the area and volume**

```q
/ v = 4/3 * pi * r^3
/ a = 4 * pi * r^2

sph: { [r] pi:-4*atan -1; a:(4%3)*pi*r xexp 3; v:4*pi*r xexp 2; `area`volume ! (a;v)}
sph[1]

key    | value
----------------
area   | 4.18
volume | 12.56

/ define argument [r]
/ define variable pi with formula
/ define variable a with formula
/ define variable v with formula
/ show dictionary with symbols `area `volume against values a and v
```

**🔵 11.3 Create function setc that takes one argument and sets the global value c to that argument**
```q
setc: {c::x}
setc[10]
c

10
/ setc 10 = setting x = 10 (implicit variable)
/ since x = 10, and you've set c as the global variable to x, then c = 10

setc `hi
c
`hi

/ you set setc = `hi, so c = x = `hi
```

**🔵 11.4 Given raise:{x xexp y}, create function that is projection of the raise. Ex, root[9] = 3**
```q
raise: {x xexp y}
root: raise[ ; 0.5]
root[9]
3

/ an embedded function is a function within another function
/ root function sets y as 0.5
/ so root 9 =x
```

**🔵 11.5 Convert all entries of list L to a string**
```q
l: (100;`price;1b)
string l
"100"
"price"
"1b"

/ l is a list of long, sym, and boolean
/ remember, mixed lists have to be contained in parathesis ( )
```

**🔵 11.6 Given the string, find and replace "cow" with "kangaroo"**

```q
st: "the cow jumped over the moon"
ssr [st; "cow";"kangaroo"]
"the kangaroo jumped over the moon"

/ ssr = string search replace.
/ syntax = ssr [listname + find this + replace with this]
```

**🔵 11.7 Create function sayHi that takes 2 arguments, first one name, second one age and behaves as follows:**
```q
/ sayHi["joe";90]
/ "hello 90 year old joe"
```
```q
sayHi:{[name;age] "hello ", string[age]," year old ", name}
sayHi["joe";90]
hello 90 year old joe

/ name and age are your arguments
/ "hello" and "year old" are simply lists of characters
/ you have to convert raw data values into strings, use , to concatenate the strings together
/ need to convert [age] to string
/ when you define argument "joe" have to use parathesis otherwise wont work
```

**🔵 11.8 I have a box of 7 eggs, find the median and average weight**
```q
eggs: 10 20 30 40 50 60 70

med eggs
40

avg eggs
40
```
<hr>

**🔵 11.9 I sold 2 boxes of eggs. 1 box had 10 eggs and i sold it for 50 each. the other box had 20 eggs and sold it for 100 each. find the average price paid per egg**

```q
10 20 wavg 50 100
83.3

/ wavg = weight average function
/ num1 num2 wavg value1 value2

```

**🔵 11.10 Generate list k of 10 random integers. Find the moving average with window size of 3**
```
k: 10?10
mavg[3;k]
8 4.5 6 5 6 5 5.33 4.33 5 4.67

/ Find the 3 largest numbers in list k

3#desc k
9 8 8 

/ take 3 of the largest from k, sort by desc

/ Find the difference between the successive elements of k

deltas k
8 -7 8 -4 -1 2 0 -5 7 -3
```

**🔵 11.11 Create function factw, using a loop to write a factorial function**
```q
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

**🔵 11.12 Re-create the factorial function as factp without using loops**
```q
factp:{prd 1+til x}
factp 3
6

/ x = implicit variable. 
/ right to left (til 6 = 0 1 2...5) + 1, multiplie together
```


**🔵 11.13 Demonstrate which calculation is faster, factorial using loops or via KDB**
```q
\ts do[1000;factw 12]
4 1008

/ 4 miliseconds 1008 bytes of memory

\ts do[1000;factp 12]
0 1008

/ 0 miliseconds 1008 bytes of memory
```

**🔵 11.14 Create function safefact that wraps factp with protected evaluation to return null On instead of error when calling on a negattive number**
```q
safefact:{@[factp; x; 0N]}
safefact -10
0N

/ apply factp, if true, return x, if false, return 0N
```


**🔵 11.15 Write function isPalindrome that returns `yes if single argument is a palindrome list. Otherwise return `no**
```q
isPalindrome:{$[x~reverse x;`yes;`no]}
isPalindrome 1 2 2 1
yes

/ $ means if/else statement
/ if x is the reverse of x, return yes. otherwise, no
/ remember, ~ is the match function
/ x = list of numbers
```

**🔵 11.16 Find the sum of all multiples of 3 or 5 below 1000**
```q
sum where {(0 =x mod 3) or (0 = x mod 5)}[til 1000]

233168

/ sum where = adds everything together
/ 0 = x mod 3/5 = no remainders when x is divdied by 3 or 5 = multiples of 3 or 5
/ x = implicit variable
/ til 1000 = implicit variable (runs through 0...999)
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
( [] syms:`a`b`c; floats: 1.1 2.2 3.3; strings: ("bob"; "jim"; "john"))

syms|floats|strings
-------------------
a   | 1.1 | bob
b   | 2.2 | jim
c   | 3.3 | john

/ syms have to start with backtick
/ strings have to enclose within (" ")
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

( [] company: `symbol$(); employees: `int$())

/ changed company type to s (symbol) and employees to i (integer)
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

/ returns values that are same (ferrari 100) 
/ does NOT dupe same values
/ any values that do NOT equal, adds as new row
/ ford = 100 and 5. so new tables contains both values

```

<a name="except_table"></a>
### 🔵 12.11 Except Table

```q
/ except table = only returns values found in LEFT table NOT found in RIGHT table

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
table t:

company | employees
-------------------
ferrari | 100
ford    | 100 
rover   | 100
bmw     | 5 
ford    | 5
```
```q
/ retrieves all columns from table t

select from t

```q
/ retrieve values from column as a column

select company from t

company 
--------
ferrari 
ford   
rover 
bmw 	 
ford 
```

```q
/ retrieve values from column as a list

t[`employees]
100 100 100 5 5
```

```q
/ retrieves row where company = ford 

select from t where company = `ford

company | employees
-------------------
ford    | 100 

```

```q
/ retrieves columns values as a row

t [`employees]
100 100 100 5 5 

```

```q
/ perform operations on entire column

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

```q
/ retrieve first 2 rows

t [ 0 1] / indexing method
or
2#t      / take method

company | employees
--------------------
ferrari | 0
ford    | 0 

```

```q
/ returns last 3 rows

-3#t

company | employees
-------------------
rover   | 0
bmw     |-105 
ford    |-105

```

```q
/ randomly selects 2 rows from table

2 ? t

company | employees
-------------------
rover   | 0
ford    |-105

```

<a name="insert_table"></a>
### 🔵 12.15 Insert Rows Table

```q
/ create empty table 

cars:([] brand:`$();model:`$();purchasedate:`date$())

/ insert `bmw, 318; 2021.01.01

`cars insert (`bmw;`318;2021.01.01)

brand model date
----------------------
bmw   318   2021-01-01

/ have to backtick table (`cars) to insert, otherwise will fail
/ have to insert correct datatype. `318 is a sym
```

```q
/ insert multiple

`cars insert (`audi`ford;`a5`fiesta;2021.01.02 2021.01.03)

brand model  date
----------------------
bmw   318    2021-01-01
audi  a5     2021-01-02
ford  fiesta 2021-01-03

/ insert table into table

`cars insert cars
`cars ,:cars

/ insert table with deleted column

`cars insert delete model from cars

brand model  date
----------------------
bmw   318    2021-01-01
audi  a5     2021-01-02
ford  fiesta 2021-01-03
bmw	     2021-01-01
audi	     2021-01-02
ford	     2021-01-03
```

```q
t: ( [] company: (); employees: () )
company|employees

/ create empty table
```

```q
insert [`t; (`Ferrari; 8)]

company|employees
-----------------
Ferrari| 8

/ backtick t to update underlying table
/ first argument is table name(t), second argument are the values to be inserted
/ semi colon separate columns for the values
```

```q
insert [`t; (Ferrari`bmw; 9 7)]

company|employees
-----------------
Ferrari| 8
Ferrari| 9
bmw    | 7

/ insert will append to the table each time (ferrari repeated)
```

```q
x: ( [] company: `Subaru`Hyundai; employees: 55 56)

company|employees
-----------------
Subaru | 55
Hyundai| 56
```

```q
`t insert x

company|employees
-----------------
Ferrari| 8
Ferrari| 9
bmw    | 7
Subaru | 8
Hyundai| 56

/ table x inserted into table t

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

/ updates apple

/ you cannot upsert multiple rows

`t upsert (`apple`orange;11 23; 100 200)
/error

/ instead you have to upsert a dictionary

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
t1+t2

sym | num
---------
a   | 2
b   | 3
c   | 4

/ both tables have to be keyed
/ column names have to match

/ if UNKEYED, can only do math on tables with numeric fields

t1: ([] sym: 1 2 3; num: 1 2 3)
t2: ([] sym: 1 1 1; num: 1 1 1)
t1+t2

sym | num
---------
2   | 2
3   | 3
4   | 4

/ will find the column names that match, and add values together
/ column names that dont match will be union joined as a new column
```
```q
/ partial key match 

t1:([id:`a`b`c] price: 1 2 3; rating: 10 20 30)
t2:([id:`b`c] price: 10 10 ; rating: 100 100)

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

t1+t2
id price rating
---------------
a   1     10
b   12    120
c   13    130

/ only keys `b`c are matching between the 2 tables
/ so will only add values in these 2 rows
/ a will simply return its original value
```

<a name="joins_table"></a>
### 🔵 12.18 Joins on Tables

```q
/ vertical joins
/ keeps columns, adds additional rows
/ both tables MUST HAVE SAME SCHEMA (column names + types)

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

t1,t2

sym  side price size
---------------------
IBM  buy   10 	 100
AAPL sell  20	 200
GOOG buy   30 	 300
MSFT sell  40	 400
```
```q
/ horizontal rows joins tables with same number of rows
/ adds extra set of columns

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

/ this actually uses each both to join the 2 tables horizontally
```
```q
/ you can also do this"

t1: 5#trade
/ t1 = first 5 rows of trade table

t1,-5#trade

/ combining first 5 rows with last 5 rows 
```
### LEFT JOIN on tables

```q
/ using left join to join tables

t1:([]sym:`a`b`c;ex:`one`two`three;size:100 200 300)
t2:([]sym:`a`b`c;ex:`one`two`three;price:0.1 0.2 0.3)

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
t: ([] a: 1 2 3; b: 4 5 6; c: 7 8 9)

a b c
------
1 4 7
2 5 8
3 6 9

t? 3 6 9
2

/ find these values within the table
/ shows index position 2

t? (2 5 8; 3 6 9)
1 2 

/ can find more than 1 list of indices at once
/ returns list of indices
```

```q
/ find first index position where chem appears in tab2

tab1:([id:"abc"]pupil:`john`paul`rachel;subject:`maths`physics`chem;mark:96 55 82)

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

**🔵 Given:**

```q
stock: ( [] sym: `MS`C`AAPL; sector:`Financial`Financial`Tech; employees: 100 100 100)

sym |sector    |employees
-------------------------
MS  |Financial |100
C   |Financial |100
AAPL|Tech      |100
```

**🔵 13.1 Extract the employees numbers (without the header)**

```q
stock [ ; `employees]
100 100 100
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

**🔵 13.2 Key the first column in stock table above**

```q
1!stock
```

**🔵 13.3 Display only the first and second rows of the stock table**

```q
2#stock

sym |sector    |employees
-------------------------
MS  |Financial |100
C   |Financial |100
```
or

```q
stock [0 1]
```

**🔵 13.4 Select the last row of stock table as a dictionary**

```q
last stock

key       | value
-----------------
sym       | AAPL
sector    | Tech
employees | 100

/ last will retrieve the last row from table stock
/ and return it as a dictionary

```

**🔵 13.5 Insert GOOG in the tech sector with 100 employees**

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

**🔵 13.6 Given:**

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
avg boss `height
182.667

avg employees `height
170f

avg (employees, boss) `height
176.33

/ joins the 2 tables together
/ calculate the average height from joined table
```

**🔵 13.7 Find the 2 tallest employees**
```q
2#`height xdesc employees

name | height
-------------
jim  | 180
john | 170

/ take 2 from employees table, sorted descending by height
```

**🔵 13.8 Given the 2 tables:**

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

`trade insert( [] dt:2021.11.01+1 ; sym:`JPM`UBS; price:1 2; size: 100 200) 

/ or

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

`stock insert [`FB; `Tech; 100]

sym  |sector|employees
---------------------
MS   |Fin   | 100
C    |Fin   | 100
AAPL |Tech  | 100
FB   |Tech  | 100

/ table name + insert (value1, value 2, value 3)
```

**🔵 13.10 In the stock table, change the number of employees for C to 300**

```q
stock upsert (`C;`Fin;300)
```
or
```q
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

/ `column name + xasc + `table name
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

<a name="retrieving_keysvalues"></a>
### 🔵 14.3 Retrieving Keys/Values

```q
/ retrieve keys from table

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
/ retrieve only the column names that are keyed

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
id |name|employer| age
----------------------
`a`|jane|  citi  | 11
`b`|jim |  citi  | 22
`c`|kim |    ms  | 13
`e`|john|    ts  | 15

/ only id column is keyed for now

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
/ or
`id xkey kt

id |name|employer| age
----------------------
`a`|jane|  citi  | 11
`b`|jim |  citi  | 22
`c`|kim |    ms  | 13
`e`|john|    ts  | 15

/ adds first column as a key
```

<a name="removing_keys"></a>
### 🔵 14.6 Removing Keys (xkey)

```q
() xkey `kt
/ or
0!kt

id |name|employer| age
----------------------
a  |jane|  citi  | 11
b  |jim |  citi  | 22
c  |kim |    ms  | 13
e  |john|    ts  | 15

```

<a name="upsert_keys"></a>
### 🔵 14.7 Upserting Keyed Rows / Tables

```q
nd: ( [id:`e`f] name:`dan`kate; employer:`walmart`walmart; age:200 200)

id |name|employer|age
----------------------
`e`|dan | walmart|200
`f`|kate| walmart|200

upsert[`kt;nd]

id |name|employer|age
----------------------
`a`|jane|citi    |11
`b`|jim |citi    |22
`c`|kim |ms      |13
`e`|dan |walmart |200
`f`|kate|walmart |200

/ if key exists and matches, updates value
/ if new key, adds new row
/ since key e already exists, overrides values for name, employer, age
/ must make sure underlying keyed columns match, otherwise error. (1 keyed col vs 2 keyed col)
```

```q
upsert [`kt; ( [id:`f`g] name:`ron`tom)]

id |name|employer|age
----------------------
`a`|jane|citi    |11
`b`|jim |citi    |22
`c`|kim |ms      |13
`e`|dan |walmart |200
`f`|ron |walmart |200
'g'|tom |        |

/ f was updated to ron, and since no employer or age info, pulled from existing kt table (kate's old row)
/ g is new key, so adds new row. since no info, returns null
```

<a name="upsert_multi_rowkeys"></a>
### 🔵 14.8 Upserting Multi Rows/Keys

```q
et: ([employer:`kx`ms`ms; loc:`NY`NY`HK] size: 10 20 30; area: 1 2 3)

employer|loc |size|area
-----------------------
`kx`    |`NY`| 10 | 1
`ms`    |`NY`| 20 | 2
`ms`    |`HK`| 30 | 3

upsert [et; ([employer:`kx`ms; loc:`NY`SG] size: 9 10)]

employer|loc |size|area
-----------------------
`kx`    |`NY`|9   |1
`ms`    |`NY`|20  |2
`ms`    |`HK`|30  |3
`ms`    |`SG`|10  |	

/ updated kx, NY to 9 (overrides prev value)
/ since there was no ms, SG, adds new row 
```

<a name="retrieve_value_keys"></a>
### 🔵 14.9 Retrieving Values as Tables from Keyed Table

```q
id |name|employer|age
----------------------
`a`|jane|citi    | 11
`b`|jim |citi    | 22
`c`|kim |ms      | 33
`d`|john|ts      | 44
`e`|dan |walmart | 200

kt ( [] id:`a`b)

name|employer|age
-----------------
jane| citi   |11
jim | citi   |22

/ retrieves rows based on the values in column id (a and b)
/ returning data as a non-keyed table

or

( [] id:`a`b) # kt

id|name |employer|age
---------------------
`a`|jane| citi   |11
`b`|jim | citi   |22

/ uses the #take function to lookup values in column id
/ notice it also returns the key column (id)
```

```q
/ retrieve values from et where key = ms and hk

Table et
employer|loc |size|area
-----------------------
`kx`    |`NY`| 10 | 1
`ms`    |`NY`| 20 | 2
`ms`    |`HK`| 30 | 3

et`ms`HK

key |value
---------
size|30
area|3

/ will lookup the keys ms and HK and return the values

et(`ms`HK; `kx`NY)

size|area 
---------
 30 | 3
 10 | 1

/ looks up values for both ms+HK (returns 30 and 3) and kx+NY (returns 10 and 1)


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
( [book:enlist`C; ticker:enlist`C]) # p

book | ticker| size
-------------------
`C`  | `C`   | 400

/ need to use enlist since only one row

```

**🔵 15.4 Upsert the following values**
```q
p
`book` | `ticker`|size
----------------------
`A`    | `MS`    | 100
`B`    | `AAPL`  | 200
`B`    | `MS`    | 300
`C`    | `C`     |**400**
**`D`**|**`MS`** |**500**

upsert [p; ([book:`C`D; ticker:`C`MS]size:400 500)]

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

* Foreign keys restrict the values that are allowed in a column

<a name="single_fkey"></a>
### 🔵 17.1 Single Foreign Keys

```q
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

/ column sym is keyed

employee:( [] name:`ryan`charlie`arthur`greg; employer:`TS`KX`KX`MS)

employee 
name   |employer
-----------------
ryan   | TS
charlie| KX
arthur | KX
greg   | MS

update `company$employer from `employee

/ similar syntax to casting
/ you limit the employer column to the domain in company table (keyed column)
/ limits the values in employer column to the domain in the company table (sym column)
/ the domain table HAS to be keyed
/ the values in employer column must exist in domain company table
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
upsert[employee; ( [] name:`james`claire; employer:`RBS`RBS)]
`cast

/ prev set employer column as fkey to company table domain (**sym**)
/ error because RBS is NOT a sym in the company table
/ fkey restricts us from adding what's not in the domain  

insert[`company; ([sym:enlist `RBS] advice:enlist `SELL; level: enlist 20)]

/ need to first add RBS into the company domain (as a keyed sym)
/ remember  need to use enlist when adding single rows

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

/ now you can append james and claire
```

<a name="retrieve_fkey"></a>
### 🔵 17.4 Retrieving Columns via fkey

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

update employer.advice, employer.level from employee

/ prev you keyed the employer column to domain of company table (linking the 2 tables)
/ from the employee table, retrieve the value (advice column) linked from employer column to company table
/ pulls in advice and level from the company table

name   |employer|advice|level
---------------------------
ryan   |TS	|SELL  |12
charlie|KX      |BUY   |10
arthur |KX      |BUY   |10
greg   |MS      |SELL  |90
```

<a name="multi_fkey"></a>
### 🔵 17.5 Multiple Foreign Keys
```q
office: ([sym:`TS`KX`C; loc:`LDN`NY`LDN] employees:10+3?1000)

sym |loc  |employees
-------------------
`TS`|`LDN`|875
`KX`|`NY` |354
`C` |`LDN`|1007

/ sym and loc columns are keyed

employee: ([] name:`ryan`charlie`arthur; employer:`TS`KX`KX; city:`LDN`NY`NY)

employee
name   |employer|city
-------------------
ryan   |TS      |LDN
charlie|KX      |NY
arthur |KX      |NY

exec `office$flip (employer;city) from employee
0 1 1

/ since the office table has 2 keyed columns, you have to "cast" 2 columns as fkey
/ ignore the flip syntax 
/ setting fkey by linking columns employer and city to the domain of company table (keyed columns)
/ ryan    -> look for TS and LDN in office table, found on row 0
/ charlie -> look for KX and NY in office table, found on row 1
/ arthur  -> look for KX and NY in office table, found on row 1
```

```q
update empOffice:`office$flip(employer;city) from `employee

employee
name   |employer|city|empOffice
-----------------------------
ryan   |TS      |LDN |	0
charlie|KX      |NY  |	1
arthur |KX      |NY  |	1

/ adds new column empOffice, and sets fkey to domain of office table

meta employee
c        |t|  f   | a
----------------------
name     |s|	  |	
employer |s|	  |
city     |s|	  |
empOffice|j|office|

/ meta shows us empOffice has an foreign key referencing the office table

update empOffice.sym, empOffice.loc from employee

name   |employer|city|empOffice| sym| loc
---------------------------------------------------
ryan   |   TS   |LDN |	 0     | TS | LDN
charlie|   KX   |NY  |   1     | KX | NY
arthur |   KX   |NY  |   1     | KX | NY

/ employee table doesnt have columns for sym or loc
/ but since you set the empOffice as foreign key, it pulls in the values from the company table
```

<hr>

<a name="fkey_problemset"></a>
## 🔴 18. Foreign Key Problem Set
[Top](#top)

**🔵 18.1. Given the following table**

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

**🔵 18.1. Insert a foreign key column into the trade table called owner, linking trade and book table, using bookID**
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

**🔵 18.2 Join the book table onto the trade table and add the name of person who did trade**
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
## 🔴 19. qSQL
[Top](#top)

```q
select
select a by b from t where c

update
select a by b from t where c

exec
exec a by b from t where c

delete
delete a by b from t where c
```
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
/ result of a select is a table
```

```q
select from trade

/ this will select the whole table
```

```q
select sym, price from trade

/ this will select the sym and price columns only
```

```q
t:([] sym:`a`b`c`d; price: 1 2 3 4)
2 sublist t

/ returns the first 2 rows of t
```
```q
/ Given a table, select the high, low, open, and close price by sym

select high: max price, low: min price, open: first price, close: last price by sym from trade
```
```q

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

fruit   grocer  price   quantity
--------------------------------
banana	tom	4	40
apple	mark	1	10
orange	mark	2	20
pear	allen	3	30
```
```q
select fruit, price from sales where fruit in `banana`pear

fruit   pear
-----------
pear	3
banana	4

/ where statement use in for syms

/ only return 1 row for select

select [1;]fruit, price from sales where fruit in `banana`pear

fruit   pear
-----------
pear	3
```


### Analytics on Grouped Data
```q
select max price by sym from trade
select price by sym from trade
ungroup select price by sym from trade
```

<a name="multipleselect_template"></a>
### 🔵 19.1A) Multiple Select

```q
/ let's say you want to bucket trade sizes based on sym into small, med, big
/ you could do this:

(select count i by sym, sizegroup:`small from trade where size within 0 999),
(select count i by sym, sizegroup:`medium from trade where size within 1000 8999),
(select count i by sym, sizegroup:`big from trade where size > 8999)

/ can use multiple select queries, but this is inefficient
/ instead, you can write a function using BIN to help classify your buckets

sizes: 2000 100 6000 11000
0 1000 9000 bin sizes
1 0 1 2

/ bin takes its LEFT hand buckets, and sorts index position of RIGHT argument
/ so sizes = 4 elements, will return index position of bin
/ 2000 = index position 1 bin
/ 100 = index position 0 bin
/ 6000 = index position 1 bin
/ 11000 = index position 2 bin

`small`med`big 0 1000 9000 bin sizes
`med`small`med`big

/ so you can name your bins using syms as small med big
/ this will bin your size list into the sym named buckets

tradesize:{`small`med`big 0 1000 9000 bin x}
tradesize sizes
`med`small`med`big

/ create function tradesize will has the small med big buckets + bin x variable
/ testing out the function with sizes, returns same as above

select count i by sym, sizebucket:(tradesize;size) fby sym from trade

/ bring it back to the original query, can use tradesize function as an aggregator for fby
/ and returns the number of trades (count i), sorted by sym and its size bucket
```


<a name="selectadd_template"></a>
### 🔵 19.2) Adding a new column using select

```q
select sym, price, size, total:price*size from trade

/ if you select a column name that doesnt exist, it will append it
/ in this case, total will be returned
```

<a name="qsqlvirtuali_template"></a>
### 🔵 19.3) Virtual Column i

```q
select i, sym, price from trade

/ q provides a virtual column i which represents the offset of each record
```

x | sym | price   
--|-------|-------
0 | C    |107.2018
1 | MSFT |96.87488
2 | RBS  |97.11338
3 | A    |100.35  
4 | B    |55.82187

<a name="qsqlselectmaxmin_template"></a>
### 🔵 19.4) Select using [ ]

```q
/ select [] can be used to get the first n or last n records of a table
/ select [n m] can be used to get records starting from n and upto count m from n

select [4] from trade

/ selects the first 4 records
```

```q
select [-3] from trade

/ selects the last 3 records
```

```q
select [1 4] from trade

/ skips 0, returns 1, 2, 3, 4
```

<a name="select_from_where"></a>
### 🔵 19.5) Where


```q
/ where clause operates left to right, so put most restrictive clause first

select from trade where date=20121.05.29, sym=`A

/ where colname = xxx
/ use commas for multiple where expressions
/ put most restrictive clause first, starting from left (saves time)

date      | time        | sym |price| size | cond
--------------------------------------------------
2021-05-29| 09:30:02.758|  A |100.35| 50300| B
2021-05-29| 09:30:17.997|  A |57.81 | 65600| C
2021-05-29| 09:30:21.507|  A |97.85 | 51800| B
```
```q
select price from trade where date=2021.05.29, sym=`A

price
-----
100.3
57.8
97.8
```
```q
select max price from trade where date=2021.05.29, sym=`A

price
------
109.99
```

```q
count select from trade where cond="A"
211597
```

```q
select by sym from trade where date=.z.d

sym |  date    |   time     |price|size |cond
----------------------------------------------
A   |2021-06-02|17:29:57.306|87.54|49100|B
AA  |2021-06-02|17:29:58.789|68.09|88100|A
AAPL|2021-06-02|17:29:58.262|76.18|22500|A

/ by sym = will set sym as the key and agg all dates with the same sym
/ since select + blank , KDB will auto select last entry in column
```

### Where clause from 2 different Tables

```q
t1: ([] date: 2021.10.21 2021.10.21 2021.10.21 2021.10.21; sym: `GOOG`MSFT`FB`AMZN; exch: `nyse`nyse`nasdaq`nasdaq)
t2: ([] sym: `GOOG`FB; exch: `nyse`nasdaq)

select from t1 where date=2021.10.21,([]sym;exch) in t2

/ this will filter date = 2021.10.21
/ and where the sym + exch columns appear in t2
```
```q
/ retrieve IBM from cond A, CSCO from A or B, MSFT from C
/ first, check the meta of the trade table

c    |t|f|a
------------
date |d| |s
time |t| |		
sym  |s| |		
price|f| | 		
size |i| |		
cond |c| |		

/ notice sym datatype is sym and cond datatype is char

/ create new table, toget with the target parameters

toget:([] sym:`IBM`CSCO`CSCO`MSFT; cond:"AABC")

sym   cond
----------
IBM    A
CSCO   A
CSCO   B
MSFT   C

/ then write a select statement using WHERE to retrieve from 2 tables

select from trade where date=2021.10.30,([]sym;cond) in toget

date       sym  price size cond
-------------------------------
2021-10-30 MSFT	60.66 48700 C
2021-10-30 IBM	59.00 28300 A
2021-10-30 MSFT	54.57 23700 C
2021-10-30 IBM	89.19 86600 A
2021-10-30 IBM	84.13 46600 A

/ first filters by date
/ then filters by the sym + cond columns in toget table

```
### Where Clause Ordering

```q
/ be careful about how you order the where filters
/ can change your output

trade:([] price: 50 60 70; size: 300 200 100)

price   size
------------
50	300
60	200
70	100

/ find largest price and size > 200

select from trade where size > 200, price = max price

price   size
------------
50	300

/ however, this is not correct as 50 is NOT the max price

select from trade where price = max price, size > 200

price   size
------------


/ this is correct. 
/ no max price (70) that is greater than 200 (300)
```
```q
/ extract all the following results:
/ gender - male and grade - A
/ gender - female and grade - B
/ gender - female and grade - A

results:([]name:`John`Paul`Rachel`Jane`Emma;gender:"MMFFF";grade:"ABBAC")

name  |gender|grade
--------------------
John  |   M  | 	A
Paul  |   M  |	B
Rachel|   F  |	B
Jane  |   F  |	A
Emma  |   F  | 	C

/ individually this would be the syntax for each query

select from results where gender="M", grade="A"
select from results where gender="F", grade="B"
select from results where gender="F", grade="A"

/ however, can use a table search function
/ usually it goes: where col_name in value (where gender = "A")
/ so you can go where (table of col names) in (table of values)

select from results where ([]gender;grade) in ([] gender:"MFF";grade:"ABA")

name  |gender|grade
--------------------
John  |   M  | 	A
Rachel|   F  |	B
Jane  |   F  |	A
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
```



<a name="select_by"></a>
### 🔵 19.6) By

```q
select first price, first time by date from trade where sym=`AAPL

date        |price|time
-------------------------------
`2021-05-29`|78.6 |09:30:03.025
`2021-05-30`|60.8 |09:30:02.686
`2021-05-31`|55.1 |09:30:18.274

/ select = return column of values
/ by date = groups date as the key column
```

```q
select open:first price, high:max price, low:min price, close:last price by date from trade where sym=`AAPL

date        |open |high  |low |close
------------------------------------
`2021-05-29`|78.66|109.91|50.5|68.01
`2021-05-30`|60.88|109.98|50.0|0.49

/ open: renames the column
```

```q
/ lets say you want to check if the latest value was an uptick, downtick, or unch
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
/ create function for signum deltas

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
/ now lets say you want to group it by sym and see total size traded by direction (uptick, downtick, etc)

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

<a name="select_count"></a>
### 🔵 19.7) Select Count 

```q
select count i, max prirce by date, time.hh from trade where sym=`RBS

/ i is a virtual column that returns the number of rows (as column x)
```
date|hh|x|prrice
-|-|-|-
`2021-05-29`|	`9`|	645 |	50.5 
`2021-05-30`|	`10`	|154	| 50.0

<a name="using_ops_functions"></a>
### 🔵 19.8) Using Operations and Functions 

```q
select price by date from trade where sym=`AAPL, price < avg price

/ finds all AAPL prices that are less than the avg price grouped by date
```

date|price
-|-
`2021-05-29`| 100 99 22 33
`2021-05-30`| 23 199 44 12

```q
select price by date=.z.d from trade where sym=`AAPL, price < avg price

/ retrieve prices, keyed by TODAY, where AAPL's price is less than the avg price
/ grouped by today; 0 = false, 1 = true
```

d | price
-|-
`0` | 23 52 63
`1`| 23 66 12

```q
select {x % max x} price by date = .z.d from trade where sym=`AApl, price < avg price

/ retrieve price / max price, keyed by today, where the price is less than the avg price
```

d | price
-|-
`0b` | 0.98 0.7 0.8
`1b` | 0.12 0.43 0.32

<a name="in_function"></a>
### 🔵 19.9) In Function

```q
select from trade where sym in `AAPL`RBS

/ in function checks if every LHS argument occurs anywhere in RHS argument (AAPL or RBS)
/ a faster way of checking "or" arguments
```

date|time|sym|price|size|cond
-|-|-|-|-|-
2021-05-30|	09:30:02.743 |	RBS |	97.113	| 80700 |	C
2021-05-30|	09:30:03.025 |	AAPL |	78.66 |	19000	| A


<a name="within_function"></a>
### 🔵 19.10) Within Function

```q
select from trade where sym=`RBS, price within 95 100

/ checks if LHS argument is within the range on RHS argument
/ has to have lower + upper bind
```

date|time|sym|price|size|cond
-|-|-|-|-|-
2021-05-30|	09:30:02.743 |	RBS |	97.113	| 80700 |	C
2021-05-30|	09:30:03.025 |	AAPL |	98.66 |	19000	| A

```q
select from trade where sym=`RBS, price within 95 100, time within 11:30 12:00

/ 2 within filters, price and time
```

date|time|sym|price|size|cond
-|-|-|-|-|-
2021-05-30|	11:40:02.743 |	RBS |	97.113	| 80700 |	C
2021-05-30|	11:44:03.025 |	AAPL |	98.66 |	19000	| A

<a name="xbar_function"></a>
### 🔵 19.11) Xbar Function
```q
/ grouping for temporal data buckets (time)

x xbar time.minute / x mins buckets
x xbar time.hh / x hour buckets
x bar time.ss / x second buckets

20 xbar time.ss / same thing
0d00:00:20 xbar time / same thing
```

```q
/ grouping for other data buckets (price)
/ apply xbar grouping to price column

x xbar price
x xbar cond
x xbar source

select sum size, cnt:count i by sym, 1 xbar price from trades

sym|price|  size  |cnt
----------------------
 A |50.0 |44191500|838
 A |51.0 |42318700|842
 A |52.0 |41432200|832

/ groups the data by sym and 1 dollar price buckets
/ cnt = tallies virtual column i; how many trades were executed by sym for that price bucket
```

```q
/ find the max price and total size of trades during 5 min window

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

```
```q
select max price by sym, 45 xbar time.minute from trade

sym |minute | price
----------------------
 A  |09:00  | 109.94
 A  |09:45  | 109.99
 A  |10:30  | 109.96

/ group by sym, set xbar as 45 minute time buckets
```

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
```q
select price by sym, 240 xbar time.minute from trade
select avg price by sym, 240 xbar time.minute from trade
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
a: ([] c1: 1 2 3; c2: `a`b`c)

exec c1 from a
1 2 3

/ exec single column returns a list

exec c1, c2 from a
c1 | 1 2 3
c2 | `a`b`c

/ exec multi columns returns a dictionary

1#exec from a
c1 | 3

/ take the first row from a

1#exec c2 from a
`a

/ take the first row and return the value in c2
```

```q
exec price from trade where date=.z.d, sym=`AAPL
62 59 13

/ exec single column = single list returned
```

```q
select price from trade where date=.z.d, sym=`AAPL

/ select = single column returned

price
------
62
59
13

```

```q
exec first price from trade where date=.z.d, sym=`AAPL
62
```

```q
exec price by sym from trade where date=.z.d, sym=`AAPL
AAPL | 62 59 13
```

```q
exec price by sym from trade where date=.z.d

sym   | price
----------------
`A`   | 108 77 88
`AA`  | 33 45 23
`AAPL`| 34 56 23
```

```q
exec first price by sym, cond from trade where date=.z.d, sym in `KX`AAPL

sym    |cond | price
------------------
`AAPL` |     | 95
`AAPL` | `A` | 43
`KX`   | `C` | 32

```


```q
a: ([] c1: 1 2 3 1 2; c2: `a`b`c`a`b)
exec distinct c1 from a
1 2 3

/ returns only distinct values in col c1

exec distinct c1, distinct c2 from a
c1 | 1 2 3
c2 | `a`b`c

/ exec allows distinct on multiple columns
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
```
```q
select city, distinct country from cnc

/ error because select expects the columns to have the same length
```

<a name="update_statement"></a>
### 🔵 19.13) Update
```q
/ updates a pre-existing column
/ if column doesnt exist, gets added to end of column list
/ original table unaffected unless the data is persisted by using backtick
```
```q
update price: 10.0 from trade

/ this will update all prices to 10
```
```q
/ to update a single where condition:

update price:10.0 from trade where sym=`C

date       time         sym  price    size  cond
------------------------------------------------
2021.10.30 09:30:02.553 C    10       63500 B   

/ to update multiple where conditions:

update price:10.0 from trade where sym in `AAPL`GOOG

date       time         sym  price    size  cond
------------------------------------------------
2021.10.30 09:30:02.553 C    10       63500 B   
2021.10.30 09:30:02.701 MSFT 10       1700  B   
2021.10.30 09:30:02.743 RBS  10       80700 C  

/ this will update prices to 10 for AAPL and GOOG 
/ the where clause updates only the filtered records
```
```q
update vol:price*size from trade where sym in `AAPL`GOOG

/ new column vol is added
```
```q
update price:avg price by sym from trade where sym in `AAPL`GOOG

/ updates the price to average price, grouped by sym 
```
```q
tt:100?trade

/ randomly selects 100 rows
```

```q
date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |422| B
2021.03.01 | 15:09:01| JPM | 74  |412| C

update cond: "D" from tt

date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |422 | D
2021.03.01 | 15:09:01| JPM | 74  |412 | D

/ updates cond to "D"
```

```q
update size%100 from tt

date       |  time   | sym |price|size| cond
---------------------------------------------
2021.01.01 | 15:10:01| BAC | 70  |42.2| D
2021.03.01 | 15:09:01| JPM | 74  |41.2| D
2021.03.01 | 15:09:01| UBS | 41  |31.2| D


/ can perform function on entire column. size divided by 100
```

```q
update advice:`sell from tt

date       |  time   | sym |price|size|cond|advice
---------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|D   | sell
2021.03.01 | 15:09:01| JPM |  74 |41.2|D   | sell
2021.03.01 | 15:09:01| UBS |  41 |31.2|D   | sell


/ if you update a column that doesnt exist, it will add the column
/ new column added called advice and populates with sell
/ notice it has to be backtick sell
```

```q
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
update maxprice: max price by sym from tt

date       |   time  | sym |price|size|cond|maxprice
----------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  D | 104
2021.03.01 | 15:09:01| JPM |  74 |41.2|  D | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  D | 91

/ since maxprice doesnt exist, adds new column to end
```

<a name="delete_columns"></a>
### 🔵 19.14) Delete Columns
```q
/ cannot have BY or WHERE clause

date       |   time  | sym |price|size|cond|maxprice
----------------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2|  D | 104
2021.03.01 | 15:09:01| JPM |  74 |41.2|  D | 102
2021.03.01 | 15:09:01| UBS |  41 |31.2|  D | 91

delete maxprice from tt

date       |   time  | sym |price|size|cond
--------------------------------------------
2021.01.01 | 15:10:01| BAC |  70 |42.2| D 
2021.03.01 | 15:09:01| JPM |  74 |41.2| D 
2021.03.01 | 15:09:01| UBS |  41 |31.2| D 

/ removes maxprice column
```
```q
delete date, time from tt

sym |price|size|cond
--------------------
BAC |  70 |42.2| D 
JPM |  74 |41.2| D 
UBS |  41 |31.2| D 

/ deletes multiple columns from the table
```
```q
/ if you try to delete rows + columns together, doesn't work

delete price from trade where sym=`BAC
error
```

<a name="delete_rows"></a>
### 🔵 19.15) Delete Rows

```q
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
### 🔵 19.16) Sort Ascending / Descending 

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
### 🔵 19.17) Renaming / Reordering Columns

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

<a name="fby_sql"></a>
### 🔵 19.18) Filter by fby

```q
/ fby aggregates values from one list based on group defined in another
/ (aggr;d) fby g
/ aggr = aggregate function = max, min, sums, etc.
/ d = column name
/ g = another column name
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
```
### Functions on fby

```q
price = (max;price) fby sym
price < (last;price) fby sym
price > (avgs;price) fby sym
price > (mavg[10];price) fby sym / moving avg 10 of price by sym
```

### fby Example 1

```q
city:`NY`NY`LA`SF`LA`SF`NY
temp:32 31 75 69 70 68 12

(min;temp) fby city
12 12 70 68 12

/ so this calculates the min temp for every city (12 for NYC)

```

### fby Example 2
```q
/ find the max price per symbol

time       |sym  |src|price | size
-----------------------------------
2019-03-11 |GOOG | L |36.01 | 1427
2019-03-11 |GOOG | O |36.01 | 708
2019-03-11 |MSFT | N |35.5  | 7810
2019-03-11 |MSFT | O |31.1  | 1100

select from t where price=(max;price) fby sym

time       |sym  |src| price | size
-----------------------------------
2019-03-11 |GOOG | L | 36.01 | 1427
2019-03-11 |GOOG | O | 36.01 | 708
2019-03-11 |MSFT | N | 35.5  | 7810

/ this is not correct, since there are still 2 GOOG (since both same "max" price)
/ you can add another fby filter for time

select from t where price=(max;price) fby sym, time=(max;time) fby sym

time      |sym  |src| price | size
-----------------------------------
2019-03-11|GOOG	| O | 36.01 | 708
2019-03-11|MSFT | N | 35.01 | 7810

/ in this case, you filtered max price by sym, and max time by sym
```
### fby Example 3
```q
/ find the max price on this date

select from trade where date=2021.10.31, price=max price

/ filter by date, then the max price from this date
```
```q
/ find max price by sym on this date

select from trade where date=2021.10.31, price=(max;price) fby sym

/ filter by date, then find max price by sym
/ groups the aggregation by sym
```
```q
/ find max price by sym and cond on this date

select from trade where date=2021.10.31, price=(max;price) fby ([]sym;cond)

/ aggregate by more than one field using a table
/ filter by date, then max price by sym and cond
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

`sym xgroup trade

sym | date
----| -----
C   | 2021.10.19 
MSFT| 2021.10.19 
RBS | 2021.10.19

/ group by column `sym
/ the same as saying:

select time by sym from trade

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
2021-10-19	09:30:02.553	C	     107.2	   63500	  B
2021-10-19	09:30:02.743	RBS	    97.1	   80700	  C
2021-10-19	09:30:02.758	A	     100.3	   50300	  B
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
### 🔵 19.23) ^ Carrot

```q
/ ^ replaces nulls with atom on left
/ has to be of compatible type

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
### 🔵 19.24) iasc/idesc

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
```q
/ Case Study: Pull the best bid from orderbook

table t:

t         bidPrices            bidSizes
------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  57 0 72 50 62 51
00:59:05  0.97 7.44 9.33 2.93  97 99 27 31
01:19:44  2.88 5.63 4.98 5.56  47 57 31 15 68 49

update bidIndex:({idesc x} each bidPrices) from t

t         bidPrices            bidSizes           bidIndex
----------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  57 0 72 50 62      2 1 0 4 
00:59:05  0.97 7.44 9.33 2.93  97 99 27 31        2 1 4 0
01:19:44  2.88 5.63 4.98 5.56  47 57 31 15 68 49  1 4 3 0

/ from col bidPrices, shows index position of descending values
/ 2nd index position = 3rd value = 9.84 largest

update bidIndex:({first idesc x} each bidPrices) from t

t         bidPrices            bidSizes           bidIndex
----------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  57 0 72 50 62      2 
00:59:05  0.97 7.44 9.33 2.93  97 99 27 31        2
01:19:44  2.88 5.63 4.98 5.56  47 57 31 15 68 49  1

/ adding first = only retrieves first value 
/ largest bid since ordered by idesc

update bestBid:bidPrices@'bidIndex from update bidIndex:({first idesc x} each bidPrices) from t

t         bidPrices            bidSizes     bidIndex   bestBid
--------------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  0 72 50 62    2          9.84 
00:59:05  0.97 7.44 9.33 2.93  23 99 27 31   2          9.33
01:19:44  2.88 5.63 4.98 5.56  57 31 15 49   1          5.63

/ bestbid = looks at bidIndex col, retrieves index position 2 from bidPrice col = 9.8
/ everything after from is what we calculated above as the bidIndex col

update bestBidSize:bidSizes@'bidIndex from update bidIndex:({first idesc x} each bidPrices) from t

t         bidPrices            bidSizes     bidIndex   bestBidSize
------------------------------------------------------------------
05:15:43  7.83 8.20 9.84 6.93  0 72 50 62    2          50 
00:59:05  0.97 7.44 9.33 2.93  23 99 27 31   2          27
01:19:44  2.88 5.63 4.98 5.56  57 31 15 49   1          31

/ bestBidSize = looks at bidIndex col, retrieves index position 2 from bidSizes col = 50

/ can combine all 3 queries into single one:

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

**🔵 20.1 Extract from trade table, trades for MS greater than 1,000 in size**

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

**🔵 20.2 From the trade table, find the total size of all trades and the average price paid per sym**

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

**🔵 20.3 From the trade table, find the trade that was largest size for each sym**

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

**🔵 20.4 From the trade table, select the latest trade for each sym, and include all details**

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

**🔵 20.5 Find all trades that have sym GOOG**

```q
select from trade where sym=`GOOG
```
sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	87.54| 49100 | B
GOOG|	2021-06-03|	87.54| 49100 | C

<hr>

**🔵 20.6 Find all trades that have sym GOOG or RBS or A**

```q
select from trade where sym in `GOOG`RBS`A
```
sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	87.54| 49100 | B
RBS|	2021-06-03|	87.54| 49100 | C
A|	2021-06-03|	87.54| 49100 | C

<hr>

**🔵 20.7 Find all trades for google that had a price between 70 and 80**

```q
select from trade where sym=`GOOG, price within 70 80
```

sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	72 | 49100 | B
GOOG|	2021-06-03|	75| 49100 | C
GOOG|	2021-06-03|	78 | 49100 | C

<hr>

**🔵 20.8 Count the number of trades and total size of trades per hour for sym RBS**

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

**🔵 20.9 Select the number of trades and total size of trades every 30 mins for the sym RBS**

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

**🔵 20.10 Find all trades for `A where the price was cheaper than the average for that day**

```q
a: update avgPrice: avg price by date from select from trade where sym=`A
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
/1 start by creating complete list of buckets

start: 09:00
end: 09:59
bucket: 15

/ so each bucket will be 15 mins

/2 number of buckets required for time span (end-start)

(end-start) % bucket
3.933

/ round up to whole number

ceiling (end-start) % bucket
4

/ ceiling function will round 3.933 up to 4
```

```q
/3 create list of buckets by creating list of integers to num of buckets
/ this is done by multiplying each element x bucket size (15)

bucket * til ceiling (end-start) % bucket
0 15 30 45

/ bucket x til 4
/ 15 x 0 1 2 3

/4 add start time by making list of time buckets and rename as times

times: start+bucket * til ceiling (end-start) % bucket
09:00u; 09:15u; 09:30u; 09:45u
```

```q
/4 cross distinct syms with times list you just created
/ and sort by sym

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
```

```q

/5 Join rack with original xbar table using # take operator

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


[Top](#top)

<a name="bottom"></a>
