---
creation date: 2023-06-19 09:47
modification date: Monday 19th June 2023 09:47:34
---

**Tags:** #linux #bash 

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_02_03.html)

--------------------------------------

#### Explanation about it:

* Bash provides extensive debugging features.
	* -x option,  which will run the entire script in debug mode.
```
bash -x scriptname

+ echo 'script start now'
script start now
+ echo 'Hi, root'
Hi, root
+ Color=Blue
+ Value=5
+ echo 'Color is Blue and value is 5'
Color is Blue and value is 5
root@root:~/bash_script#

```

* Debug a specific part

```
echo "script start here"

set -x
w
set +x

#Output
script start here
+ w
USER TTY .....
+ set +x
--
```