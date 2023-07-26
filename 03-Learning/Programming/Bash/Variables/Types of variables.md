---
creation date: 2023-06-24 17:29
modification date: Saturday 24th June 2023 17:29:15
---

**Tags:** #linux #bash

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/chap_10.html)

--------------------------------------

#### Explanation about it:

##### Assignment of values:

```
VARIABLE=12
echo $VARIABLE
```

##### Using the declare built-in:

```
declare OPTIONS VARIABLE=value
```

![[Pasted image 20230624173809.png]]

```
declare -i var=12
var=string
echo $var
0
```


##### Constants:

```
readonly OPTION VARIABLE(s)
```

```
readonly var=12
var=15
bash: var: readonly variable
```

