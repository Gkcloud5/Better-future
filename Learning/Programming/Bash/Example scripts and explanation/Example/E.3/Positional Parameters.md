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
```

### Output:



### Explanation:



### Things know:
