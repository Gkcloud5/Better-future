#### Source: [Recursion](https://www.programiz.com/python-programming/recursion)

**A function that calls itself is know as recursive function**

![[Pasted image 20230329200052.png]]


##### Example:

```
def factorial(x):
    """This is a recursive function
    to find the factorial of an integer"""

    if x == 1:
        return 1
    else:
        return (x * factorial(x-1))


num = 3
print("The factorial of", num, "is", factorial(num))
```

![[Pasted image 20230329200206.png]]

![[Pasted image 20230330200658.png]]

