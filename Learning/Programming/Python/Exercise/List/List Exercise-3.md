#### Exercise:
**Turn every item of a list into it's square**
  Given a list of numbers. write a program to turn every item of a list into its square.

#### Expected output:

![[Pasted image 20230423123004.png]]

#### Logic think:
* iterate a given list
* square a iterated values
* create a new list

#### Program:

```
numbers = [1, 2, 3, 4, 5, 6, 7]

square_list=[i*i for i in numbers]
print(square_list)
```

```
#Soultion1
numbers = [1, 2, 3, 4, 5, 6, 7]
# result list
res = []
for i in numbers:
    # calculate square and add to the result list
    res.append(i * i)
print(res)
```

#### Output:

![[Pasted image 20230423123455.png]]

