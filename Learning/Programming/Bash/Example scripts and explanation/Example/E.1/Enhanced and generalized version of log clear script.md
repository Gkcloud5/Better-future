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
   echo "lines, $1"
else
   lines=$LINES #default, if not specified on command-line
fi

cd $LOG_DIR

if [ `pwd` != "$LOG_DIR" ]
then
   echo "Can't change to $LOG_DIR"
   exit $E_XCD
fi

#tail -n $lines messages > mesg.temp
#mv mesg.temp messages

cat /dev/null >  messages

cat /dev/null >  wtmp
echo "Log files cleaned up"

exit 0

```

### Output:

![[Pasted image 20230626005006.png]]

### Explanation:

* In above script we gave special error code
	* This will help us to know where we get error
		* we can get error code --> $?
* Here we specially check root user is accessing script 
* Here we specially double confirm the directory


### Things know:

* `[ -n "$1"]` --> This is true when $1 is empty does not contain any value
* `$UID` --> Linux built-in user id checking command