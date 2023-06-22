---
creation date: 2023-06-22 17:36
modification date: Thursday 22nd June 2023 17:36:33
---

**Tags:** #linux #bash

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_07_01.html)

--------------------------------------

#### Explanation about it:

```
if TEST-COMMANDS; then CONSEQUENT-COMMANDS;fi
```

* TEST-COMMAND list is executed and if its return status is zero
	* Then the CONSEQUENT-COMMANDS list is executed.

##### Some primary expression:

```
[ -a FILE] --> TRUE if FILE exists
[ -b FILE] --> TRUE if FILE exists and is a block-special file
[ -c FILE] --> TRUE if FILE exists and is a character special file
[ -e FILE] --> TRUE if FILE exists
[ -f FILE] --> TRUE if FILE exists and is a regular file
.... please check website
```

##### Checking files:

```
cat filecheck.sh

#!/bin/bash

echo "This scripts check file"
echo "Checking"

if [ -f /var/log/messages ]
    then
        echo "file exists"
fi
echo
echo "..done"
```

##### Testing exist status:

* ? --> it holds the exit status of the previously executed command

![[Pasted image 20230622180126.png]]


##### String Comparison:

```
if [ "$(whoami)" != 'root' ];then
    echo "this is not root user"
    exit 1;
else
   echo "this is root user"
   exit 1;
fi
```

![[Pasted image 20230622181316.png]]

```
gender="female"

if [[ "$gender" == f* ]]
then
    echo "Nice to meet you madam"
fi
```