---
creation date: 2023-07-28 13:03
modification date: Friday 28th July 2023 13:03:47
---

### Script:[](https://tldp.org/LDP/abs/html/ops.html#ARITHOPS)

```
#!/bin/bash

n=1; echo -n "$n "

let "n =$n + 1"
echo -n "$n "

: $(( n = $n + 1))
echo -n "$n "

n=$(($n+1))
echo -n "$n "

n=$[ $n + 1 ]
echo -n "$n "
```

### Output:



### Explanation:

* `+=` Increment variable by a constant
	* let var += 5 
* `*=`
* /=
* %=

### Things know:
