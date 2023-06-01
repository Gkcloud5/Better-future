#### Exercise:
**Remove a items from the set**

#### Sample output:

![[Pasted image 20230423181856.png]]


#### Logic think:

* we can use `remove` method to vomit selected values // this method only remove one character
* Or we can use `difference_update()` method

#### Program:

```
set1 = {10, 20, 30, 40, 50}

print(set1.difference_update(10,20,30))
```


#### Output:

![[Pasted image 20230423182334.png]]

