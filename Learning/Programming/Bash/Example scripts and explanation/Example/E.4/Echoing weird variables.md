---
creation date: 2023-06-28 16:41
modification date: Wednesday 28th June 2023 16:41:30
---

### Script: [](https://tldp.org/LDP/abs/html/quotingvar.html#WEIRDVARS)

```
#!/bin/bash

echo

var="'(]\\{}\$\""
echo $var
echo "$var"

echo

IFS='\'
echo $var
echo "$var"

echo

var2="\\\\\""
echo $var2
echo "$var"

echo

var3='\\\\'
echo "$var3"

```

### Output:

![[Pasted image 20230628164926.png]]

### Explanation:

* In this program helps to know how many ways we have `echo` a variable.

### Things know:

* `IFS` --> Internal field separator
	* It is a special variable that determines how bash splits strings into words or fields when performing word splitting or field splitting.
