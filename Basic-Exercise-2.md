#### Exercise:
**Print the sum of the current number and the previous number**
 Write a program to iterate the first 10 numbers and in each iteration, print the sum of the current and previous number

#### Sample output:

![[Pasted image 20230419223320.png]]

#### Logic Think:

* Need to get input 10
* need to add current number + previous number
* need to print previous number also

#### Program:

```
n = int(input("Enter a number"))
prev = 0
for i in range(n):
    sum = prev + i
    print("Current number", i, "Previous number", prev,"Sum:", sum)
    prev = i
    
```


#### Output:

![[Pasted image 20230419224816.png]]

