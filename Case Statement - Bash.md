---
creation date: 2023-06-22 20:34
modification date: Thursday 22nd June 2023 20:34:56
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_07_03.html)

--------------------------------------

#### Explanation about it:

```
case EXPRESSION in case1) COMMAND-LIST;; case2) COMMAND-LIST;; ...CASEN)
COMMAND-LIST;;esac
```

```
#!/bin/bash

space=`df -h | awk '{print $5} | grep % | grep -v use'`
```