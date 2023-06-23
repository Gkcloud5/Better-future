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

space=`df -h | awk '{print $5}' | grep % | grep -v Use | sort -n | tail -1 | cut -d "%" -f1 -`
```

![[Pasted image 20230622204220.png]]


```
#!/bin/bash

space=`df -h | awk '{print $5}' | grep % | grep -v Use | sort -n | tail -1 | cut -d "%" -f1 -`

case $space in
[1-6]*)
    Message="All is quiet."
    ;;
[7-8]*)
    Message="Start thinking about cleaning out some stuff, $space"
    ;;
9[1-8])
    Message="Space going to full, $space"
    ;;
99)
    Message="Emergency, please clean space, $space"
    ;;
esac

echo $Message
```

![[Pasted image 20230622205400.png]]

