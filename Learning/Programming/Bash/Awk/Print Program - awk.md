---
creation date: 2023-06-21 16:49
modification date: Wednesday 21st June 2023 16:49:55
---

**Tags:** #linux #bash #awk 

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_06_02.html)

--------------------------------------

#### Explanation about it:

* print command in awk outputs selected data from the input file

```
ls -l | awk '{print $5}'
```

##### Formatting fields:

```
ls -la | awk '{print "size is  " $5 " file name is " $9 }'
```

![[Pasted image 20230621170120.png]]

##### Print command and regular expressions:

```
df -h | awk '/dev\/xv/ { print $6 "\t: " $5 }'
```

![[Pasted image 20230621171330.png]]

