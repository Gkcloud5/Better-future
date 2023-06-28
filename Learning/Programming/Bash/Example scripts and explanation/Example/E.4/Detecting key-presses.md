---
creation date: 2023-06-28 17:05
modification date: Wednesday 28th June 2023 17:05:02
---

### Script: [](https://tldp.org/LDP/abs/html/escapingsection.html#BASHEK)

```
#!/bin/bash
key="no value yet"
while true; do
    clear
    echo "Bash extra keys demo. keys to try:"
    echo
    echo "* Insert, Delete, Home, End, Page_up and page_down"
    echo "* The four arrow keys"
    echo "* Tab. enter, escape, and space key"
    echo "* The letter and number keys, etc"
    echo 
    echo "    d =  show date/time"
    echo "    q = quit"
    echo "================"
    echo

#Convert separate home-key to home-key_num_7
if [ "$key" = $'\x1b\x4f\x48' ];then
   key=$'\x1b\x5b\x31\x7e'
fi

#Convert the separate end-key to end-key_num_1.
if [ "$key" = $'\x1b\x4f\x46']

```

### Output:



### Explanation:



### Things know:
