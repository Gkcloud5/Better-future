#### Exercise:
**Calculate income tax for the given income by adhering to the below rules**


#### Sample output:

![[Pasted image 20230420181846.png]]



#### Logic Think:
* If income is less then or equal to 10000 then there is no tax
* If incomes more then 10000 and below 20000 so there is a 10% tax applicable
* If income more then 20000 so there is 20% tax
* If income is 45000 then for first 10000 there is no tax and for next 10000 income tax will be 10% then remaining amount 25000 income tax will be 20%

#### Program:
```
income = int(input("Enter a income"))

if 10000 >= income:
   print("No tax")

if 10000 < income > 
```