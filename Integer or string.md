---
creation date: 2023-06-27 13:15
modification date: Tuesday 27th June 2023 13:15:56
---

### Script:

```
#!/bin/bash
#NAME:int-or-string.sh

a=2334
let "a += 1"
echo "a = $a"
echo

b=${a/23/BB}
echo "b = $b"
declare -i b
echo "b = $b"
echo

c=BB34
echo "c = $c"
d=${c/BB/23}

echo "d = $d"
let "d += 1"
echo "d = $d"
echo

e=''
echo "e = $e"
let "e += 1"
echo "e = $e"
echo

exit $?
```

### Output:

![[Pasted image 20230627150431.png]]

### Explanation:

* Here we simply assigned value and replace with another value and added it

### Things know:

