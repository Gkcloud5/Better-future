#### Source: [Handle Exception](https://www.programiz.com/python-programming/exception-handling)

**Exception abnormally terminate the execution of a program**

```
try...except
```

#### Python try...except Block:

```
try:
 # Code that may cause exception

except:
# Code to run when exception occurs
```

* Every `try` block is followed by an `except` block.

##### Example:

```
try:
    numerator = 10
    denominator = 0

    result = numerator/denominator

    print(result)
except:
    print("Error: Denominator cannot be 0.")

# Output: Error: Denominator cannot be 0. 
```


#### Catching specific exception:

```
try:
    
    even_numbers = [2,4,6,8]
    print(even_numbers[5])

except ZeroDivisionError:
    print("Denominator cannot be 0.")
    
except IndexError:
    print("Index Out of Bound.")

# Output: Index Out of Bound
```

