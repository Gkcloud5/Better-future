---
creation date: 2023-06-23 15:13
modification date: Friday 23rd June 2023 15:13:48
---

**Tags:** #linux #bash

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_08_02.html)

--------------------------------------

#### Explanation about it:

* `read` built-in command is used to get input from 

```
read [options] NAME1 NAME2 ... NAMEN
```

```
#!/bin/bash

echo "Provide your birth year"

read year

echo "This is your birth year $year"
```

![[Pasted image 20230623152104.png]]


##### Redirection and file descriptors:

* Best file descriptors
	* stdin   --> 0
	* stdout --> 1
	* stderr  --> 2

```
ls -l * 2 > /var/tmp/redirect.txt
```