---
creation date: 2023-06-27 13:09
modification date: Tuesday 27th June 2023 13:09:09
---

### Script:

```
#!/bin/bash

a=23
echo $a

b=$a
echo $b

a=`echo Hello`
echo $a

a=`ls -l`
echo $a

echo

echo "$a"

exit 0
```

### Output:

![[Pasted image 20230627131300.png]]

### Explanation:

* Here we are assigned some simple variables

### Things know:

* `ls -l` we can assign command output to one variable
* if we use `"$a"`  double quotes then output will be print in new line.