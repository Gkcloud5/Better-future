---
creation date: 2023-07-03 20:36
modification date: Monday 3rd July 2023 20:36:35
---

### Script:

```
#!/bin/bash
# If we are unsure how a certain condition might evaluate, 
# test it in an if-test

echo
echo "Testing \"0\""
if [ 0 ]
then
   echo "0 is true"
else
   echo "0 is false"
fi

echo

echo "Testing \"1\""
if [ 1 ]
then
   echo "1 is true."
else
   echo "1 is false"
fi

echo 

echo "Testing \"-1\""
if [ -1 ]
then
   echo "-1 is true"
else
   echo "-1 is false"
fi
echo

xyz=
echo "Testing \"-n \$xyz\""
if [ -n "$xyz" ]
then
   echo "Null variable is true"
else
   echo "Null variable is false"
fi

echo

exit 0
```

### Output:

![[Pasted image 20230703205043.png]]

### Explanation:

* Here we just checked some if condition 
	* How it works with different conditions.

### Things know:

* `-n` --> 