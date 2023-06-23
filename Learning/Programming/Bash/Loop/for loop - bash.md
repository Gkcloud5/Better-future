---
creation date: 2023-06-23 16:17
modification date: Friday 23rd June 2023 16:17:01
---

**Tags:** #linux #bash #for-loop

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_01.html)

--------------------------------------

#### Explanation about it:

* A list of commands is executed for each value in the list

```
for NAME [in LIST]; do COMMANDS; done
```

```
#!/bin/bas

for i in `cat example`
do
   touch "$i".for
done
```

![[Pasted image 20230623162300.png]]