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
###Own solution
income = int(input("Enter a income"))

if income <= 10000:
    print("No tax")

if 10000 < income:
    if (income < 20000):
      taxable_income = income-10000
      tax = taxable_income * 10 /100
      print(tax)
    
    if (20000 < income):
      taxable_income = income-10000
      tax1 = 10000 * 10/100
      tax2_income = taxable_income - 10000
      tax2 = tax2_income * 20/100
      total_tax = tax1+tax2
      print(total_tax)
```

```

```

#### Output:

![[Pasted image 20230421143406.png]]