---
creation date: 2023-08-02 11:34
modification date: Wednesday 2nd August 2023 11:34:51
---

### Script:[](https://tldp.org/LDP/abs/html/contributed-scripts.html#MAILFORMAT)

```
#!/bin/bash
ARGS=1
E_BADARGS=85
E_NOFILE=86

if [ $# -ne $ARGS ]
then
   echo "Usage: `basename $0` filename"
   exhit $E_BADARGS
```

### Output:



### Explanation:



### Things know:
