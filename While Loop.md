##### Source: [While](https://www.programiz.com/python-programming/while-loop)

**While loop is used to run a block code until a certain condition is met.

##### Syntax:

```
while condition:
    # body of while loop
```

![[Pasted image 20230319203107.png]]

##### Flow chart:
![[Pasted image 20230319203130.png]]



##### Example 1:

```
# program to display numbers from 1 to 5

# initialize the variable
i = 1
n = 5

# while loop from i = 1 to 5
while i <= n:
    print(i)
    i = i + 1
```

![[Pasted image 20230327184212.png]]

##### Example 2:

```
# program to calculate the sum of numbers
# until the user enters zero

total = 0

number = int(input('Enter a number: '))

# add numbers until number is zero
while number != 0:
    total += number    # total = total + number
    
    # take integer input again
    number = int(input('Enter a number: '))
    

print('total =', total)
```

![[Pasted image 20230327184520.png]]

##### While loop with else:

```
counter = 0

while counter < 3:
    print('Inside loop')
    counter = counter + 1
else:
    print('Inside else')
```

![[Pasted image 20230327184606.png]]

