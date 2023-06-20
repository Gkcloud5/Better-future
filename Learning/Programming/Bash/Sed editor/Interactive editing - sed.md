---
creation date: 2023-06-19 15:39
modification date: Monday 19th June 2023 15:39:21
---

**Tags:** #linux #bash #sed

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_05_02.html)

--------------------------------------

#### Explanation about it:

```
sed '/errors/p' example.txt
```

![[Pasted image 20230619154455.png]]

```
sed -n '/error/p' example.txt
```

![[Pasted image 20230619154606.png]]

##### Delete a line:

```
sed '/errors/d' example.txt
```

![[Pasted image 20230619154723.png]]


##### Range of lines:

* remove specific range from file

```
sed '2,4d' filename

#it remove a line from 2 to 4 in file
```

![[Pasted image 20230620165736.png]]

```
sed -n '/It was/,/and I/p' example
```

![[Pasted image 20230620173640.png]]


#### Find and replace with sed:

```
sed 's/apologize/sorry/' example
```

