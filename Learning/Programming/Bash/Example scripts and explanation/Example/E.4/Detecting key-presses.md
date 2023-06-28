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
if [ "$key" = $'\x1b\x4f\x46' ];then
   key=$'\x1b\x5b\x34\x7e'
fi

case "$key" in
  $'\x1b\x5b\x32\x7e')
      echo Insert Key
  ;;
  $'\x1b\x5b\x33\x7e')
      echo Delete key
  ;;
  $'\x1b\x5b\x31\x7e')
      echo Home key
  ;;
  $'\x1b\x5b\x34\x7e')
      echo End key
  ;;
  $'\x1b\x5b\x35\x7e')  # Page_Up
   echo Page_Up
  ;;
  $'\x1b\x5b\x36\x7e')  # Page_Down
   echo Page_Down
  ;;
  $'\x1b\x5b\x41')  # Up_arrow
   echo Up arrow
  ;;
  $'\x1b\x5b\x42')  # Down_arrow
   echo Down arrow
  ;;
  $'\x1b\x5b\x43')  # Right_arrow
   echo Right arrow
  ;;
  $'\x1b\x5b\x44')  # Left_arrow
   echo Left arrow
  ;;
  $'\x09')  # Tab
   echo Tab Key
  ;;
  $'\x0a')  # Enter
   echo Enter Key
  ;;
  $'\x1b')  # Escape
   echo Escape Key
  ;;
  $'\x20')  # Space
   echo Space Key
  ;;
  d)
    date
   ;;
  q)
    echo Time to quit
    echo
    exit 0
    ;;
  *)
    echo You Pressed: \'"$key"\'
    ;;
esac

echo
echo "=========="

unset K1 K2 K3
read -s -N1 -p "Press a key: "
K1="$REPLY"
read -s -N2 -t 0.001
K2="$REPLY"
read -s -N1 -t 0.001
K3="$REPLY"
key="$K1$K2$K3"

done
exit $?
```

### Output:

![[Pasted image 20230628175448.png]]

![[Pasted image 20230628175506.png]]

![[Pasted image 20230628175515.png]]


### Explanation:

* Here we are displaying output what key we press in keyboard

### Things know:

* `read -s -N2 -t 0.001`
	* read --> Get input from client
	* `-s`   --> silent, it means while getting input it does not show in kernel
	* `-N2` --> limit of getting input, here limit is 2 so we can get 2character at same time
	* `0.001` --> this time limit between getting next character input
