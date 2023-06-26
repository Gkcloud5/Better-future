---
creation date: 2023-06-26 18:57
modification date: Monday 26th June 2023 18:57:30
---

### Script:

```
#!/bin/bash

BACKUPFILE=backup-$(date +%m-%d-%Y)

archive=${1:-$BACKUPFILE}

tar cvf - `find . -mtime -1 -type f -print` > $archive.tar
gzip $archive.tar
echo "Directory $PWD backed up in archive file \"$archive.tar.gz\"."

exit 0
```

### Output:

![[Pasted image 20230627002807.png]]

### Explanation:



### Things know:
