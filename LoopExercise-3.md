#### Exercise:
**Calculate the sum of all numbers from 1 to given number**

#### Sample output:

![[Pasted image 20230421152954.png]]

#### Logic Think:
* Need to get input from user
* Value must start from 1 and end from user input value

#### Program:

```
num = int(input("Enter a number"))
sum=0

for i in range (1, num+1):
    sum = sum + i
    #print(i, sum)
print(sum)
```

#### Output:

![[Pasted image 20230421153313.png]]

