---
creation date: 2023-06-19 09:07
modification date: Monday 19th June 2023 09:07:42
---

**Tags:** #linux #bash 

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_02_01.html)

--------------------------------------

#### Explanation about it:

##### 1. Writing and naming:

* Shell script is a sequence of commands for which you have repeated use
	* This sequence is typically executed by entering the name of the script on the command line.
	* You can use scripts to automate tasks using the cron facility.

```
locate scriptname
```

```
#script content
#!/bin/bash
clear

echo "script start now"

echo "Hi, $USER"

Color="Blue"
Value="5"

echo "Color is $Color and value is $Value"


#Permission
chmod +x *scriptname*

#Execution
bash *scriptname* 
or
source *scriptname* --> it does not need execute permission


```