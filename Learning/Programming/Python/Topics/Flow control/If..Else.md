##### Source: [if..Else](https://www.programiz.com/python-programming/if-elif-else)

If condition used to run a function only condition is true.

**3 Statements**
* `if` statement
* `if..else` statement
* `if..elif..else` statement

#### IF statement:
 Syntax:
```
if condition:
    # body of if statement
```

![[Pasted image 20230319195954.png]]

##### Example1:

```
number = 10

# check if number is greater than 0
if number > 0:
    print('Number is positive.')

print('The if statement is easy')
```


#### If..Else Statement:

Syntax:
 ```
 if condition:
    # block of code if condition is True

else:
    # block of code if condition is False
```

![[Pasted image 20230319200142.png]]


#### If...Elif...else statement:

It used to check 2 conditions

##### Syntax:

```
if condition1:
    # code block 1

elif condition2:
    # code block 2

else: 
    # code block 3
```

![[Pasted image 20230319200453.png]]

#### Nested If:

 `If` statement inside of an `if` statement

**Syntax**:

```
# outer if statement
if condition1:
    # statement(s)

    # inner if statement
    if condition2: 
        # statement(s)
```


![[Pasted image 20230319200639.png]]

##### Example of nested IF:

```
number = 5

# outer if statement
if (number >= 0):
    # inner if statement
    if number == 0:
      print('Number is 0')
    
    # inner else statement
    else:
        print('Number is positive')

# outer else statement
else:
    print('Number is negative')

# Output: Number is positive
```

