---
creation date: 2023-06-28 16:52
modification date: Wednesday 28th June 2023 16:52:03
---

### Script:[](https://tldp.org/LDP/abs/html/escapingsection.html#ESCAPED)

```
#!/bin/bash

echo ""
echo "This will print
as two lines"
echo
echo "This will print \
as one line."
echo;echo
echo "============="
echo "\v\v\v\v"
echo "============="
echo "Vertical tabs"
echo -e "\v\v\v\v"
echo "============"
echo;echo
echo "Quotation mark"
echo -e "\042"
echo "============"

echo; echo "NEWLINE and BEEP"
echo $'\n'
echo $'\a'
echo $'\t \042 \t'
echo $'\t \x22 \t'
echo 
quote=$'\042'
echo "$quote Quoted string $quote and the lies outside"
echo "---------"
ABD=$'\101\102\103\010'
echo $ABC
echo
exit 0
```


### Output:

![[Pasted image 20230628170155.png]]

### Explanation:

* Here is example while echo a escaped character how will get results

### Things know:

* 