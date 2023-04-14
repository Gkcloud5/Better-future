#Advanced #list 

#### Source: [list](https://www.learnpython.org/en/List_Comprehensions)

**List comprehensions is a very powerful tool, which created a new list on another list, in a single, readable line.**

* We can perform operation in list.

```
##Without using list comprehensions
list_new = [1,2,3,4,5]
list_square=[]
for i in list_new:
    square = i ** 2
    list_square.append(square)
print(list_square)
```

```
##With list comprehensions
list_square_new = [sqaure_new ** 2 for square_new in list_new]
print(list_square_new )
```