---
creation date: 2023-06-23 17:23
modification date: Friday 23rd June 2023 17:23:44
---

**Tags:** 

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_06.html)

--------------------------------------

#### Explanation about it:

```
select WORD [in LIST]; do RESPECTIVE-COMMANDS; done
```

```
#!/bin/bash

echo "This script can make any of the files in this directory"
echo "Enter the number of the file you want to protect:"

select FILENAME in *;
do
   echo "You picked $FILENAME ($REPLY), it is now only accessible to you."
   chmod go-rwx "$FILENAME"
done
```

![[Pasted image 20230624165848.png]]

```
#!/bin/bash

PS3="Your Choice:"
QUIT="Quit this program - I feel safe now"
touch "$"
```