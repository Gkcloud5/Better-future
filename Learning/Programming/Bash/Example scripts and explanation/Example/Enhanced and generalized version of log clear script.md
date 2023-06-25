---
creation date: 2023-06-25 17:25
modification date: Sunday 25th June 2023 17:25:14
---

### Script:

```
#!/bin/bash

LOG_DIR=/var/log
ROOT_UID=0 #only users with $UID 0 have root privileges
LINES=50 #Default number of lines saved
E_XCD=86 #Can't change directory?
E_NOTROOT=87 #non-root exit error

#Run as root
if [ "$UID" -ne "$ROOT_UID" ]
then
   echo "Must be root to run this script"
   exit $E_NOTROOT
fi

if [ -n "$1"]
then
   lines=$1
   echo "lines,"
else
   lines=$LINES #default, if not specified on command-line
fi

cd $LOG_DIR

if [ `pwd` != "$LOG_DIR" ]
then
   echo "Can't change to $LOG_DIR"
   exit $E_XCD
fi

tail -n $lines messages > mesg.temp
mv mesg.temp messages
```

### Output:



### Explanation:



### Things know:
