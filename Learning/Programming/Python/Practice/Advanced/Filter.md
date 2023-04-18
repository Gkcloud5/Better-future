#Advanced #Filter

#### Source:
[Filter](https://www.learnpython.org/en/Map%2C_Filter%2C_Reduce)
[Youtube1](https://www.youtube.com/watch?v=2E21RpSOZSA)
[Youtube-2](https://www.youtube.com/watch?v=keJmkX-hFE0)

**Filter function helps to get only true values.**

```
filter(func, *iterables*)
```


##### Example1:
```
num = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
def filter_numbers(data):
    if data % 2 == 0:
       return True
    else:
       return False

answer = filter(filter_numbers, num)
print(list(answer))
```

![[Pasted image 20230418160718.png]]


##### Example 2:
```
Mark = [12, 34, 56, 75, 87, 36, 63, 55]
def is_pass(score)
    return score > 36

over_35 = list(filter(is_pass, Mark))
print()
```