---
creation date: 2023-06-23 17:14
modification date: Friday 23rd June 2023 17:14:17
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_05.html)

--------------------------------------

#### Explanation about it:

* `break` statement is used to exit the current loop it's normal ending.

```
#!/bin/bash

# This script converts all file names containing upper case characters into file# names containing only lower cases.

LIST="$(ls)"

for name in "$LIST"; do

if [[ "$name" != *[[:upper:]]* ]]; then
continue
fi

ORIG="$name"
NEW=`echo $name | tr 'A-Z' 'a-z'`

mv "$ORIG" "$NEW"
echo "new name for $ORIG is $NEW"
done
```
