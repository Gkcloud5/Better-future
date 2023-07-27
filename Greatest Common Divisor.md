---
creation date: 2023-07-27 16:46
modification date: Thursday 27th July 2023 16:46:30
---

### Script:[](https://tldp.org/LDP/abs/html/ops.html#GCD)

```
#!/bin/bash

ARGS=2
E_BADARGS=85

if [ $# -ne "$ARGS"]
then
    echo "Usage: `bashname $0` first-number second-number"
    exit $E_BADARGS
fi

gcd ()
{
  dividend=$1
  divisor=$2
  remainder=1
  until [ "$remainder" -eq 0 ]
  do 
	let "remainder = $dividend % $divisor"
	dividend=$divisor
	divisor=$remainder
  done
}

gcd $1 $2
echo; echo "GCD of $1 and $2 = $dividend"
```

### Output:



### Explanation:

* `=` assignment operator
	* var=27
* Arithmetic operator
	* +
	* -
	* *
	* /
	* **
	* % --> return remainder

### Things know:
