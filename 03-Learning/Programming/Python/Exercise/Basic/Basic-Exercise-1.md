
#### Exercise:
**Calculate the multiplication and sum of two numbers**
Given two integer numbers return their product only if the product is equal to or lower than 1000, else return their sum.

#### Sample output:
![[Pasted image 20230419223223.png]]


#### Program:
```
def func(num1, num2)
    mult = num1 * num2
    if mult > 1000:
       mult = num1 + num2
       print(mult)
    else:
       print(mult)

func(20,60)
```

##### Logic think:
* Input two integer
* Multiply a input if value less or equal to 1000
* if multiplication value is more than 1000 then need to add those value

#### Output:
![[Pasted image 20230419222453.png]]
