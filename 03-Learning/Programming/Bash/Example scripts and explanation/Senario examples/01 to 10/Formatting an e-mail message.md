---
creation date: 2023-08-02 11:34
modification date: Wednesday 2nd August 2023 11:34:51
---

### Script:[](https://tldp.org/LDP/abs/html/contributed-scripts.html#MAILFORMAT)

```
#!/bin/bash
ARGS=1
E_BADARGS=85
E_NOFILE=86

if [ $# -ne $ARGS ]
then
   echo "Usage: `basename $0` filename"
   exit $E_BADARGS
fi

if [ -f "$1" ]
then
   file_name=$1
else
   echo "File \"$1\" does not exist"
   exit $E_NOFILE
fi

MAXWIDTH=70

sedscript='s/^>//
s/^ *>//
s/^ *//
s/        *//'

sed "$sedscript" $1 | fold -s --width=$MAXWIDTH

exit $?
```

### Output:

![[Pasted image 20230802114808.png]]


### Explanation:

* `-f` used to check it's file or not

