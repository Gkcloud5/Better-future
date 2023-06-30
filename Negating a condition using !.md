---
creation date: 2023-06-30 18:24
modification date: Friday 30th June 2023 18:24:50
---

### Script: [](https://tldp.org/LDP/abs/html/exit-status.html#NEGCOND)

```
#!/bin/bash
true
echo "exit status of \"true\" = $?"

! true
echo "exit status of \"! true\" =$?"

true
!true

ls | bogus_command
echo $?

! ls | bougus_command
echo $?
```

### Output:

![[Pasted image 20230630220105.png]]

### Explanation:

* Here we know how error code

### Things know:

* 