---
creation date: 2023-06-27 16:10
modification date: Tuesday 27th June 2023 16:10:45
---

### Script:

```
#!/bin/bash

until [ -z "$1" ]
do
  echo -n "$1 "
  shift
done

echo

echo $2

exit
```

### Output:

![[Pasted image 20230627162111.png]]

### Explanation:

* In this example we are used `shift` command to move arguments.
	* By doing this it change position of parameters

### Things know:

* `shift` will used to change position of arguments.
* `-z` it's true when there is empty.