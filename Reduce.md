#Advanced #Reduce

#### Source:
[Reduce](https://www.learnpython.org/en/Map%2C_Filter%2C_Reduce)
[Youtube](https://www.youtube.com/watch?v=2E21RpSOZSA)

**Reduce applies a function of two arguments cumulatively to the elements of an iterable, optionally starting with an initial argument.**

```
reduce(func, iterbale[, initial])
```

##### Example 1:
```
##without reduce
from functools import reduce

list1 = [1, 2, 3, 4]
num=0
for i in list1:
    num=num+i
print(num)
```

![[Pasted image 20230418162454.png]]

```
#With reduce

```