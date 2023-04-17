#Advanced #Map #Filter #Reduce

#### Source:
[Map, filter](https://www.learnpython.org/en/Map%2C_Filter%2C_Reduce)
[Youtube-1](https://www.youtube.com/watch?v=G4r1IBMdF7c&pp=ygUSTWFwLCAgcHlodG9uIHRhbWls)
[Youtube-2](https://www.youtube.com/watch?v=2E21RpSOZSA)

### Map():
 It take input from list, tiple. pass a each value to function and return map output.

```
def add(n):
    return n + n

values = (1,2,3,4,5)

result = map(add, values)
print(list(result))
```

![[Pasted image 20230417221644.png]]


##### Example1:
```
#Convert string to int
numbers=["5", "12", "34", "21"]
print(type(numbers[0]))
numbers=list(map(int,numbers))
print(type(numbers[0]))

```

![[Pasted image 20230417222809.png]]

