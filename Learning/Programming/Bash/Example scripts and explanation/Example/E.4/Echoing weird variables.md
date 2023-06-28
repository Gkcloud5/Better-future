---
creation date: 2023-06-28 16:41
modification date: Wednesday 28th June 2023 16:41:30
---

### Script:

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



### Explanation:



### Things know:

* `IFS` --> Internal field separator
	* 