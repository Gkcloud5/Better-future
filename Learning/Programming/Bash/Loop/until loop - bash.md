---
creation date: 2023-06-23 16:55
modification date: Friday 23rd June 2023 16:55:39
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_03.html)

--------------------------------------

#### Explanation about it:

* It is same as while loop but here loop stop only when condition is true

```
until TEST-COMMAND;
do
  Consequent-Commands;
done
```

```bash
#!/bin/bash

i="0"
until [ $i == 4 ]
do
  echo "$i"
  i=$[$i+1]
done
echo "outisde, $i"
```


![[Pasted image 20230623170352.png]]