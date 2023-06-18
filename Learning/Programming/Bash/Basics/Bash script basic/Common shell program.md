---
creation date: 2023-06-18 15:30
modification date: Sunday 18th June 2023 15:30:29
---

**Tags:** #linux #bash 

#### Source:
[tldp](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_01_01.html)

--------------------------------------

#### Explanation about it:

##### 1. General shell functions:

* Shell program interprets user commands
	* Directly entered by the user
	* Can be read from a file called shell script.
* Shell scripts are interpreted not compiled.
* Shell reads commands from the script line by line.

##### 2. Shell types:

* Linux have variety of shell types
	* `sh or Bourne shell:` This is basic shell, a small program with few feature.
	* `bash or Bourne shell again:` It's standard GNU shell. it's for beginning user as well powerful tool also.
	* `csh or C shell:` syntax of this shell resembles that C programming language
	* `ksh or korn shell:` it's superset of the Bourne shell, it's little complicated for use.

```
root@root:~# cat /etc/shells
# /etc/shells: valid login shells
/bin/sh
/bin/bash
/usr/bin/bash
/bin/rbash
/usr/bin/rbash
/usr/bin/sh
/bin/dash
/usr/bin/dash
/usr/bin/tmux
/usr/bin/screen

```
