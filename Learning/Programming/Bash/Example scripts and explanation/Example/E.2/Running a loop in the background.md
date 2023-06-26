---
creation date: 2023-06-26 18:29
modification date: Monday 26th June 2023 18:29:26
---

### Script:

```
#!/bin/bash
#NAME: Background-loop.sh

for i in 1 2 3 4 5 6 7 8 9 10
do
  echo -n "$i "
done & #Run this loop in background
       # Will sometimes execute after second loop

echo 

for i in 11 12 13 14 15 16 17 18 19 20
do
  echo -n "$i "
done

echo

exit 0
```

### Output:

![[Pasted image 20230626183547.png]]


### Explanation:

* To solve this non sorted value we can use `&&`

![[Pasted image 20230626184146.png]]


### Things know:
