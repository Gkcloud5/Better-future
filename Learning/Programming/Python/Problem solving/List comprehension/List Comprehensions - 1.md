#### Source:
[HR](https://www.hackerrank.com/challenges/list-comprehensions/problem?isFullScreen=true)

#### Solution1:

```
x = int(input())
y = int(input())
z = int(input())
n = int(input())

#Brief soultion
arr = []
for i in range(x+1):
    for j in range(y+1):
        for k in range(z+1):
            if i + j + k != n:
               arr.append([i,j,k])

print (arr)
```

#### Solution 2:

```

```