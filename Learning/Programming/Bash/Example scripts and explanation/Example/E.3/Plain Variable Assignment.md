---
creation date: 2023-06-27 02:16
modification date: Tuesday 27th June 2023 02:16:24
---

### Script:

```
#!/bin/bash

echo

a=879
echo "The value of \"a\" is $a."

let a=16+5
echo "The value of \"a\" is now $a."
echo

echo -n "Values of \"a\" in the loop are:"
for a in 7 8 9 11
do
  echo -n "$a "
done

echo
echo

echo -n "Enter \"a\""
read a
echo "value is $a"

echo

exit 0
```

### Output:

![[Pasted image 20230627023913.png]]


### Explanation:

* This is simple explanation for assigning variable

### Things know:

* 