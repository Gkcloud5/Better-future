---
creation date: 2023-06-26 01:34
modification date: Monday 26th June 2023 01:34:54
---

### Script:

```
#!/bin/bash
#rpm-check.sh

SUCCESS=0
E_NOARGS=65

if [ -z "$1" ]
then
   echo "Usage: `basename $0` rpm-file"
   exit $E_NOARGS
fi

{
#Begin code block
echo
echo "Archieve description:"
rpm1=`rpm -qpi $1` #query description

echo "$rpm1"

echo "Archieve listing:"
rpm -i --test $1  #query whether rpm file can be installed.

if [ "$?" -eq $SUCCESS ]
then
   echo "$1 can be installed."
else
   echo "$1 cannot be installed."
fi
echo

}  > "$1.test" #redirect output of everything in block to file

echo "Results of rpm test in file $1.test"

exit 0
```

### Output:



### Explanation:



### Things know:
