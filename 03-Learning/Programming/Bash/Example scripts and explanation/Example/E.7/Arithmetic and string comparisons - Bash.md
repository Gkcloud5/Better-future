---
creation date: 2023-07-22 14:13
modification date: Saturday 22nd July 2023 14:13:45
---

### Script:[](https://tldp.org/LDP/abs/html/comparison-ops.html#EX13)

```bash
#!/bin/bash

a=4
b=5

echo

if [ "$a" -ne "$b" ]
then
   echo "$a is not equal to $b"
   echo 
fi


```

### Output:

![[Pasted image 20230722142343.png]]

### Explanation:

##### Integer comparison:

* `-eq` --> is qual to 
	* if [  "$a" -eq "$b" ]
* `-ne` --> is not equal to
* `-gt` --> is greater than
* `-ge` --> is greater than or equal to
* `-lt` --> is less than
* `-le` --> is less than or equal to
* `<` --> is less than
* `<=` --> is less than or equal to
* `>` --> is greater than
* `>=` --> is greater than or equal to

##### String comparison:

* `=` --> is equal to
* `===` --> is qual to
* `!=` --> is not equal to
* `<` --> is less than 
	* ASCII alpha order
* `-z` --> true if string is null, it has zero length
* `-n` --> true if string is not null


