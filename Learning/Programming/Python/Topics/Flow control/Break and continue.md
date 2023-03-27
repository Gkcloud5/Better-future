#### Source: [Break&continue](https://www.programiz.com/python-programming/break-continue)

### Break:
**Break statement is used to terminate the loop immediately when it is encountered**

##### Syntax: 
`break`

![[Pasted image 20230327184902.png]]


##### Example 1:

```
for i in range(5):
    if i == 3:
        break
    print(i)
```

![[Pasted image 20230327184943.png]]

##### Example 2:

```
# program to find first 5 multiples of 6

i = 1

while i <= 10:
    print('6 * ',(i), '=',6 * i)

    if i >= 5:
        break
    
    i = i + 1
```

![[Pasted image 20230327185021.png]]

### Continue:
**It is used to skip the current iteration of the loop, then the control of the program jumps to the next iteration**

```
for i in range(5):
    if i == 3:
        continue
    print(i)
```

![[Pasted image 20230327185445.png]]


##### Example 2:

```
# program to print odd numbers from 1 to 10

num = 0

while num < 10:
    num += 1
    
    if (num % 2) == 0:
        continue

    print(num)
```

![[Pasted image 20230327185614.png]]

