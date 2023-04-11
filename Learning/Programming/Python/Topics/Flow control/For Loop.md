#flowcontrol 
##### Source: [Loop](https://www.programiz.com/python-programming/for-loop)

**Loops are used to repeat a block of code**

#### 2 Types of loops:

* for loop
* while loop

#### for loop:
 It is used to run a block of code for a certain number of times, it is used to iterate over any sequence such as list, tuple, string.

##### Syntax:

```
for val in sequence:
    # statement(s)
```

*Here **VAL** access each item of sequence on each iteration. Loop continues until we reach the last item in the sequence.*

##### Flowchart:

![[Pasted image 20230319201313.png]]

##### Example 1:

```
languages = ['Swift', 'Python', 'Go', 'JavaScript']

# access items of a list using for loop
for language in languages:
    print(language)
```

![[Pasted image 20230319201346.png]]

#### For loop with range:

**range() is a python built-in function** 

##### Example 2:

```
# use of range() to define a range of values
values = range(4)

# iterate from i = 0 to i = 3
for i in values:
    print(i)
```

![[Pasted image 20230319202746.png]]

#### For loop with else:

```
digits = [0, 1, 5]

for i in digits:
    print(i)
else:
    print("No items left.")
```

![[Pasted image 20230319202856.png]]


### IDE: [[Loops]]