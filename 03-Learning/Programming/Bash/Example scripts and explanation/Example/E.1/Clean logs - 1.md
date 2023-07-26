---
creation date: 2023-06-25 16:53
modification date: Sunday 25th June 2023 16:53:54
---

### Script:

```
#!/bin/bash

cd /var/log
cat /dev/null > messages
cat /dev/null > wtmp
echo "log files cleaned up"
```

### Output:

![[Pasted image 20230625170359.png]]

### Explanation:

* It went to folder and clear logs

### Things know:

* /dev/null --> It is linux null device file. this will discard anything written to it
	* [dev/null](https://www.digitalocean.com/community/tutorials/dev-null-in-linux)
