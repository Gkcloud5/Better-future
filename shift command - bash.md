---
creation date: 2023-06-24 17:12
modification date: Saturday 24th June 2023 17:12:23
---

**Tags:** #linux #bash #shift

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_09_07.html)

--------------------------------------

#### Explanation about it:

* `shift` command is one of the bash built-in that comes with bash.
* It is used to shift the positional parameters in a script or a function.

```
#!/bin/bash

function print_arguments() {
    echo "Arguments"
    echo "........."
    while [ $# -gt 0];do
        echo "$1"
        shift
    done
}

print_arguments "apple" "banana" "cherry" "date"
```