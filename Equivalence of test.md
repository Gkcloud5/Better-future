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
   echo "First"
```

### Output:



### Explanation:



### Things know:
