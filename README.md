# Allen's Notes for KDB+ / Q

Tables example 

### 9. Queries: q-SQL

Append using Assign ,:

```q

t:([] name:`symbol$(); iq:`int$()) / create empty table
```
name | iq
-----|---

```q
t,:`name`iq!(`Beeblebrox; 42)
t,:`name`iq!(`Dent; 98.0)
```
name | iq
-----|---
Beeblebrox | 42
Dent | 98

Assign can also be used with a row of naked values

```q
t,:(`Prefect; 126)
```
name | iq
-----|---
Beeblebrox | 42
Dent | 98
Prefect | 126



