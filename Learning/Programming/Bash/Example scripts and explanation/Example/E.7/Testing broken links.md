---
creation date: 2023-07-18 16:12
modification date: Tuesday 18th July 2023 16:12:30
---

### Script:[](https://tldp.org/LDP/abs/html/fto.html#BROKENLINK)

```
#!/bin/bash

[ $# -eq 0 ] && directorys=`pwd` || directorys=$@


linkchk () {
   for element in $1/*; do
   [ -h "$element" -a ! -e "$element" ] && echo \ "$element\"
   [ -d "$element" ] && linkchk $element
   done
}

for directory in $directorys; do
    if [ -d $directory ]
       then linkchk $directory
       else
	       echo "$directory is not a directory"
	       echo "usage: $0 dir1 dir2 ..."
	fi
done

exit $?
```

### Output:

![[Pasted image 20230718163242.png]]

### Explanation:

* Here we used test expression and perform some condition

### Things know:

* https://tldp.org/LDP/abs/html/fto.html#BROKENLINK
