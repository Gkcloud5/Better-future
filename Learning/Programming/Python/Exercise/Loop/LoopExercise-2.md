#### Exercise:
 **Print the following pattern by using loop**

![[Pasted image 20230421145501.png]]

#### Logic Think:
* Need to know how many rows we need
* Here printable value is number so we need to think regarding that

#### Program:

```
num = int(input("Enter a number"))

for i in range (1, num+1):
    for j in range (1, i+1):
       print(j, end =" ")
    print()
```

#### Output:

![[Pasted image 20230421152824.png]]