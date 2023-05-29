#### Source:
[HR](https://www.hackerrank.com/challenges/find-second-maximum-number-in-a-list/problem?isFullScreen=true)

#### Question:

![[Pasted image 20230529194208.png]]


#### Solution 1:(using direct method)

```
n = int(input())
arr = map(int, input().split())
    
arr = list(arr)

list_new = []

[list_new.append(x) for x in arr if x not in list_new]

list_new.sort()


print (len(list_new))
print (list_new[(int(len(list_new)) - 2)])
```


#### Solution 2:(Using Function)

```

```