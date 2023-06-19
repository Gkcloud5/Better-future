---
creation date: 2023-06-19 12:57
modification date: Monday 19th June 2023 12:57:14
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_04.html)

--------------------------------------

#### Explanation about it:

##### Brace expansion:

```
echo sp{el,il,al}l
```

* Brace expansion is a mechanism by which arbitrary string may be generated.


##### Command expansion:

```
$(command) #$date
or
`date`
```


##### Arithmetic expansion:

```
$((EXPRESSION))

$((10+15))


$[EXPRESSION]
$[35+45]
```