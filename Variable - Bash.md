---
creation date: 2023-06-19 10:27
modification date: Monday 19th June 2023 10:27:03
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_02.html)

--------------------------------------

#### Explanation about it:

* Two type of variable
	* Global variable
	* Local Variable

##### Global variable:

* It is environment variable.

```
#to see global variable
env or printenv
```

```
root@root:~# printenv
SHELL=/bin/bash
PWD=/root
LOGNAME=root
XDG_SESSION_TYPE=tty
MOTD_SHOWN=pam
HOME=/root
```


##### Local Variable:

* Local variable are variable that are limited in scope to a particular block of code or function.


##### Variable by content:

* 4 Types
	* String Variables
	* Integer Variables
	* Constant Variables
	* Array Variables


#### Creating Variables:

* Variables are case sensitive by default.

```
#Example of variable creation
MYVAR="2"
first_name="GK"

```

#### Exporting variables

```
export varname="value"
```