---
creation date: 2023-06-25 17:09
modification date: Sunday 25th June 2023 17:09:58
---

### Script:

```
#!/bin/bash

LOG_DIR=/var/log
cd $LOG_DIR
echo $LOG_DIR
pwd
cat /dev/null > messages
cat /dev/null > wtmp

echo "Logs cleaned up"
exit
```

### Output:

![[Pasted image 20230625171725.png]]


### Explanation:

* Created a special variable for 

### Things know:
