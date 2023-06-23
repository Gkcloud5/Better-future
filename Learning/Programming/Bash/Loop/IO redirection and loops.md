---
creation date: 2023-06-23 17:05
modification date: Friday 23rd June 2023 17:05:34
---

**Tags:** #linux #bash 

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_04.html)

--------------------------------------

#### Explanation about it:

```
#!/bin/bash

# This script creates a subdirectory in the current directory, to which old
# files are moved.
# Might be something for cron (if slightly adapted) to execute weekly or 
# monthly.

ARCHIVENR=`date +%Y%m%d`
DESTDIR="$PWD/archive-$ARCHIVENR"

mkdir "$DESTDIR"

# using quotes to catch file names containing spaces, using read -d for more 
# fool-proof usage:
find "$PWD" -type f -a -mtime +5 | while read -d $'\000' file

do
gzip "$file"; mv "$file".gz "$DESTDIR"
echo "$file archived"
done
```

