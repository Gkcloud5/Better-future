---
creation date: 2023-06-21 17:33
modification date: Wednesday 21st June 2023 17:33:15
---

**Tags:** #linux #bash #awk 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_06_03.html)

--------------------------------------

#### Explanation about it:

##### Field separator:

* It is either a single character or a regular expression.
* Field separator is represented by the built-in variable `FS`.

```
awk 'BEGIN {FS=":" } { print $1 "\t" $5}' /etc/passwd
```

![[Pasted image 20230621181229.png]]


##### Create awk script:

```
vi printnames.awk

BEGIN { FS=":"}
{ print $1 "\t" $5}

```

![[Pasted image 20230621181603.png]]

##### Output filed separators:

```
awk '{ print $1 $2}' test

awk '{ print $1,$2}' test
```

![[Pasted image 20230621181846.png]]


