https://www.hackerrank.com/challenges/py-if-else/problem?isFullScreen=true



Solution:

```
if n % 2 == 1:
    print ("Weird")
else:
    if 6 <= n <= 20:
        print ("Weird")
    elif 2 <= n <=5 or n >= 20:
        print ("Not Weird")
```