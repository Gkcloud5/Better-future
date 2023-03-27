#### Source: [function](https://www.programiz.com/python-programming/function)

A function is a block of code that performs a specific task

Dividing a complex problem into smaller chunks makes our program easy to understand and reuse


### Types of function:
2 Types of function:
* **Standard library functions** -- These are built-in functions in python that are available to use.
* **User-defined functions** -- We can create our own functions based on our requirements

#### Function declaration:

##### Syntax:
```
def function_name(arguments):
    # function body 

    return
```

![[Pasted image 20230327190944.png]]

##### Example 1:
```
def greet():
    print('Hello World!')
```

![[Pasted image 20230327191536.png]]


#### Python function arguments:
An argument is a value that is accepted by a function.

##### Example 1:
```
# function with two arguments
def add_numbers(num1, num2):
    sum = num1 + num2
    print('Sum: ',sum)

# function with no argument
def add_numbers():
    # code
```

![[Pasted image 20230327191741.png]]

##### Return statement in python:

If we want our function to return some value to a function call, use the `return` statement.

```
def add_numbers():
    ...
    return sum
```