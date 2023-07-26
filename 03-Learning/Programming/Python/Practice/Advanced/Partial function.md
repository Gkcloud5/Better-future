#Advanced #Functions  #Python 

#### Source:
[Partial](https://www.learnpython.org/en/Partial_functions)
[Youtube](https://www.youtube.com/watch?v=mWcFMrrQR4A)

**Partial function is a copy of normal function but we restrict arguments here**

```
##normal function
from operator import mul
print(mul(3,4))
print(mul(4,4))
```

![[Pasted image 20230416172644.png]]

```
##partial function
from functools import partial
mul1 = partial(mul,4)
print(mul1)
print(mul1(2))
```

![[Pasted image 20230416172922.png]]

