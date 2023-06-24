---
creation date: 2023-06-24 17:55
modification date: Saturday 24th June 2023 17:55:30
---

**Tags:** #linux #bash

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_11_01.html)

--------------------------------------

#### Explanation about it:

##### What are functions:

* Functions are group of commands for later execution, using single name for this group or routine.
* When calling on a function as a simple command name, the list of commands associated with that function name is executed.

```
function FUNCTION{
COMMANDS
}

FUNCTION(){
COMMANDS
}
```


```bash
#!/bin/bash

echo "Function example"

test(){
echo "Postitional parameter 1 in the function is $1"
}
```