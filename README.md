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
7. [Rename Column Table](#rename_column_table)
8. [Add Column Table](#add_column_table)
9. [Sort Column Table](#sort_column_table)
10. [Union Table](#union_table)
11. [Except Table](#except_table)
12. [Inter Table](#inter_table)
13. [Distinct Table](#distinct_table)
14. [Retrieve From Table](#retrieve_table)
15. [Insert Table](#insert_table)
16. [Operations on Tables](#operations_table)

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
5. [Select from where](#select_from_where)
6. [Select by](#select_by)
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
5. [Each Previous](#eachprevious_adverb)

## 25. [Adverbs Problem Set](#adverbs_problemset)

## 26. [Import and Exporting Data](#importexport_header)
1. [Importing / Loading TXT Files](#txt_import)
2. [Exporting / Saving TXT Files](#txt_export)
3. [Exporting / Saving Tables as txt, csv, excel, and xml files](#tables_exportformat)
4. [Exporting / Saving Tables with New Name](#export_tablenewname)
5. [Importing CSV Files](#csv_import)
6. [Saving to Binary Files](#binaryfile_export)

## 27. [Splayed Tables](#splayedtable_header)

## 28. [Case Studies](#casestudies_header)
1. [Loading CSV Files](#load_csv)
2. [Comparing Current Orders against Potential Crosses](#cross_case)
3. [Netting off buys and sells from same Stock](#nettingbuyssells_case)

## 29. [Random Questions](#random_questions)



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
```
1 2
* take # will take the first 2 values of list k

```q
-2#k
```
3 4
* take last 2 values of list k

```q
5 # 8
```
8 8 8 8 8 
* take 5 values of 8

```q
5 # 1 2 3
```
1 2 3 1 2
* take 5 values from this list

<a name="drop_intro"></a>
### 🔵 1.14 Drop
k: 1 2 3 4

```q
2_k
```
3 4
* drop the first 2 values from list k

```q
-2_k
```
1 2
* drop the last 2 values from list k

<hr>

<a name="pluscolon"></a>
### 🔵 1.16 +:

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
### 🔵 1.17 Multi-line Comment

```q
/
to write a multi line comment
start with "/"
end with "\"
\
```


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
### Date

Given:
d: 2011.02.22

```q
d.year
d.mm
d.month
d.dd
```
2011i \
2i \
22i 

<a name="time_type"></a>
### 🔵 2.2 Time

Given:
t: 11:02:58:000

```q
t.hh
t.mm
t.minute
t.ss
t.second
```
11i \
2i \
11:02 \
58i \
11:02:85 

```q
.z.t
.z.d
.z.n
```
* current time
* current date
* current timespan

<a name="cast_type"></a>
### 🔵 2.3 Casting
* casting = changes one datatype to another type that's compatible
* parsing = converting from a string to a native type
* x $ y 
* x = target type
* y = source type
* Casting y to x

```q
Casting strings to sym

/ "a","b","c" are strings

"S" $ "a","b","c"
`abc
```

```q
Converting syms to strings 

/ `abc is a sym

string `abc
"abc"
```

```q
`date$2
```
2000-01-03d
* 2nd day of the millennia

```q
`time$2
```
00:00:00.002t
* 2 + 00:00:00.000

```q
`month$2
```
2000.03m
* KDB time starts at 2000.01.01 
* 2 + 2000.01.01

```q
`minute$2
```
00:02
* takes 2 + 00:00

```q
`seconds$2
```
00:00:02

```q
`boolean$9
```
1b
* casting a boolean will always be true (1b), unless its 0

```q
`boolean$0
```
0b

<a name="enu_cast"></a>
### 🔵 2.4 Enumeration
* enumeration is converting a list of values to a defined domain which restricts values to that domain

```q
suits:`hearts`clubs`spades`diamonds
l: `hearts`clubs`diamonds
el: `suits$l
```
* enumerate all symbols in list l under same domain as suits
* will enforce/restrict their type as same domain 

```q
el,:`apple
```
cast
* if you try adding a value that is NOT within that domain (apple), you will get a cast error

```q
el[0]:`pear
```
cast
* also cannot update value if not in the existing domain

<hr>

<a name="casting_problemset"></a>
## 🔴 3. Data Types & Casting & Enumeration Problem Set
[Top](#top)

**🔵 3.1 What is the syntax to add to a list**
```q
el, : apple
```
* listname + , + :

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
```
* these are strings which you are trying to parse into the date datatype
* have to use upper case when parsing

<hr>

**🔵 3.4 Given the mixed list L: ("100.1";"hello";"10"), convert elements to float, char, and int**
```q
"F*I"$("100.1";"hello";"10")
```
100.1
"hello" 
10i
* have to use capital F and I
* the astrik is used for strings

<hr>

**🔵 3.5 Create empty symbol list s**

```q
s: `symbol$()
```

**Append integer 3 to list s**
```q
s ,: 3
```
type 
* error because 3 is an int and the list is enumerated as syms

**Append symbol ooo to list s**
```q
s,:`ooo
```

<hr>

**🔵 3.6 Create an enumeration t containing values p q r that is restricted to domain s**
```q
s: `symbol$()
t: `s$`p`q`r
```
* t is now an enumeration which only contain domain s (symbols)

**🔵 3.7 Insert new value u into t**

```q
s,:`u
t,:`u
```
* since t is restricted to domain s, need to first add u into s before adding to t

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
```

<a name="retrieve_list"></a>
### 🔵 4.6 Retrieving from Lists
L: 10 20 30

```q
L[0]
L[1 2]
L 1 2 3
```
10 \
10 20 \
10 20 30 \

* retrieval uses 0 indexing logic (count starts with 0)
* notice you DONT use colons : when retrieving from lists

<a name="update_list"></a>
### 🔵 4.7 Update List Values
L: 10 20 30
```q
L[0 1 2] : 40 50 60
```
40 50 60
* notice you use colon : to update values

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
### 🔵 4.10 Sublist

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
```

```q
2 2 sublist 1 2 3 4 5
3 4

/ from index position 2, take 2 items
```

<a name="find_list"></a>
### 🔵 4.11 Find in List

```q
1 2 3 4 5 ? 3
2

/ find position of 3
```
```q
1 2 3 4 5 ? 7
5

/ not found, returns max index + 1
```
```q
1 2 2 3 4 ? 2
1

/ only returns first occurence
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

<hr>

<a name="list_problemset"></a>
## 🔴 5. Lists Problem Set
[Top](#top)

**🔵 5.1 What is the difference between 3 ? 10 and 3 ? 10 20 30**

```q
3 ? 10

/ returns 3 random numbers from 0-10
```

```q
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

* A dictionary is a mapping between a list of keys and a list of values of the same length
* left of ! = list of keys
* right of ! = list of values

<a name="dict_from_list"></a>
### 🔵 8.1 Constructing a Dictionary from Lists
```q
k:`apple`plum
v:`green`purple
d:k!v
```
key|value
-|-
apple|	green
plum|	purple

<a name="retrieve_dict"></a>
### 🔵 8.2 Retrieving Values from Dictionaries

Given dictionary d, 3 ways to retrieve a

```q
d:`a`b`c!1 2 3
```
key|values
-|-
a|	1
b|	2
c|	3

```q
d[`a]
d`a
d@`a

/ all 3 syntax work for retrieving values in a dictionary
```

```q
key d
a b c

/ retrieves all keys in d
```

```q
value d
1 2 3

/ retrieves all values in d
```

```q
d @ `a`b`a`
1 2 1 1

/ can retrieve multiple values
```

<a name="index_retrieve_dict"></a>
### 🔵 8.3 Index Retrieve

```q
dc:`c1`c2!(10 * til 5; 1+ til 3)
```
key | value
-|-
c1	|0 10 20 30 40
c2	|1 2 3

```q
dc[`c2]
1 2 3 

/ retrieves list c2
```

```q
dc[`c2;2]
3

/ retrieves from list c2, index position 2 (0 1 2)
```

```q
dc[ ; 1]

/ takes index position 1 from values (2nd column)
```
key|value
-|-
c1	|10
c2	|2 

<a name="take_dict"></a>
### 🔵 8.4 Take

```q
2#d

/ take first 2 entries from d
```

key | value
-|-
a | 1
b |2

```q
`a`b#d

/ take keys `a and `b and its values from d
```

key | value
-|-
a | 1
b | 2

```q
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
2_d

/ drop first 2 rows from dictionary d
```

key | value
-|-
C | 3


```q
d: `a`b`c ! 1 2 3

`b _ d

/ drop key `b and its value (2)
```

key | value
-|-
a | 1
c | 3

<a name="upsert_dict"></a>
### 🔵 8.6 Upsert

```q
d [`e]: 99

/ upsert = update insert
/ if key exists, will update value
/ if key doesn't exist, will insert new key + value
```

key|value
-|-
a|	1
b|	2
c|	3
e|	99

<a name="multi_key_dict"></a>
### 🔵 8.7 Multi Key Dictionaries

```q
md: (`a`b;`c`d;`e`f) ! 1 2 3
```
* created a dictionary md with 2 keys for every 1 value
* ; separate the various rows

key| value
-|-
a b	|1
c d	|2
e f	|3

<a name="repeat_key_dict"></a>
### 🔵 8.8 Repeat Keys

You can technically have multiple repeat keys, but this is NOT recommended

```q
dk: 1 2 3 1 ! `a`b`c`d

/ notice key 1 is repeated
```

key|values
-|-
1|	a
2|	b
3|	c
1|	d

```q
dk[1]
a

/ if you attempt to retrieve a repeated key, it will only return the first value
```

<a name="find_dict"></a>
### 🔵 8.9 Find Operator ?

```q
d?2
b

/ ? is the find operator
/ from dictionary d, find key 2, return its value (b)
```

<a name="dict_opt"></a>
### 🔵 8.10 Dictionary Operators
```q
d: `a`b`c ! 1 2 3

sum d
6

avg d
2
```

```q
neg d

/ turns all values negative
```

key|value
-|-
a|	-1
b|	-2
c|	-3

```q
d%100

/ divides all values by 100
```

key|value
-|-
a|	0.01
b|	0.02
c|	0.03

```q
Adding / Joining Dictionaries

d1:`a`b`c!1 2 3
d2:`a`b`c!1 2 3

d1+d2
d1,d2
```
key|value
-|-
a|	2
b|	4
c|	6

<hr>

<a name="dict_problemset"></a>
## 🔴 9. Dictionary Problem Set
[Top](#top)

**🔵 1. Given the below dictionary, find the type, the keys, and its values**
```q
d:`p`q`r`s!10 20 40 100
```
key|value
-|-
p|	10
q|	20
r|	40
s|	100

```q
type d
key d
value d
```
99h \
p q r s \
10 20 40 100 \

<hr>

**🔵 2. Add new entry u 200 to list d**
```q
d[`u]: 200
```
* upsert. will update if key exists, if not, will append it

key|value
-|-
p|	10
q|	20
r|	40
s|	100
u| 200

<hr>

**🔵 3. Change value of p to 2**
```q
d[`p]:2
```
<hr>

**🔵 4. Create dictionary d2, only containing values of p q r from dictionary d**
```q
d2:`p`q`r#d
```
* take p q r from dictionary d

<hr>

**🔵 5. Add common elements in d2 and d, only return common keys and values**
```q
(key[d] inter key[d2]) # d+d2
```
* inter returns values occuring in both lists
* take the common keys in dictionary d and d2 and show its values

key|value
-|-
p|	20
q|	40
r|	80

<hr>

**🔵 6. Given the 2 dictionaries below, find those who are greater than 1.7m in height**
```q
dheight:`john`mark`luke`paul`ian`peter!1.5 1.6 1.7 1.8 1.9 1.4
dweight:`john`mark`luke`paul`ian`peter!81 72 88 91 55 110
```
dheight

key|value
-|-
john|	1.5
mark|	1.6
luke|	1.7
paul|	1.8
ian|	1.9
peter|	1.4

dweight

key|value
-|-
john|	81
mark|	72
luke|	88
paul|	91
ian|	55
peter|	110

```q
dheight > 1.7
```
key|value
-|-
john|	0b
mark|	0b
luke|	0b
paul|	1b
ian|	1b
peter|	0b

* dictionary + condition = examines values as booleans, returns as true/false

```q
where dheight > 1.7
```
* where = returns the keys

paul ian

<hr>

**🔵 7. Find the average height of people who weight over 90**
```q
where dweight > 90
```
paul peter

```q
dheight where dweight > 90
```
1.8 1.4

```q
avg dheight where dweight > 90
```
1.6

<hr>

**🔵 8. Find the body mass index (weight) / (height x height)**
```q
dweight%dheight*dheight
```
key|value
-|-
john|	36.0
mark|	28.1
luke|	30.4
paul|	28.0
ian|	15.2
peter|	56.1

<hr>

<a name="functions_header"></a>
## 🔴 10. Functions
[Top](#top)

Functions are encased in { }


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

* while will execute a statement x number of times until statement is no longer true

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

/ a = 1; a becomes 1+1(2)
/ b = 2; b becomes 2+1(3)
/ show enlist shows b and a in a clean list
/ stop running this loop when first condition becomes false
```

key|value
-|-
3|2
4|3
5|4
6|5

<a name="multi_cond_while_loop"></a>
### 🔵 10.11 Multi Condition While Loops

```q
a:1
b:2
while[(a<10) and (b<3); a:a+1; b:b+1; show enlist b,a]
```
* if you have 2 conditions, must use ( ) as KDB reads right to left
* 2 < 3, yes. 1< 10, yes
* so a = 1+1 = 2 and b=2+1 = 3
* shows 3 2
* 3 is not < 3, so false. stops running

```q
isprime:{if[x<2; 0b]; a:2; while[a<x; if[(x mod a)=0;0b]; a+:1]; 1b}
```
* if x = 1
* x(1) < (2) (TRUE) so returns 0b (not prime)\

* if x = 4
* x(4)< 2 (FALSE), skip 0b statement, moves onto a:2
* a(2) < x(4)? (TRUE), x mod a = 4 mod 2 = 0 (no remainders if you divide 4 by 2). (TRUE), so returns 0b (not prime)\

* if x = 7
* x(7) < 2 (FALSE), skip 0b
* a(2) < x(7) (TRUE), x mod a = 7 mod 2 = 1 (FALSE), so returns 1b (TRUE)

```q
findprime: { [n] r:(); a:1; while [a<n; if[isprime[a];r,:a]; a:a+1];r}
findprime 10 
```
2 3 5 7
* n = single argument
* r () = empty list
* a starts from 1, if a (1) < n (10) TRUE, append a to list r
* go through every value of a, and add to list r

<hr>

<a name="func_problem_set"></a>
## 🔴 11. Functions Problem Set
[Top](#top)

**🔵 11.1 Create a function volc that accepts 2 arguments (r and h), that returns the volume of the given volc [2;3]** \
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

**🔵 11.2 Write function sph that takes radius and returns the area and volume**\
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

**🔵 11.3 Create function setc that takes one argument and sets the global value c to that argument**
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

**🔵 11.4 Given raise:{x xexp y}, create function that is projection of the raise. Ex, root[9] = 3**
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

**🔵 11.5 Convert all entries of list L to a string**
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

**🔵 11.6 Given the string, find and replace "cow" with "kangaroo"**

```q
st: "the cow jumped over the moon"
ssr [st; "cow";"kangaroo"]
```
"the kangaroo jumped over the moon"
* ssr = string search replace.
* syntax = ssr [listname + find this + replace with this]

<hr>

**🔵 11.7 Create function sayHi that takes 2 arguments, first one name, second one age and behaves as follows:**

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

**🔵 11.8 I have a box of 7 eggs, find the median and average weight**

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

**🔵 11.9 I sold 2 boxes of eggs. 1 box had 10 eggs and i sold it for 50 each. the other box had 20 eggs and sold it for 100 each. find the average price paid per egg**

```q
10 20 wavg 50 100
```
83.3
* wavg = weight average function

<hr>

**🔵 11.10 Generate list k of 10 random integers. Find the moving average with window size of 3**
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

**🔵 11.11 Create function factw, using a loop to write a factorial function**
```q
factw:{r:i:1; while[i<=x; r*:i; i+:1];r}
factw 3
```
6
* x is implicit variable= 3
* set r = i = 1
* while i(1) <= x(3) TRUE, execute following statements
* r = r(1) * i(1) = 1
* i = i(1) + 1 = 2

i(2) <= x(3) TRUE, so continue executing
* r = r(1) x i(2) = 2
* i = i(2) + 1 = 3

i(3) <= x(3) TRUE
* r = r(2) x i(3) = 6
* i = i(3) + 1 = 4

i(4) <= x(3) FALSE, so returns r = 6

<hr>

**🔵 11.12 Re-create the factorial function as factp without using loops**
```q
factp:{prd 1+til x}
factp 3
```
6
* x = implicit variable. 
* right to left (til 6 = 0 1 2...5) + 1, multiplie together

<hr>

**🔵 11.13 Demonstrate which calculation is faster, factorial using loops or via KDB**
```q
\ts do[1000;factw 12]
```
4 1008
* 4 miliseconds 1008 bytes of memory

```q
\ts do[1000;factp 12]
```
0 1008
* 0 miliseconds 1008 bytes of memory

<hr>

**🔵 11.14 Create function safefact that wraps factp with protected evaluation to return null On instead of error when calling on a negattive number**
```q
safefact:{@[factp; x; 0N]}
safefact -10
```
0N
* apply factp, if true, return x, if false, return 0N

<hr>

**🔵 11.15 Write function isPalindrome that returns `yes if single argument is a palindrome list. Otherwise return `no**
```q
isPalindrome:{$[x~reverse x;`yes;`no]}
isPalindrome 1 2 2 1
```
yes
* $ means if/else statement
* if x is the reverse of x, return yes. otherwise, no
* remember, ~ is the match function
* x = list of numbers

<hr>

**🔵 11.16 Find the sum of all multiples of 3 or 5 below 1000**
```q
sum where {(0 =x mod 3) or (0 = x mod 5)}[til 1000]
```
233168
* sum where = adds everything together
* 0 = x mod 3/5 = no remainders when x is divdied by 3 or 5 = multiples of 3 or 5
x = implicit variable
til 1000 = implicit variable (runs through 0...999)

<hr>

<a name="tables_header"></a>
## 🔴 12. Tables
[Top](#top)

* A table is a flipped dictionary.
* Vectors of data are organized by columns. 
* Tables are encased by parathesis ( ) and contain brackets [ ] which assigns the key.

<a name="dict_to_table"></a>
### 🔵 12.1 Flipping Dictionary to Table

```q
d: `company`employees`! (`ford`bmw; 300 100)
```
key|Value
-|-
company	|`ford`bmw
employees|	300 100

```q
flip d

/ when you flip a dictionary, you get a table
```
company | employees
-|-
ford |	300
bmw	| 100

<a name="simple_table"></a>
### 🔵 12.2 Simple Table

```q
( [] company: `ford`bmw; employees: 300 100)

/ have to define a table within parathesis ( )
/ tables must have [] which are for key columns
/ semi colon ; separates next column
```
company | employees
-|-
ford |	300
bmw	| 100

<a name="single_row_table"></a>
### 🔵 12.3 Single Row Table

```q
( [] company: enlist `ford; employees: enlist 300)

/ have to use enlist for atoms and single row tables
```
company | employees
-|-
ford |	300

<a name="mixed_table"></a>
### 🔵 12.3 Mixed Table

```q
( [] syms:`a`b`c; floats: 1.1 2.2 3.3; strings: ("bob"; "jim"; "john"))

/ syms have to start with backtick
/ strings have to enclose within (" ")

```
syms|floats|strings
-|-|-
a|	1.1 |	bob
b|	2.2	|jim
c|	3.3	|john


<a name="meta_datatypes_table"></a>
### 🔵 12.4 Meta / Data Type Table

Meta returns a table where each row is a column

```q
( [] company:(); employees:() )
meta t

/ create empty table with no types
/ c = column names
/ t = datatype (s = symbol, j = long)
/ f = foreign key
/ a = attributes
```
c|t|f|a
-|-|-|-
company|	|	|
employees|	|	|

```q
( [] company: `symbol$(); employees: `int$())

/ changed company type to s (symbol) and employees to i (integer)
```
c|t|f|a
-|-|-|-
company|	s	|	|
employees|	j	|	|

<a name="countrowsimple_table"></a>
### 🔵 12.5 Count Row Table

company | employees
-|-
ford |	300
bmw	| 100

```q
count t
2

/ counts number of rows in table
```

```q
cols t
`company`employee

/ returns list of all columns
```

<a name="rename_column_table"></a>
### 🔵 12.6 Rename Column Table xcol

```q
`a`b xcol t

/ renamed first 2 columns from company/employee to a/b
```

a | b
-|-
ford |	300
bmw	| 100

<a name="add_column_table"></a>
### 🔵 12.7 Add Column

```q
select company, employees, newval: 101 from t

/ select will retrieve columns as values
/ if you select a column that doesnt exist, it will add it (newval)
```
company | employees | newval
-|-|-
ford |	300 | 101
bmw	| 100 | 101

<a name="sort_column_table"></a>
### 🔵 12.8 Sort Column Table (xasc)

```q
`employees xasc t

/ will sort ascending by employees
```
company | employees | newval
-|-|-
bmw	| 100 | 101
ford |	300 | 101

<a name="union_table"></a>
### 🔵 12.9 Union Table

Table t

company | employees
-|-
ferrari| 100
ford |	100 
rover| 100

Table u

company | employees
-|-
ferrari| 100
bmw |	5 
ford| 5

```q
t union u

/ returns values that are same (ferrari 100). does NOT dupe same values.
/ any values that do NOT equal, adds as new row

```
company | employees
-|-
ferrari| 100
ford | 100 
rover| 100
bmw |	5 
ford| 5

<a name="except_table"></a>
### 🔵 12.10 Except Table

```q
t except u

/ from table t, check table u for any key + value matches, and remove
/ ferrari 100 appears in both tables, hence removed
/ then returns remaining rows in table t
/ in table u, bmw + ford aren't matches, so ignored
```
company | employees
-|-
ford| 100
rover | 100 

<a name="inter_table"></a>
### 🔵 12.11 Inter Table

```q
t inter u

/ only returns rows from both table t and u that match
```
company | employees
-|-
ferrari| 100

<a name="distinct_table"></a>
### 🔵 12.12 Distinct Table

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

/ will return distinct values per row
```
a|b
-|-
1|	1
2	|3


<a name="retrieve_table"></a>
### 🔵 12.13 Retrieve From Table

Table t:

company | employees
-|-
ferrari| 100
ford | 100 
rover| 100
bmw |	5 
ford| 5

```q
select from t

/ retrieves all columns from table t
```
company | employees
-|-
ferrari| 100
ford | 100 
rover| 100
bmw |	5 
ford| 5

```q
select company from t

/ only retrieves the company column
```

company | 
-|
ferrari| 
ford |  
rover| 
bmw |	 
ford| 

```q
select from t where company = `ford

/ retrieves rows where company = ford 
```

company | employees
-|-
ford | 100 

```q
t [`employees]

/ retrieves column= employee as a row
```
100 100 100 5 5 

```q
t [`employees] - : 100

/ -100 from every value in column employee
```
company | employees
-|-
ferrari| 0
ford | 0 
rover| 0
bmw |	-105 
ford| -105

```q
t [ 0 1]
or
2#t

/ returns first 2 rows
```
company | employees
-|-
ferrari| 0
ford | 0 


```q
-3#t

/ returns last 3 rows
```

company | employees
-|-
rover| 0
bmw |	-105 
ford| -105

```q
2 ? t

/ randomly selects 2 rows from table
```

company | employees
-|-
rover| 0
ford| -105

<a name="insert_table"></a>
### 🔵 12.14 Insert Table

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

<a name="operations_table"></a>
### 🔵 12.15 Operations on Tables

With KEYED tables, you can use arithmetic between tables

```q
t1: ([sym: `a`b`c] num: 1 2 3)
t2: ([sym: `a`b`c] num: 1 1 1)
t1+t2

/ both tables have to be keyed
/ column names have to match
```

sym | num
-|-
a | 2
b | 3
c | 4


```q
/ if UNKEYED, can only do math on tables with numeric fields

t1: ([] sym: 1 2 3; num: 1 2 3)
t2: ([] sym: 1 1 1; num: 1 1 1)
t1+t2

/ will find the column names that match, and add values together
/ column names that dont match will be union joined as a new column
```

sym | num
-|-
2 | 2
3 | 3
4 | 4

<hr>

<a name="tables_problem_set"></a>
# 🔴 13. Tables Problem Set
[Top](#top)

**🔵 Given:**

```q
stock: ( [] sym: `MS`C`AAPL; sector:`Financial`Financial`Tech; employees: 100 100 100)
```
sym|sector|employees
-|-|-
MS	|Financial|	100
C	|Financial	|100
AAPL|	Tech	|100

**🔵 13.1 Extract the employees numbers (without the header)**

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

**🔵 13.2 Key the first column in stock table (above)**

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

**🔵 13.3 Display only the first and second rows of the stock table**

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

**🔵 13.4 Select the last row of stock table as a dictionary**

```q
last stock
```
key |value
-|-
sym |`AAPL
sector | `Tech
employees | 100

<hr>

**🔵 13.5 Insert GOOG in the tech sector with 100 employees**

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

**🔵 13.6 Given:**

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

**🔵 13.6 Find the average height of the bosses, the employees, and both the bosses and employees**

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

**🔵 13.7 Find the 2 tallest employees**
```q
2#`height xdesc employees
```
name|height
-|-
jim	|180
john|	170

* take 2 from employees table, sorted descending by height

<hr>

**🔵 13.8 Given the 2 tables:**

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

**🔵 13.9 Insert the following record into stock**
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

**🔵 13.10 In the stock table, change the number of employees for C to 300**

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
## 🔴 14. Keyed Tables
[Top](#top)

<a name="single_keyed_table"></a>
### 🔵 14.1 Single Keyed Table

```q
( [id: `a`b`c`e] name:`jane`jim`kim`john; employer:`citi`citi`ms`ts; age: 11 22 33 44)

/ the [ ] square bracket holds the key columns
```

id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	john|	ts|	15

<a name="multi_keyed_table"></a>
### 🔵 14.2 Multi Keyed Table

```q
kt: ( [id:`a`b`c`d; name:`jane`jim`kim`john] employer:`citi`citi`ms`ts; age: 11 22 33 44)

/ columns id and name are both keyed columns
```

id|name|employer|age
-|-|-|-
`a`|	`jane`|	citi|	11
`b`|	`jim`|	citi|	22
`c`|	`kim`|	ms|	13
`e`|	`john`|	ts|	15

<a name="retrieving_keysvalues"></a>
### 🔵 14.3 Retrieving Keys/Values

```q
key kt

/ retrieves key columns
```

id|name
-|-
a	|jane
b	|jim
c	|kim
d	|john

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
### 🔵 14.4 Changing Keys

Table kt

id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	john|	ts|	15

/ only id column is keyed for now

```q
`id`name xkey `kt

/ changed key columns to both id and name
/ use backtick kt to change underlying table
```

id|name|employer|age
-|-|-|-
`a`|	`jane`|	citi|	11
`b`|	`jim`|	citi|	22
`c`|	`kim`|	ms|	13
`e`|	`john`|	ts|	15

<a name="adding_keys"></a>
### 🔵 14.5 Adding Keys

```q
1!kt

/ adds first column as a key
```
id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	john|	ts|	15

<a name="removing_keys"></a>
### 🔵 14.6 Removing Keys

```q
() xkey `kt
or
0!kt
```

id|name|employer|age
-|-|-|-
a|	jane|	citi|	11
b|	jim|	citi|	22
c|	kim|	ms|	13
e|	john|	ts|	15

<a name="upsert_keys"></a>
### 🔵 14.7 Upserting Keys

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

/ if key exists and matches, updates value
/ if new key, adds new row
/ since key e already exists, overrides values for name, employer, age
/ must make sure underlying keyed columns match, otherwise error. (1 keyed col vs 2 keyed col)
```

id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	dan|	walmart|	200
`f`|	kate|	walmart|	200

```q
upsert [`kt; ( [id:`f`g] name:`ron`allen)]

/ f was updated to ron, and since no employer or age info, pulled from existing kt table (kate's old row)
/ g is new key, so adds new row. since no info, returns null
```

id|name|employer|age
-|-|-|-
`a`|	jane|	citi|	11
`b`|	jim|	citi|	22
`c`|	kim|	ms|	13
`e`|	dan|	walmart|	200
`f`|	ron|	walmart|	200
`g`|	allen|	|	

<a name="upsert_multi_rowkeys"></a>
### 🔵 14.8 Upserting Multi Rows/Keys

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

/ updated kx, NY to 9 (overrides prev value)
/ since there was no ms, SG, adds new row 
```

employer|loc|size|area
-|-|-|-
`kx`|	`NY`|	9|	1
`ms`|	`NY`|	20|	2
`ms`|	`HK`|	30|	3
`ms`|	`SG`|	10|	

<a name="retrieve_value_keys"></a>
### 🔵 14.9 Retrieving Values from Keyed Table

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
## 🔴 15. Keyed Tables Problem Set
[Top](#top)

**🔵 15.1 Create the following keyed table**

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

**🔵 15.2 Retrieve entries where book is B, using select**
```q
select from p where book=`B
```
book | ticker|size
-|-|-
`B`| `AAPL`| 200
`B`| `MS`| 300

<hr>

**🔵 15.3 Retrieve entries where book is C and ticker is c, using take**
```q
( [book:enlist`C; ticker:enlist`C]) # p
```
book | ticker|size
-|-|-
`C`| `C`| 400

* underlying table p has 2 keyed columns (book and ticker)
* you cannot retrieve 2 keyed columns if underlying table only has 1 key column

**🔵 15.4 Upsert the following values**

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
## 🔴 16. Table Attributes
[Top](#top)

<a name="set_attribute_creation"></a>
### 🔵 16.1 Setting Attributes During Creation
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
### 🔵 16.2 Applying Attribute to Existing Data
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
### 🔵 16.3 Clear Attributes
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
### 🔵 16.4 Sorted Attribute
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
### 🔵 16.5 Unique Attribute
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
### 🔵 16.6 Grouped Attribute
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
### 🔵 16.7 Parted Attribute
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
## 🔴 17. Foreign Key Restrictions
[Top](#top)

* Foreign keys restrict the values that are allowed in a column

<a name="single_fkey"></a>
### 🔵 17.1 Single Foreign Keys

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
### 🔵 17.2 Checking Foreign Keys

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
### 🔵 17.3 Upserting with Foreign Keys
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
### 🔵 17.4 Retrieving Columns via fkey
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
### 🔵 17.5 Multiple Foreign Keys
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

**4 Types of Queries**

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
* select/update/exec/delete - the columns(original or modified by functions) returned
* from t - from table you want to run the query on
* where c - apply filtering conditions
* by b - group by columns b

### 🔸 Select Template
* the result of a select statement is a table

### Example Where subphrases
```q
select from trade where size>300, price>100
select from trade where sym in `AAPL`GOOG
select from trade where price within (200:300)
select from trade where (price>100) and size>300
select from trade where (price>100) or size> 300
select i, sym, price from trade where i>5
select price, i by sym from trade
```

### Analytics on Grouped Data
```q
select max price by sym from trade
select price by sym from trade
ungroup select price by sym from trade
```

### xbar
rounds right argument down to nearest multiple of left argument
```q
7 xbar 10 20 30 40 50
7 14 28 35 39
```
```q
5 xbar 11:00 + 0 3 5 11
11:00 11:00 11:05 11:10
```
remember, it evaluates right to left (so 11+0 3 5 11), then does 5 xbar
```q
select price by sym, 240 xbar time.minute from trade
```
```q
select avg price by sym, 240 xbar time.minute from trade
```

### 🔸 Exec Template
* exec from one column returns a list
* exec from more than one column returns a dictionary
* one diff between select and exec is the column lists do not have to be rectangular to return a result

```q
exec sym from trade
`GOOG`GOOG`MSFT
```
```q
exec sym, price, size from trade
```
* exec from multiple columns returns a dictionary
```q
exec price by sym from trade
```
exec with single column with by clause returns a dictionary


### Select vs Exec
```q
cnc: ([] city:`toronto`london`ny`vancouver; country:`canada`england`usa`canada)
```
city | country
-|-
toronto|	canada
london	|england
ny|	usa
vancouver|	canada

```q
exec city, distinct country from cnc
```
key|value
-|-
city|	toronto london ny vancouver
country|	canada england usa

```q
select city, distinct country from cnc
```
error because select expects the columns to have the same length

### 🔸 Update Template
* update phrase updates a pre-existing column in t with value evaluated with an assignemtn
* if column doesnt exist, gets joined to the result at the end of column list
* original table unaffected unless the data is persisted by using backtick

```q
update price: 10.0 from trade
```
this will update all prices to 10
```q
update price:10.0 from trade where sym in `AAPL`GOOG
```
this will update prices to 10 for AAPL and GOOG 
uses where clause - updates only the filtered records

```q
update vol:price*size from trade where sym in `AAPL`GOOG
```
new column vol is added 

```q
update price:avg price by sym from trade where sym in `AAPL`GOOG
```
updates the price to average price, grouped by sym 

<a name="select_template"></a>
### 🔵 19.1) Select Template

```q
select a by b from t where c

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

* select [] can be used to get the first n or last n records of a table
* select [n m] can be used to get records starting from n and upto count m from n

```q
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
### 🔵 19.5) Select from where

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
### 🔵 19.6) Select By

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
### 🔵 19.7) Select Count 

```q
select count i, max prirce by date, time.hh from trade where sym=`RBS
```
date|hh|x|prrice
-|-|-|-
`2021-05-29`|	`9`|	645 |	50.5 
`2021-05-30`|	`10`	|154	| 50.0

* i is a virtual column that returns the number of rows (as column x)

<a name="using_ops_functions"></a>
### 🔵 19.8) Using Operations and Functions 

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
### 🔵 19.9) In Function

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
### 🔵 19.10) Within Function

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
### 🔵 19.11) Xbar Function
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
### 🔵 19.12) Exec Query

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
### 🔵 19.13) Update

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
### 🔵 19.14) Delete Columns
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
### 🔵 19.15) Delete Rows
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

* fby aggregates values from one list based on group defined in another
* (aggr;d) fby g
* aggr = aggregate function = max, min, sums, etc.
* d = column name
* g = another column name

```q
(sum;price) fby sym
(sums;price) fby sym
(max;price) fby sym
(last;price) fby sym
(first;price) fby sym
(max;price) fby sym
(avg;price) fby sym
```

```q
price = (last;price) fby sym
price < (last;price) fby sym
price > (last;price) fby sym
```

### fby Example 1

```q
city:`NY`NY`LA`SF`LA`SF`NY
temp:32 31 75 69 70 68 12

(min;temp) fby city
/ returns
/ 12 12 70 68 12
```
so this calculates the min temp for every city (12 for NYC)


### fby Example 2

Given the following table, find the max price per symbol

time | sym | src | price | size
-|-|-|-|-
2019-03-11 |	GOOG |	L|	36.01|	1427
2019-03-11 |	GOOG |	O|	36.01|	708
2019-03-11 |	MSFT |	N|	35.5|	7810
2019-03-11 |	MSFT |	O|	31.1|	1100

```q
select from t where price=(max;price) fby sym
```
time | sym | src | price | size
-|-|-|-|-
2019-03-11 |	GOOG |	L|	36.01|	1427
2019-03-11 |	GOOG |	O|	36.01|	708
2019-03-11 |	MSFT |	N|	35.5|	7810

* this is not correct, since there are still 2 GOOG (since both same "max" price)
* you can add another fby filter for time

```q
select from t where price=(max;price) fby sym, time=(max;time) fby sym
```
time | sym | src | price | size
-|-|-|-|-
2019-03-11T09:00:04.123000	GOOG	O	36.01	708
2019-03-11T09:00:08.123000	MSFT	N	35.5	7810

* in this case, you filtered max price by sym, and max time by sym

```q
update num: (sums;num) fby sym from`sym`time xasc timeline
```
* aggregate running sums by sym
* backtick sym, time xasc timeline sorts the timeline table ascending first by sym, then by time

<hr>

<a name="qsql_problem_set"></a>
## 🔴 20. qSQL Problem Set
[Top](#top)

**🔵 1. Extract from trade table, trades for MS greater than 1,000 in size**

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

**🔵 2. From the trade table, find the total size of all trades and the average price paid per sym**

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

**🔵 3. From the trade table, find the trade that was largest size for each sym**

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

**🔵 4. From the trade table, select the latest trade for each sym, and include all details**

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

**🔵 5. Find all trades that have sym GOOG**

```q
select from trade where sym=`GOOG
```
sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	87.54| 49100 | B
GOOG|	2021-06-03|	87.54| 49100 | C

<hr>

**🔵 6. Find all trades that have sym GOOG or RBS or A**

```q
select from trade where sym in `GOOG`RBS`A
```
sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	87.54| 49100 | B
RBS|	2021-06-03|	87.54| 49100 | C
A|	2021-06-03|	87.54| 49100 | C

<hr>

**🔵 7. Find all trades for google that had a price between 70 and 80**

```q
select from trade where sym=`GOOG, price within 70 80
```

sym|date|price|size|cond
-|-|-|-|-
GOOG|	2021-06-03|	72 | 49100 | B
GOOG|	2021-06-03|	75| 49100 | C
GOOG|	2021-06-03|	78 | 49100 | C

<hr>

**🔵 8. Count the number of trades and total size of trades per hour for sym RBS**

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

**🔵 9. Select the number of trades and total size of trades every 30 mins for the sym RBS**

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

**🔵 10. Find all trades for `A where the price was cheaper than the average for that day**

```q
a: update avgPrice: avg price by date from select from trade where sym=`A
```

<hr>

<a name="qsql_joins"></a>
## 🔴 21. qSQL Joins
[Top](#top)

<a name="left_join"></a>
### 🔵 qSQL Join Left 

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
### 🔵 qSQL Plus Join 

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
### 🔵 qSQL Inner Join 

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
trade ij stock
```
* adds columns where the key matches (sym), otherwise remove

x|date |        sym|  price|    size  | sector | employees
-|-----|-----------|---------|------| -|-
1|2021.06.03| C   | 107.2018| 63500| Tech | 100
2|2021.06.03| MSFT |96.87488| 1700| Tech | 100

* removes row UBS since no match

<a name="union_join"></a>
### 🔵 qSQL Union Join 

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


<a name="qsqljoins_problem_set"></a>
## 🔴 22. qSQL Joins Problem Set
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

**🔵 1. Find the total value of trades by sector, include those who's sector is unknown (totalvalue = price x size)**

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

**🔵 2. Combine trades from trade and fbTrades Table into a table t2, sorted by date. Include all columns**

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

**🔵 3. Find the highest and lowest price in the trade table for each sym**

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

**🔵 4. Find the 2 highest trade prices for each sym**

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

**🔵 5. Find the average daily price for each sym in trade table. Join the newsItems table to show only those items where the sym had a newsItem on that date**

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

**🔵 6. Take the newsItems table and join the trade table to bring in the latest price for each ticker**

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

<a name="timeseries_joins"></a>
## 🔴 23. Timeseries Tables Joins
[Top](#top)

<a name="asof_join"></a>
### 🔵 Asof Time Join
* joins the closest matches from one table to another
* syntax = aj [column; source table; lookup table]
* last item of columns will be less than or equal join

```q
t: ( [] time: 07:00 08:30 09:59t; sym:`a`a`b; price: 0.9 1.5 1.9; size:100 200 300)
q: ( [] time: 08:00 09:00 10:00t; sym:`a`b`a; bid: 1 9 4)
```
table t

time|sym|price|size
-|-|-|-
07:00:00.000|	a|	0.9|	100
08:30:00.000|	a|	1.5|	200
09:59:00.000|	b|	1.9|	300

table q

time|sym|bid
-|-|-
08:00:00.000|	a|	1
09:00:00.000|	b|	9
10:00:00.000|	a|	4

```q
aj [`sym`time; t;q]
```
* syntax = aj [column; source table; lookup table]
* columns = sym, time
* t = source table
* q = lookup table
* column names must match

time|sym|price|size|bid
-|-|-|-|-
07:00:00.000|	a|	0.9|	100|	
08:30:00.000|	a|	1.5|	200	|1
09:59:00.000|	b|	1.9|	300	|9

* bid column pulled in
* from trade table, look through each sym, then time (less than or equal to)
* from trade, found a, but in q, no time less than or equal to 7:00am. so bid = null
* from trade, found a, found 8:00am <= 8:30, so bid = 1
* from trade, found b, found 9:00am <=9:59, so bid = 9

```q
fq: update qtime:time, qsym: sym from q
ft: update ftime:time, fsym:sym from t
```
* create new table fq with columns qtime and qsym
* create new table ft with columns ftime and fsym

table fq

time|sym|bid|qtime|qsym
-|-|-|-|-
08:00:00.000|	a|	1|	08:00:00.000|	a
09:00:00.000|	b|	9|	09:00:00.000|	b
10:00:00.000|	a|	4|	10:00:00.000|	a

table ft

time|sym|price|ftime|fsym
-|-|-|-|-
07:00:00.000|	a|	0.9|	100|	07:00:00.000|	a
08:30:00.000	|a|	1.5|	200|	08:30:00.000|	a
09:59:00.000	|b|	1.9|	300|	09:59:00.000|	b

```q
aj [`sym`time;ft;fq]
```
* ft = source table
* fq = lookup table

time|sym|price|size|ftime|fsym|bid|qtime|qsym
-|-|-|-|-|-|-|-|-|
07:00:00.000|	a|	0.9|	100|	07:00:00.000|	a	|		| |
08:30:00.000|	a|	1.5	|200|	08:30:00.000|	a	|1	|08:00:00.000|	a
09:59:00.000|	b|	1.9	|300|	09:59:00.000|	b|	9	|09:00:00.000|	b

 * aj0 is the same as aj, but uses the lookup tables time column

<a name="uniontime_join"></a>
### 🔵 Union Time Join

* union join combines all entries from both tables, then can sort by time

```q
q uj t
```
time|sym|bid|price|size
-|-|-|-|-
08:00:00.000|	a|	1|	| |	
09:00:00.000|	b|	9|	| |
10:00:00.000|	a|	4| | |
07:00:00.000|	a|		|0.9|	100
08:30:00.000|	a|		|1.5|	200
09:59:00.000|	b|		|1.9|	300

```q
`time xasc q uj t
```
time|sym|bid|price|size
-|-|-|-|-
07:00:00.000|	a|		|0.9|	100
08:00:00.000|	a|	1|		|
08:30:00.000|	a|		|1.5|	200
09:00:00.000|	b|	9|		|
09:59:00.000|	b|		|1.9|	300
10:00:00.000|	a|	4|		|


<a name="windowtime_join"></a>
### 🔵 Window Time Join

* wj pulls in values from that time window

Given:

table t:

time | sym | price
-|-|-
09:00:00.000 |	a|	10.0
09:04:00.000|	a	|11.0
09:12:00.000|	a	|12.0
09:13:00.000|	a	|13.0

table q:

time|sym|bid
-|-|-
09:00:00.000|	a|	10.0
09:01:00.000|	a	|10.0
09:02:00.000|	a|	11.0
09:03:00.000|	a|	13.0
09:04:00.000|	a|	13.0
09:05:00.000|	b|	14.0
09:06:00.000|	b|	14.0
09:07:00.000|	b|	15.0
09:08:00.000|	a|	15.0
09:09:00.000|	a|	17.0
09:10:00.000|	a|	17.0
09:11:00.000|	a|	18.0
09:12:00.000|	a|	18.0

```q
windows:flip t.time +\: -00:02 00:02t
```
08:58:00.000t;09:02:00.000t;09:10:00.000t;09:11:00.000t);(09:02:00.000t;09:06:00.000t;09:14:00.000t;09:15:00.000t

* from table t, produce a time interval 2 mins +\- for each row of time
* pairs of time values to specify the interval time values


```q
wj[windows;`sym`time;t;(q;(::;`bid))]
```

time|sym|price|bid
-|-|-|-
09:00:00.000|	a|	10.0|	10 10 11f
09:04:00.000|	a|	11.0|	11 13 13f
09:12:00.000|	a|	12.0|	17 18 18f
09:13:00.000|	a|	13.0|	18 18f

* wj will output same number of rows as original table t
* windows - interval pairs you created
* columns you want to match on (sym, time) within source table t
* start new list, look up values from table q (lookup table)
* :: = return all values from the bid column
* 1st row, looks up in table q, any syms (a) from 8:58 to 9:02, and returns the bid
* 2nd row, looks up in table q any syms (a) from 9:02 to 9:06, and returns the bid 

```q
wj[windows;`sym`time;t;(q;(::;`bid); (avg;`bid); (count;`bid))]
```
* can perform functions! 

time | sym | bid | bid
-|-|-|-
09:00:00.000|	a|	10.0|	10 10 11f	3
09:04:00.000|	a|	11.0|	11 11 13f	3
09:12:00.000|	a|	12.0|	17 17 17f	3
09:13:00.000|	a|	13.0|	17 17f	2


wj vs wj1
* wj pulls in prevailing values not within time window
* wj1 strictly excludes values outside the interval (for ex, if time interval was 10:00 - 10:15)


<a name="adverbs_header"></a>
## 🔴 24. Adverbs
[Top](#top)

<a name="eachboth_adverbs"></a>
### 🔵 Each Both ,'
* modifies a dyadic function to operate on corresponding pairs of items between lists of equal length
* acts like concatenate between 2 lists

### EACH BOTH - 2 lists of integers

```q
L: 1 2 3
K: 50 60 70
L,'K
```
(1 50;2 60;3 70)

L|K
-|-
1| 50
2 |60
3 |70

* concatenates the first elements of L and to first element of K
* lists must be same length

### EACH BOTH - 2 dictionaries

```q
d1:`p`o`i ! 1 2 3
d2:`p`o`k ! 4 5 6
```
d1
key|value
-|-
p|	1
o|	2
i|	3

d2
key|value
-|-
p|	4
o|	5
k|	6

```q
d1,d2
```
key|value
-|-
p	|4
o	|5
i	|3
k	|6

* when you simply JOIN dictionaries, the d2 will override anything existing keys in d1 (p, o)
* acts like an UPSERT

```q
d1,'d2
```
key|value
-|-
p|	1 4
o|	2 5
i|	3 
k| 6

* EACH BOTH will join the values together
* retains the keys, and combines the values together

### EACH BOTH - Tables

```q
t1: ( [] a:1 2 3)
t2: ( [] b:4 5 6)
```

```q
t1, t2
```
can't simply join; mismatch (because rows have different columns names)

```q
t1, 't2
```

a|b
-|-
1	|4
2	|5
3	|6

* each both will stitch the two tables together


<a name="each_monadic"></a>
### 🔵 Each Monadic

each modifies a monadic function to make it operate one level deeper

```q
j: ("race fast, safe car."; 0 1 2; `a`b`c)
```
"race fast, safe car." \
0 1 2 \
a b c

```q
reverse j
```
so this reverses the mixed list at the top most level

a b c \
0 1 2 \
"race fast, safe car."

```q
reverse each j
```
reverse within each list

".rac efas , tsaf ecar"
2 1 0
c b a

<a name="eachright_eachleft"></a>
### 🔵 Each Right / Each Left
* similar to concatenate
* x,/: each right; will join left item (x) to each item on right
* x,\: each left; will join left item (x) to each item on left

### each left ,\:
x, \:y / each left, returns a list of each element from x with all of y
so pegs to x (left) to each element of y (right)

```q
l: 1 2 3
k: `a`b`c
l,\:k

/ returns:
/ 1`a`b`c
/ 2`a`b`c
/ 3`a`b`c
```

### each right ,/:
x,/:y / each right, returns a list of all the x with each element of y
so pegs to y (right) to each element of x (left)

```q
l: 1 2 3
k: `a`b`c
l,/:k

/ returns:
/ 1 2 3`a
/ 1 2 3`b
/ 1 2 3`c
```

```q
st:("welcome";"to the"; "terminal")
```
"welcome" \
"to the " \
"terminal" 

```q
">",/:st
```
* joins the left item to each item on right

">welcome" \
">to the " \
">terminal" 

```q
">",st
```
* if you simply joined it, it will join it at the top most level of the list

">" \
"welcome" \
"to the " \
"terminal" 

```q
1 2 +/: 100 200 300
```
* each right; since 2 arguments on left, there will be 2 columns

key | value
-|-
101 | 102
201 | 202
301 | 302

```q
1 2 +\: 100 200 300
```
* each left (the bar tilts towards left); since 3 arguments on right, there will be 3 columns

key | value
-|-
101 | 201 | 301
102 | 202 | 302

```q
st, \:"--->"
```
* each left; adds right hand argument to each of st

"welcome--->" \
"to the---> " \
"terminal--->" 

<a name="scan_adverb"></a>
### 🔵 Scan
* useful for calculations such as running totals, running products, where the previous value is used in the next value calculation

```q
{x + y} \ [1 2 3 4 5]
{x + y} scan [1 2 3 4 5]
```
* 1+0 =1; 1+2 = 3; 3+3=6; 4+6=10; 5+10=15
* can also use "scan" instead of \

1 3 6 10 15

```q
{x,y} \ [1 2 3 4 5]
```
1 \
1 2 \
1 2 3 \
1 2 3 4 \
1 2 3 4 5

<a name="eachprevious_adverb"></a>
### 🔵 Each Previous

```q
{x+y}': [1 2 3 4 7]
```
0N 3 5 7 11

* O + 1 = ON
* 1 + 2 = 3
* 2 + 3 = 5
* 3 + 4 = 7

```q
10 + ': 1 2 3 4 7
```
11 3 5 7 11
* 10 + 1 = 11
* 1 + 2 = 3
* 2 + 3 = 5
* 3 + 4 = 7

<hr>

<a name="adverbs_problemset"></a>
## 🔴 25. Adverbs Problem Set
[Top](#top)

## 🔵 1. Given: ("cow"; "fox";"badger") use EACH RIGHT to prepend "the" before each item##

```q
strs: ("cow";"fox";"badger")
"the" ,/: strs
```
"the cow" \
"the fox" \
"the badger"

* x / y = add x to the left of y

<hr>

## 🔵 2. Use EACH LEFT to add "jumped" to strs ##

```q
strs,\: " jumped"
```
"cow jumped" \
"fox jumped" \
"badger jumped"

* the \: (top points left, so each left). 

<hr>

## 🔵 3. Given the nested list: dd: (1 5 10; 200 30 40; 20 23 24), find the max of each list ##

```q
dd: (1 5 10; 200 30 40; 20 23 24)
max each dd
```
10 200 24

<hr>

## 🔵 4. Using EACH PRIOR, create a function that calculates the moving sum with window size of 2 ##

```q
L: 20 30 4 6 1 2
+': [L]
20 50 34 10 7 3

alternatively:

```q
2 msum L
```
 or 
 
 ```q
 {x+y}': [L]
 
```

<hr>

## 🔵 5. Use EACH BOTH to join the lists to give (5 8; 7 3; 9 4) ##

numbers: 5 7 9 \
powers: 8 3 4

```q
numbers, 'powers
```
key| value
-|-
5| 8
7| 3
9| 4

<hr>

## 🔵 6. Use EACH BOTH to raise 5 to the power of 8, 7 to the power of 3, etc. ##

```q
numbers xexp' powers
```
390625 343 6561f

<hr>

## 🔵 7. A bank account pays 5% interest a year. Write a function that takes the current balance and returns the new balance after one year. Then use scan\ with that function to display the interest every year, up to 7 years in the future ##

assume starting balance of 100

```q
{x * 1.05} 100
```
105

```q
{x * 1.05} \ [7; 100.]
```
105 \
110.25\
115.7625

* use monadic version of scan that takes 2 arguments
* first argument = how many times to run
* second argument = starting value for function

<hr>

## 8. Create a function, fib, that takes a fibonnaci sequence as its argument and returns the sequence complete with the next entry ##

```q
fib: {x, sum -2#x}
fib 1 1
```
1 2 3

<hr>

## 🔵 9. Use the over function to create a function fibn to generate a fib sequence n numbers long where n is the functions argument ##

```q
fibn: {x fib/ 1 1}
fibn 5
```
1 1 2 3 5 8 13

<hr>

<a name="importexport_header"></a>
## 26. 🔴 Importing and Exporting / Saving Data
[Top](#top)

<a name="txt_import"></a>
### 🔵 26.1) Importing TXT files

Assume you have a txt file in your directory called test.txt

```q
hopen `:test.txt
read0 `:test.txt
```

* file handler = a temporary reference number that an OS assigns to a file requested by a user to be opened
* hopen function will open the txt file
* read0 function will read the txt file

<a name="txt_export"></a>
### 🔵 26.2a) Exporting / Saving TXT files

to write to txt, simply use hopen to get the file handle, store the file handle, and store strings to it

```q
fh:hopen `:hi.txt
fh "10"
fh "20"
neg[fh] "30"
read0 `:hi.txt
```
"1020" \
"30"

* by putting neg[fh], you enter into a new line

```q
hclose fh
```
closes the file handle so you can no longer edit it


<a name="tables_exportformat"></a>

### 🔵 26.2b) Saving TXT files
There are 2 ways to save to text: save function or 0 operator

1) save function (save `name.csv)
2) 0: operator 
 
0: is more flexible and powerful, allowing selection of a table subset and any name of file desired.
The benefit of exporting to CSV is that for transferring data to other systems their support is ubiquitous. However the space requirement of converting each digit of a number to separate characters is significant.

trade

date |       time |        sym|  price |   size | cond
-|-|-|-|-|-
2013.09.28| 09:30:02.553 | C |   107.2018 | 63500 | B
2013.09.28| 09:30:02.701| MSFT | 96.87488 | 1700  | B
2013.09.28| 09:30:02.743| RBS |  97.11338 | 80700 | C
2013.09.28| 09:30:02.758| A   | 100.35    | 50300 | B
2013.09.28| 09:30:02.907| B   | 55.82187  | 92700 | A

```q
save `trade.csv
/ syntax is save backtick filename.csv
/ this will be saved to your q folder
```

```q
";" 0: trade / converts table to list of strings separated by semi colons
`newfilename.csv 0: ";" 0: trade / saves to csv file
```

0: allows you to choose custom separaters and file names
; is what you are separating items with
trade = table name


### 🔵 26.3) Exporting / Saving tables as txt, csv, excel, and xml files

Given table cars:
```q
cars: ( [] maker: `Ford`Tesla`Honda; price: 100 200 300; weight: 1000 2000 3000)
```
maker|price|weight|
-|-|-
Ford|	100|	1000
Tesla|	200|	2000
Honda|	300|	3000

```q
save `cars.txt
save `cars.csv
save `cars.xls
save `cars.xml
```
* this will automatically save and export your table to any of the file types in your directory

```q
save `$"newdir/cars.txt"
```
* this will create a new filepath and directory for your file to save your file
* the new folder will be called "newdir"

<a name="export_tablenewname"></a>
### 🔵 26.4) Exporting / Saving tables with a new name

```q
`carsnewname.csv 0: "," 0: cars
```
maker,price,weight \
Ford,100,1000 \
Tesla,200,2000 \
Honda,300,3000

* by using the 0: function, you can rename your file to anything you want (carsnewname)

<a name="csv_import"></a>
### 🔵 26.5) Importing CSV Files

Assume you have a file called nyse_20110621.csv on your computer

```q
("**********"; ",") 0: `:nyse_20110621.csv
```
* so the 0: loads the file on the right hand side
* the **** are just KDB datatype layers; one * for each column
* this will interpret all values as strings, allowing for easy way to check the data

"symbol" | "A"
-|-
"date" |"21-june-2011"
"open" | "14.94"
"high" | "15.94"
"low" |"13.43"
"close" | "24.52"
"volume"| "100"

```q
("SSFFFFJ"; ",") 0: `:nyse_20110621.csv
```
* replace the * with the datatype (string string, float float, long etc)
* interprets the values more sensibly

symbol | A
-|-
date |21-june-2011
open | 14.94
high | 15.94
low |13.43
close | 24.52
volume| 100

```q
("SSFFFFJ"; enlist ",") 0: `:nyse_20110621.csv
```
* by adding in the enlist, you are treating the first column as a header
* converts it into a table

symbol | date | open | high | low | close | volume
-|-|-|-|-|-|-
A|	21-Jun-2011|	48.7|	50.32|	48.67|	49.82|	3509600
AA|	21-Jun-2011|	14.94	|15.42|	14.92|	15.37|	18310600


<a name="binaryfile_export"></a>
### 🔵 26.6) Saving to Binary Files
Binary files are a direct byte stream that is similar to kdb's in-memory representation of data. 
Features include:

1) Requires significantly less space than a text file (kdb+ supports compression) 
2) Quicker to save load
3) Reading / writing is simply streaming bytes, it is extremely fast.
4) We use get / set to read/write.
5) You can append and upsert.
6) Once loaded in, the entire entity is stored in memory.

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

Assume dictionary d
```q
d: `p`o`i!1 2 3

set[`:q/dict;d]
/ this will save as dictionary d to your folder
```

<a name="binaryfile_export"></a>
### 🔵 26.7) Retrieving / Loading Binary Files

```q
get `:q/dict
/ this will load the dict dictionary 
```

key | value
-|-
p|	1
o	|2
i	|3






<a name="Splayedtable_header"></a>
## 27. 🔴 Splayed Table
[Top](#top)

* splaying a table in kdb+ allows saving a table with separate files for each column
* this reduces memory required as columns are only memory mapped as needed
* you cannot splay a table that is keyed! must 0! to remove key first

Given Table T:
```q
t: ([] a: 1 2 3; b: .z.d+1 3 5)
```
a|b
-|-
1|	2021-06-30
2|	2021-07-02
3|	2021-07-04


```q
set[`:splay/t/; t]
```
* set = saves binary / splayed tables
* first argument = file path. splay is the folder name (make sure you have / after t to SPLAY the table)
* t = the data you want to save
* the table (t) becomes a folder, and each column becomes a file
* the .d file is a list that contains the column names

```q
get `:splay/t/a
```
1 2 3

* the get syntax will return the values in that column

```q
get `:splay/t/.d
```
a b

* the .d file contains thhe name of all columns

Any sym column you want splayed must first be enumerated
enumerate = converting a list of values to a defined domain which restricts values to that domain

Assume trade table t

```q
sy: exec distinct sym from trade
```
C MSFT RBS A B BAC etc.

* exec will return your query in a single row (instead of column)

```q
update sym: `sy$sym from `trade
```
* this will enumerate all the syms from trade table to the domain of sy

```q
set[`:trade/; trade]
```
* now you can save your trade table as a splayed table

<hr>

<a name="casestudies_header"></a>
## 28. 🔴 Case Studies
[Top](#top)

<a name="load_csv"></a>
### 🔵 1. Loading CSV Files

With Column Headers

if a delimiter is enlisted, the first row of the csv file is read as a column header

```q
("SSJ"; enlist",")0: `sample.csv
```
* S=sym
* J=int

Without Column Headers

if the CSV file contains data but no column names, dont need to enlist a delimiter

```q
("SSJ";",") 0: `:sample.csv
```

<hr>

<a name="cross_case"></a>
### 🔵 2. Comparing Current Orders against Potential Crosses

Objectives:
1. Pull in CSV file of current orders (trade)
2. Pull in CSV file of proposed crosses (cross)
3. For each symbol, check opposing direction, and pull in quantity to cross
4. Create new column displaying shares that can cross
5. Retrieve columns in clean format to export back into csv


```q
t:("SSJ";enlist",") 0: `:trade.csv
```
t 

ric| side | qty
-|-|-
1810.HK|	Buy|	500
0700.HK|	Buy|	500
9988.HK|	Buy|	500
0001.HK|	Buy|	500
0016.HK|	Buy|	500
0151.HK|	Buy|	500
0005.HK|	Buy|	500


```q
c:("SSJ";enlist",") 0: `:cross.csv
```
c

ric | brokerside | brokerquantity
-|-|-
1810.HK|	Sell|	100
0700.HK|	Sell|	100
9988.HK|	Sell|	100
8888.HK|	Sell|	100
0016.HK|	Buy|	100
1234.HK|	Buy|	100
3033.HK|	Buy|	100

```q
1!`c
```
first set the RIC as a key column in cross file

```q
A: update crossableqty:?[side=brokerside;0N; qty - brokerquantity] from t lj 1!c
```
A

ric|side|qty|brokerside|brokerquantity|crossableqty
-|-|-|-|-|-
1810.HK|	Buy|	500|	Sell|	100|	400
0700.HK|	Buy|	500|	Sell|	100|	400
9988.HK|	Buy|	500|	Sell|	100|	400
0001.HK|	Buy|	500|	Sell|	100|	400

```q
A2: select from A where crossableqty > 0
```
ric|side|qty|brokerside|brokerquantity|crossableqty
-|-|-|-|-|-
1810.HK|	Buy|	500|	Sell|	100|	400
0700.HK|	Buy|	500|	Sell|	100|	400
9988.HK|	Buy|	500|	Sell|	100|	400
0001.HK|	Buy|	500|	Sell|	100|	400

```q
select ric, side, crossableqty from A2
```
ric|side|crossableqty
-|-|-
1810.HK|	Buy|	400
0700.HK|	Buy|	400
9988.HK|	Buy|	400
0001.HK|	Buy|	400

* this is the end result. these are the lines where you can cross 

<hr>

<a name="nettingbuyssells_case"></a>
### 🔵 3. Netting off buys and sells from same Stock

* same stock, multiple lines of buys and sells in the same stock
* determine what is the net quantity

Given
```q
t:([] ric:`AAPL; side:`buy`sell`sell`buy`buy; size:10 30 50 100 90)
```
ric | side |size
-|-|-
AAPL|	buy|	10
AAPL|	sell|	30
AAPL|	sell|	50
AAPL|	buy|	100
AAPL|	buy|	90

```q
select ?[side=`buy;size;neg size] by ric from t
```
ric | size
-|-
AAPL |	10 -30 -50 100 90

```q
select sum ?[side=`buy;size;neg size] by ric from t
```
ric | size
-|-
AAPL |	120

<hr>

## 🔵 4. Turn 2 lists of symbols into one longer list. 

```q
`AAPL`IBM`VOD and `O`N`L

/ expected outcome
AAPL.O IBM.N VOD.L
```

* convert syms O N L into strings
* add . to each element of O N L
* convert APPL IBM VOD into strings
* concatenate the 2 lists of strings together
* convert the strings back into symbols
* strings are NOT a datatype

```q
L1: `AAPL`IBM`VOD
L2:`O`N`L 

string L2 / convert from sym to string
/ ("O";"N";"L")

s2: ".",/: string L2 / using EACH RIGHT to add . to every element of O N L
/ (".O";".N";".L")

s1: String L1 / convert sym to string
/ ("AAPL";"IBM";"VOD")

S1,'S2 / using EACH BOTH joins each element of s1 to each element of s2
/ ("AAPL.O";"IBM.N";"VOD.L")

"S" $ (S1,'S2) / cast back to sym
/ `AAPL.O`IBM.N`VOD.L
```

* convert L1 and L2 to strings (so you can add . and later join)
* use EACH BOTH ADVERB to join each elemnt of S1 to each elemnt of S2
* cast the list of strings back to list of syms


<hr> 

## 🔵 5. Create a function that will return latest prices (with max timestamp within the date) for the date.
If there is not any price for that particular date, return the latest previous price
There is no predefined ordering of the source table.
Try to preserve the column order.

Given: 

```q
t: ([] date:raze (3#2016.01.06;4#2016.01.07;6#2016.01.08); sym:`a`b`c`a`b`a`b`a`b`c`a`b`c; price:1 2 3 1.1 2.1 1.2 2.2 1.3 2.3 3.2 1.4 2.4 3.3; timestamp:raze (3#2016.01.06T22:00:00.000; 2#2016.01.07T22:00:00.000; 2#2016.01.08T23:00:00.000; 3#2016.01.08T22:00:00.000; 3#2016.01.06T22:30:00.000))
```

Example 1:
f [t; 2016.01.06]

date | sym | price | timestamp
-|-|-|-
2016-01-06|	a|	1|	2016-01-06T22:00:00.000
2016-01-06|	b|	2|	2016-01-06T22:00:00.000
2016-01-06|	c|	3|	2016-01-06T22:00:00.000

Example 2:

f [t; 2016.01.07]

date | sym | price | timestamp
-|-|-|-
2016-01-06|	c|	3|	2016-01-06T22:00:00.000
2016-01-07|	a|	1.2|	2016-01-08T23:00:00.000
2016-01-07|	b|	2.2 |	2016-01-08T23:00:00.000

Example 3:

f [t; 2016.01.08]

date | sym | price | timestamp
-|-|-|-
2016-01-08|	a|	1.3|	2016-01-08T22:00:00.000
2016-01-08|	b|	2.3|	2016-01-08T22:00:00.000
2016-01-08|	c|	3.2|	2016-01-08T22:00:00.000

```q
f:{[t;d] select last price, max timestamp by date, sym from t where date<=d, timestamp=(max;timestamp) fby date, price=(last;price) fby sym}
```

* select last price, max timestamp
* set date, sym as keys
* date <=d means look for previous day if current date doesnt satisfy query conditions
* the FBY is the most important part of this problem. 
* the ORDER of the FBY also matters a lot. 
* you want to filter the LAST PRICE by sym, then
* you want to filter the MAX TIMESTAMP by the date


## 🔵 6. Given the 2 tables:

```q
t1: ([] sym:`a`b`c;ex:`x)
t2:([] ex:`y;sym:`a`b`c)

ps:(( [] sym:`a`b`c`a`b`c; ex:`x`x`x`y`y`y; price: 1.1 2.1 3.1 1.2 2 3.3); ( [] sym:`a`b`c`a`b`c; ex:`x`x`x`y`y`y; size: 200 100 300 200 50 200))
```

## Part 1: Join the first two tables using t1 schema ##

Desired Result:

sym | ex
-|-
a | x
b |x
c |x
a |y
b |y
c |y

```q
t3: t1,t2
```
sym | ex
-|-
a|	x
b|	x
c|	x
a|	y
b|	y
c|	y

## Part 2: Join list of tables to newly created table using sym and ex as a keys

Desired Result:

sym | ex | price | size
-|-|-|-
a|	x| 1.1 | 200
b|	x|2.1|100
c|	x|3.1|300
a|	y|1.2|200
b|	y|2|50
c|	y|3.3|200

```q
ps1:2!first ps
ps2:2!last ps
```
* you want to split up list of tables ps into 2 separate tables by using first ps, last ps
* use 2! to set the sym and ex columns as keys

ps1

sym|ex|price
-|-|-
`a`|`x`|	1.1
`b`|	`x`|	2.1
`c`|	`x`|	3.1
`a`|	`y`|	1.2
`b`|	`y`|	2.0
`c`|	`y`|	3.3

ps2

sym|ex|size
-|-|-
`a`|`x`|	200
`b`|	`x`|	100
`c`|	`x`|	300
`a`|	`y`|	200
`b`|	`y`|	50
`c`|	`y`|	200

```q
ps3:ps1 lj ps2
```
* join the ps1 and ps2 tables back together to make table ps3

sym|ex|price|size
-|-|-|-
`a`|`x`|1.1|	200
`b`|	`x`|	2.1|100
`c`|	`x`|	3.1|300
`a`|	`y`|	1.2|200
`b`|	`y`|	2| 50
`c`|	`y`|	3.3| 200

```q
t4: t3 lj ps3
```

* use left join to join ps3 to t3

sym|ex|prirce|size
-|-|-|-
x|	a|	1.1|	200
x|	b|	2.1|	100
x|	c|	3.1|	300
y|	a|	1.2|	200
y|	b|	2.0|	50
y|	c|	3.3|	200


## Part 3: Add 3 new columns: avg_price_by_sym, avg_size_by_ex, wavg_price_by_sym (weighted by size)

Desired Result:

sym|ex|prirce|size| avg_price_by_sym| avg_size_by_ex | wavg_price_by_sym
-|-|-|-|-|-|-
x|	a|	1.1|	200 | 1.15 | 200 | 1.15
x|	b|	2.1|	100|2.05| 200| 2.0667
x|	c|	3.1|	300|3.2| 200| 3.18
y|	a|	1.2|	200|1.15| 150| 1.15
y|	b|	2.0|	50|2.05| 150| 2.06667
y|	c|	3.3|	200|3.2| 150| 3.18

```q
update avg_price_by_sym: avg price by sym from `t4
update avg_price_by_ex: avg size by ex from `t4
update wavg_price_by_sym: size wavg price by sym from `t4
```
sym|ex|prirce|size| avg_price_by_sym| avg_size_by_ex | wavg_price_by_sym
-|-|-|-|-|-|-
a|	x|	1.1|	200|	1.15|	200|	1.15
b|	x|	2.1|	100|	2.05|	200|	2.0667
c|	x|	3.1|	300|	3.2	|200	|3.18
a|	y|	1.2|	200|	1.15|	150|	1.15
b|	y|	2.0|	50	|2.05	|150	|2.0667
c|	y|	3.3|	200|	3.2	|150	|3.18


## 🔵 7. Given the table:

```q
orders: ( [] order:10*1 + til 8; sym:`NYSE`NYSE,6#`NASDAQ; start: 08:00 09:00 09:00 08:00 10:00 12:30 13:30 18:00; end:11:00 13:00 15:30 13:30 11:30 13:30 14:30 19:00)
```

order | sym | start | end
-|-|-|-
10|	NYSE|	08:00|	11:00
20|	NYSE|	09:00|	13:00
30|	NASDAQ|	09:00|	15:30
40|	NASDAQ|	08:00|	13:30
50|	NASDAQ|	10:00|	11:30
60|	NASDAQ|	12:30|	13:30
70|	NASDAQ|	13:30|	14:30
80|	NASDAQ|	18:00|	19:00

<hr>

<a name="random_questions"></a>
## 29. 🔴 Random Questions
[Top](#top)

<hr> 

### What is an Atom vs a List?

```q
An atom - is an irreducible value of a specific data type
A list -  is an ordered sequence of items
```

<hr> 

### What is a dictionary and a table? How are they related?

```q
Dictionaries are a data structure that maps from a domain to a range of values. 
Contains a ! to separate keys and values.

A table is a flipped dictionary. Vectors of data are organized by columns. 
Tables are encased by parathesis ( ) and contain brackets [ ] which assigns the key.
```

<hr> 

### what is the difference between a table and a keyed table?

```q
A table - is a flipped dictionary. Vectors of data are organized by columns.

A keyed table - is a table of keyed records mapped to a table of value records.
```

### What is the difference between a sym and a string?

```q
A sym -  is an atomic entity holding text. Represented with a back tick. 
Smaller in size than a char.

A string - is a list of chars. Represented by " " double parathesis
```

<hr> 

### What is casting? Cast an int to a float

```q
casting converts one datatype to another
```

```q
`int$3.0 / cast float to int
3
```

<hr> 

### What happens when you cast a date to an int?

```q
`int$2000.10.04
3
/ casts as dates from 2000.01.01
```

<hr> 

### Convert syms a b c to a String

```q
string `a`b`c
("a","b","c")
/ simply use the string function
```

### How do you cast a string to a sym?

```q
`$"a","b","c"
"S"$"a","b","c"
`abc
```

### What is a common reason for casting time to seconds or minutes?

A common use of casting is for performing aggregations. We can bucket data stored from milliseconds to seconds to minutes (effectively, rounding up). This allows us to get the average price per minute.

```q
t:([] time:`#asc .z.t + 10?100000; price:asc 100.+til 10)

t
time         price
------------------
11:31:49.745 100
11:31:49.856 101
11:32:05.188 102
11:32:09.395 103
11:32:11.325 104
11:32:24.285 105
11:32:45.249 106
11:32:55.355 107
11:33:18.703 108
11:33:18.855 109
```
```q
select avg price by `minute$time from t
time | price
-----| -----
11:31| 100.5
11:32| 104.5
11:33| 108.5
```

<hr> 

### What is parsing?

Parsing is converting a string to another datatype.

```q
l:("1.00001"; "200"; "3.1417")
"FIF"$l

1.00001 / float
200 / int
3.1417 / float
```

<hr> 

### What are the common operators?

```q
#   / take
_   / drop
?   / find, randomize
@   / apply
!   / dictionary, key, unkey, 
$   / cast, enumerate
,   / join
^   / fill
```
<hr> 


### Show 3 ways to retrieve values from a dictionary

```q
d: `a`b`c!1 2 3

d[`a] = 1
d@`a = 1
d `a = 1
```

<hr> 

### What happens when you try retrieving from a dictionary that has non-unique keys?

```q
d: `a`b`c`a!1 2 3 4
d[`a] = 1 / returns the first entry
```

<hr> 

### Take first 2 items from dict. retrieve value from key 'c

```q
d: `a`b`c!1 2 3
2 # d / returns a dictionary of first 2 rows
(enlist `c) # d / have to use enlist when retrieving single domain
```

<hr> 

### How do you upsert different keys/values from the original dict's datatype?
The upserted keys and values must match in type. <br >
Way around this is to keep dictionary generic using null item

```q
dz: enlist[::]!enlist[::]
dz
dz[`a]:100
dz[100]:`a

key value
a 100
100 a
```

<hr> 

### What are some common table functions?

```q
t:([] company:`ford`bmw; employees:300 100)
t
type t               / what datatypes the table is
count t              / return number of rows
cols t               / retrieve symbol list of column names
meta t               / shows info on type, foreign keys, and attributes
`employees xasc t    / sorts table by employee column
```

<hr> 

### Show examples of union, except, and inter function on tables

```q
t:([] company:`ford`bmw`benz; employees:100 200 300)
u: ([] company:`ford`bmw`ferrari; employees:100 200 400)
```
table t

company | employees
-|-
ford	|100
bmw	|200
benz	|300


table u
company | employees
-|-
ford	|100
bmw	|200
ferrari	|400

```q
t union u / combines every key and value

ford 100
bmw 200
benz 300
ferrari	400
```

```q
t except u / returns item in t NOT in u

benz 300
```

```q
t inter u / returns only common elements in both t and u

ford 100
bmw 200
```

<hr> 

### Show 2 ways to insert data into a table

```q
t:([] company:(); employees:())
insert[`t; (`ferrari;8)]
insert[`t; ([] company:`subaru`hyundai; employees:55 56)]
```
both work; second example specifies column names

<hr> 

### Show how to append using table joins , (comma)

```q
t:([] company:(); employees:())
t:t,([] company:`bmw`skoda; employees:200 300)
```

<hr> 

### what is the difference between equals = and match ~

```q
4 = 4.0
1b / true

4 ~ 4.0
0b / false. match is a lot more strict.
```

<hr> 




[Top](#top)

<a name="bottom"></a>
