#### Source: [Argument](https://www.programiz.com/python-programming/function-argument)

**Argument is a value that is accepted by a function**

##### Example 1:

```
def add_numbers(a, b):
    sum = a + b
    print('Sum:', sum)

add_numbers(2, 3)

# Output: Sum: 5
```

- In above example, the function `add_numbers` takes two parameters: `a` and `b`.

##### Example 2: Function Argument with default values

```
def add_numbers( a = 7,  b = 8):
    sum = a + b
    print('Sum:', sum)


# function call with two arguments
add_numbers(2, 3)

#  function call with one argument
add_numbers(a = 2)

# function call with no arguments
add_numbers()
```

![[Pasted image 20230329195702.png]]


##### Example 3: Python keyword Argument

```
def display_info(first_name, last_name):
    print('First Name:', first_name)
    print('Last Name:', last_name)

display_info(last_name = 'Cartman', first_name = 'Eric')
```

![[Pasted image 20230329195755.png]]

