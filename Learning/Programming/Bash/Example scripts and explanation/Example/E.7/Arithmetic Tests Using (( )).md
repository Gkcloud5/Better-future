---
creation date: 2023-07-17 17:41
modification date: Monday 17th July 2023 17:41:36
---

### Script:[](https://tldp.org/LDP/abs/html/testconstructs.html#ARITHTESTS)

```
#!/bin/bash

(( 0 ))
echo "Exit status of \"(( 0 ))\" is $?." #1

(( 1 ))
echo "Exit status of \" (( 1 ))\" is $?." #0

(( 5 > 4 ))
echo "Exit status of \"(( 5 > 4 ))\" is #?." #true #0

(( 5 > 9 ))
echo "Exit status of \"(( 5 > 9 ))\" is $?." #false #1

(( 5 == 5 ))
echo "Exit status of \"(( 5 == 5 ))\" is $?." #true #0

var1=5
var2=4

if (( var1 > var2 ))
then
   echo "$var1 is greater than $var2"
fi

exit 0
 ```

### Output:

![[Pasted image 20230717182148.png]]


### Explanation:

* `(( ))` expands and evaluates an arithmetic expression.
	* If the expression evaluates as zero --> It returns an exit status of 1 or false.
	* If  non-zero expression returns an exit status of 0, or true.

 