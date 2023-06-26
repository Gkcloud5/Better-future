---
creation date: 2023-06-27 01:40
modification date: Tuesday 27th June 2023 01:40:45
---

### Script:

```
#!/bin/bash

a=375
hello=$a

#No space between `=`

echo hello

echo $hello   #assign_var1

echo ${hello} #assign_var2

echo

hello="A B  C   D"
echo $hello
echo "$hello"

echo

mixed_bag=2\ ---\ Whatever

echo "$mixed_bag"

echo; echo

unlitialized_variable=23
echo "uninitialized_variable = $unlitialized_variable"
unset unlitialized_variable
echo "uninitialized_variable = $unlitialized_variable"

echo

exit 0
```

### Output:

![[Pasted image 20230627015516.png]]

### Explanation:

* Above program

### Things know:
