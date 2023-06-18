---
creation date: 2023-06-18 17:00
modification date: Sunday 18th June 2023 17:00:59
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_01_03.html)

--------------------------------------

#### Explanation about it:

* When bash program executed, a new process is created because bash makes an exact copy of itself.
	* This child process has the same environment as its parent, only the process ID number is different, this procedure is called `forking`.
* After the forking process, the address space of the child process is overwritten with the new process data. this is done th