---
creation date: 2023-06-23 16:24
modification date: Friday 23rd June 2023 16:24:39
---

**Tags:** #linux #bash #while

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_02.html)

--------------------------------------

#### Explanation about it:

* While construct allows for repetitive execution of a list of commands

```
while CONTROL-COMMAND;
do
  CONSEQUENT-COMMANDS;
done
```

```
#!/bin/bash

i="0"

while [ $i -lt 4 ]
do
xterm &
i=$[$i+1]
echo $i
done
```

![[Pasted image 20230623165329.png]]


