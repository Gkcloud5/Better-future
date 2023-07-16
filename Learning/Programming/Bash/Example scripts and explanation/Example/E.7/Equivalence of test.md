---
creation date: 2023-07-16 18:13
modification date: Sunday 16th July 2023 18:13:15
---

### Script 1:[](https://tldp.org/LDP/abs/html/testconstructs.html#EX11)

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


### Script 2:

```
#!/bin/bash
file=/etc/passwd

if [[ -e $file ]]
then
   echo "File exists"
fi

```

### Output2:

![[Pasted image 20230716182253.png]]

### Explanation:

* `-e` used to check file is exist or not
* `-z` command used to check string is empty or not

### Things know:

* Use case of `-e and -z`
