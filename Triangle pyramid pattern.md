#Pattern #logical #Python

#### Source:
[Youtube](https://www.youtube.com/watch?v=Yz4wy4OuoCE&list=PLIFRUdRwOM0_2VMQ_8BBY4SIEXNjkwfW5&index=3)

#### Need to print:
```
    *
   * *
  * * *
 * * * * 
* * * * *
```

#### Program:
```
rows = int(input("enter a number"))
space = rows-1
for i in range(0,rows):
    for j in range(0, space):
        print(end = " ")
    space = space - 1
    for k in range(0, i+1):
        print("* ", end = " ")
    print() 
```

##### Program logic information:
```
rows = int(input("enter a number"))
```
* Getting input from user, how many row we need to print

```
space = rows-1
```
* The above line will help to determine a space in output

```
for i in range(0,rows):
print() 
```
* This will decide how many rows we need to print.

```
space = rows-1
for j in range(0, space):
        print(end = " ")
    space = space - 1
```
* These lines are helps to give space before astrix in output
* 
