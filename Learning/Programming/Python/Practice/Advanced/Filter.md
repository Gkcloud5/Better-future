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
    else
       return False

answer = filter(filter_numbers, num)
print(list(answer))
```