---
creation date: 2023-07-31 14:31
modification date: Monday 31st July 2023 14:31:07
---

### Script:[](https://tldp.org/LDP/abs/html/ops.html#ANDOR)

```
#!/bin/bash

a=24
b=47

if [ "$a" -eq 24 ] && [ "$b" -eq 47 ]
then
	echo "Test #1 Succeeds"
else
	echo "Test #1 Fails"
fi

if [ "$a" -eq 98 ] || [ "$b" -eq 47 ]
then
    echo "Test #2 success"
else
	echo "Test #2 fails"
fi

```

### Output:

![[Pasted image 20230731143726.png]]
### Explanation:

* && and || are logical operators
	* return only true or false
* && --> only true all condition is true
* || --> it true any one of the condition is true


