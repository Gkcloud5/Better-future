#### Exercise:
**Return a new set of identical items from two sets**


#### Expected output:
![[Pasted image 20230423180256.png]]


#### logic think:
* intersection of two sets will return common elements in both sets.

#### Program:

```
set1 = {10, 20, 30, 40, 50}
set2 = {30, 40, 50, 60, 70}

set = set1 & set2
print("&", set)

set_int = set1.intersection(set2)
print("intersection", set_int)
```

#### Output:

![[Pasted image 20230423180555.png]]
