---
creation date: 2023-08-01 17:57
modification date: Tuesday 1st August 2023 17:57:21
---

### Script:[](https://tldp.org/LDP/abs/html/numerical-constants.html#NUMBERS)

```
#!/bin/bash

let "dec=32"
echo "decimal number = $dec"

let "oct = 032"
echo "octal number = $oct"

let "hex = 0x32"
echo "Hex number = $hex"
```

### Output:

![[Pasted image 20230801180509.png]]

### Explanation:

* number prefix with 0 then it's octal
* prefix with 0x then it's hexadecimal

