#Advanced #lambda #Python 

#### Source: 
[lambda](https://www.learnpython.org/en/Lambda_functions)
[youtube](https://www.youtube.com/watch?v=3wIXSaOL0Mk)

**Anonyms function, we can use `n` number of argument and store in a single variable

```
##Syntax
lambda arguments : expression
```

```
x = lambda x : x * 10
print(x(5))

x = lambda x,y: x * 10 + y
print(x(7,2))
```

![[Pasted image 20230414225537.png]]

##### Example 1:

```
l = [2,4,7,3,14,19]
for i in l:
    # your code here
    my_lambda = lambda x : (x % 2) == 1
    print(my_lambda(i))
```

![[Pasted image 20230414230138.png]]

