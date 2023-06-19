---
creation date: 2023-06-19 11:44
modification date: Monday 19th June 2023 11:44:28
---

**Tags:** #linux #bash

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_03.html)

--------------------------------------

#### Explanation about it:

* Quoting is used to remove the special meaning of characters or words.

###### Escape characters:

* Escape character are used to remove the special meaning from a single character.
* `\` is used as an escape character

```
date=10121988
echo $date
echo \$date
```

![[Pasted image 20230619125136.png]]

###### Single quotes:

```
echo '$date'

#output
$date
```

###### Double quote:

* Dollar sign and the backticks retain their special meaning within the double quotes

```
echo "$date"

echo "`date`"
```

![[Pasted image 20230619125535.png]]

