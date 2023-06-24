---
creation date: 2023-06-24 17:41
modification date: Saturday 24th June 2023 17:41:35
---

**Tags:** #linux #bash

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_10_02.html)

--------------------------------------

#### Explanation about it:

* An array is a variable containing multiple values.

##### Creating Arrays:

```
ARRAY[INDEXNR]=value

declare -a ARRAYNAME

ARRAY=(value1 value2 .... valueN)

```


```
ARRAY=(one two three)
echo ${ARRAY[*]}
one two three

echo $ARRAY[*]
one[*]

echo ${ARRAY[2]}
three

ARRAY[3]=four
one two three four
```

