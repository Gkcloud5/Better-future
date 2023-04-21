#### Exercise:
**Display a numbers from a list using loop**
* The number must be divisible by five
* If the number is greater than 150, then skip it and move to the next number
* If the number is greater than 500, then stop the loop

#### Sample output:

![[Pasted image 20230421172028.png]]


#### Logic Think:
* Number divided by 5
* if number is above 150 then skip and move next number
* if number is above 500 then stop the loop

#### Program:

```
numbers = [12, 75, 150, 180, 145, 525, 50]

for i in numbers:
   if i % 5 == 0:
      while i > 150:
          continue
      while i > 500:
          break
   print(i)
```


#### Output:
![[Pasted image 20230421173814.png]]
