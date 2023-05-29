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

```python
n = int(input())
arr = map(int, input().split())

#convert to list   
arr = list(arr)


#Function for get runner value
def list_runner(arr):
    list_score = []
    for x in arr:
       if x not in list_score:
           list_score.append(x)
    list_score.sort()
    len_list = len(list_score)
    return list_score[(len_list-2)]

#Function assigned to variable
list_new = list_runner(arr)
    
print(list_new)
```

