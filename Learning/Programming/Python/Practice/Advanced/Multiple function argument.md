#Advanced #Functions 

#### Source: 
[Multiple function](https://www.learnpython.org/en/Multiple_Function_Arguments)

**Every function in python receives a predefined number of arguments**
```
def myFunc(first, second, third):
    # do something
    ...
```

##### Send a argument to functions:

```
def foo(first, second, third, *therest):
    print("First: %s" %(first))
    print("Second: %s" %(second))
    print("Third: %s" %(third))
    print("And all the rest... %s" %(list(therest)))

foo(1, 2, 3, 4, 5)
```

![[Pasted image 20230415122750.png]]

