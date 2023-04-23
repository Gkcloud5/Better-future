#### Exercise:
**Get only unique items from two sets**
 Write a program to return a new set with unique items from both sets by removing duplicates

#### Expected output:

![[Pasted image 20230423180914.png]]


#### Logic think:

* We need to use `union` for this task

#### Program:

```
set1 = {10, 20, 30, 40, 50}
set2 = {30, 40, 50, 60, 70}

set = set1 | set2
print(set)

set_new = set1.union(set2)
print()
```