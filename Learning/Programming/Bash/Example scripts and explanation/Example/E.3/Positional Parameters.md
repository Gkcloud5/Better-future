---
creation date: 2023-06-27 15:11
modification date: Tuesday 27th June 2023 15:11:24
---

### Script:

```
#!/bin/bash

MINPARAMS=10

echo

echo "The name of the sctipt is \"$0\"."
echo

if [ $# -lt "$MINPARAMS"]
then
   echo "This script needs at least $MINPARAMS command line arguments"
   exit 1
fi

if [-n "$1"]
then
   echo "Parameter #1 is $1"
fi

if [ -n "${9}" ]
then
   echo "Parameter #10 is ${10}"
fi

echo

exit 0
```

### Output:

![[Pasted image 20230627152152.png]]

### Explanation:

* Here we declare variable with argument that passed with script 

### Things know:

* We can get arguments by using `$position number` inside program.