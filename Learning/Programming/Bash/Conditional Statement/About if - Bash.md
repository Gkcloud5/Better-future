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
[ -b ]
```