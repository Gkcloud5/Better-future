---
creation date: 2023-06-17 01:44
modification date: Saturday 17th June 2023 01:44:57
---

**Tags:** 

#### Source:
[HR](https://www.hackerrank.com/challenges/python-string-formatting/problem?isFullScreen=true)

--------------------------------------

#### Question:

![[Pasted image 20230617014543.png]]

![[Pasted image 20230617014551.png]]


#### Solution 1: own

```
from decimal import Decimal

def print_formatted(number):
    width = len(bin(number)[2:])
    # your code goes here
    oct_value=""
    hex_value=""
    bin_value=""
    for i in range(1,number+1):
        Decimal_value = Decimal(i)
        dec_value = str(Decimal_value)
        oct_value = oct(i)
        hex_value=hex(i)
        bin_value=bin(i)
        print (dec_value.rjust(width), oct_value.replace("0o", "").rjust(width), hex_value.replace("0x","").upper().rjust(width), bin_value.replace("0b","").rjust(width) )
        # hex(i), bin(i))

if __name__ == '__main__':
    n = int(input())
    print_formatted(n)
```

#### Solution - 2: chatGPT

```
def print_formatted(number):
    width = len(bin(number)[2:])  # Calculate the width based on binary representation
    for i in range(1, number + 1):
        decimal = str(i)
        octal = oct(i)[2:]
        hexadecimal = hex(i)[2:].upper()
        binary = bin(i)[2:]
        print(f"{decimal.rjust(width)} {octal.rjust(width)} {hexadecimal.rjust(width)} {binary.rjust(width)}")

# Test the function
n = int(input("Enter a number: "))
print_formatted(n)
```


