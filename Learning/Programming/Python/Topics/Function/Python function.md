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

**The return statement also denotes that the function has ended. Any code after return is not executed**

##### Example 1:
```
# function definition
def find_square(num):
    result = num * num
    return result

# function call
square = find_square(3)

print('Square:',square)

# Output: Square: 9
```


### Benefits of using function:

1. Code reusable:
   We can use same function multiple times in our program which makes our code reusable.

```
# function definition
def get_square(num):
    return num * num

for i in [1,2,3]:
    # function call
    result = get_square(i)
    print('Square of',i, '=',result)
```

![[Pasted image 20230327193141.png]]

2. Code readability:
    Function help us break our code into chunks to make our program readable and easy to understand.

