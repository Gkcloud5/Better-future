---
creation date: 2023-06-26 01:04
modification date: Monday 26th June 2023 01:04:18
---

### Script:

```
#!/bin/bash

File=/etc/fstab-bkp

{
read line1
read line2
} < $File

echo "First line in $File"
echo "$line1"
echo

echo "Second line in $File"
echo "$line2"
exit 0
```

### Output:

![[Pasted image 20230626010825.png]]

![[Pasted image 20230626012457.png]]

### Explanation:

* In above example we are reading a file by using `<`
	* It redirect file to variable

### Things know:

* We can use `<` to redirect and read file line by line
* If we want to take specific line then we need to use cat + tail.