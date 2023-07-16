---
creation date: 2023-07-16 18:13
modification date: Sunday 16th July 2023 18:13:15
---

### Script:[](https://tldp.org/LDP/abs/html/testconstructs.html#EX11)

```
#!bin/bash


echo

if test -z "$1"
then
   echo "No command-line arguments"
else
   echo "First command-line arguments"
fi

if /usr/bin/test -z "$1"
then
   echo "No command line arguments"
else
   echo "First command-line argument is $1"
fi

echo

if [ -z "$1" ]
then
   echo "No command-line arguments"
else
   echo "First command-line argument is $1"
fi

echo

if /usr/bin/[ -z "$1" ]
then
   echo "No command-line arguments"
else
   echo "First command-line argument is $1"
fi

echo

exit 0
```

### Output:

![[Pasted image 20230716181942.png]]

### Explanation:



### Things know:
