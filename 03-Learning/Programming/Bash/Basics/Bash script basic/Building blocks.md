---
creation date: 2023-06-18 17:22
modification date: Sunday 18th June 2023 17:22:51
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_01_04.html)

--------------------------------------

#### Explanation about it:

##### Shell Building blocks:

* Shell reads its input from a file, from a string or from the user's terminal.
* Input is broken up into words and operators, obeying in the quoting rules.
* shell parses the tokens into simple and compound commands.
* Bash performs various shell expansions, breaking the expanded token into lists of filenames and commands and arguments.
* redirection is performed if necessary.
* commands are executed.
* Optically the shell waits for the command to complete and collects its exit status.

* **Shell commands:** 
	* touch filename
	* ls | more
	* ....
* **Shell functions:** 
	* Shell functions are a way to group commands for later execution using single name for the group.
* **Shell Parameters:** 
	* Parameter is an entity that stores a values,
		* It can be name, a number or a special value.
	* For shell's purpose, a variable is a parameter that stores a name. 
