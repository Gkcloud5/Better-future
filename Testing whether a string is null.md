---
creation date: 2023-07-26 19:11
modification date: Wednesday 26th July 2023 19:11:40
---

### Script:[](https://tldp.org/LDP/abs/html/comparison-ops.html#STRTEST)

```
#!/bin/bash

string1 =  $1
echo "parameter $1"

if [ -n $string1] //not quoted so it's declared
then
	echo "string is not null, $string1"
else
	echo "String is null"
fi

echo 

if [ -n "$string1"] //double quoted, it seems it's tring
then
	echo "Double quoted character"
else
	echo "double quote act is variable not a string"
fi
echo


```

### Output:



### Explanation:

* = `if [ "$a" = "$b" ]` --> is not equal to
* == `if [ "$a" == "$b" ]` --> check both are equal or not
* !=
* <, > --> result based on ASCII character
* `-z` it's true when string is null
* `-n` it's true when string is not null


