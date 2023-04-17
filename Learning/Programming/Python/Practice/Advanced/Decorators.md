#Advanced #Decorators

#### Source:
[Decorators](https://www.learnpython.org/en/Decorators)
[Youtube](https://www.youtube.com/watch?v=ffUekX06xZ0)

#### What is decorator:
  Change behavior's of function without modifying function. 

```
def this_is_dec(func):
    def youtube():
        print("Entering into dec")
        func()
        print("One function called")
    return youtube

def test():
    print("i am a test function")

test = this_is_dec(test) // method 1 to call
test()
```

![[Pasted image 20230417202613.png]]


```
def this_is_dec(func):
    def youtube():
        print("Entering into dec")
        func()
        print("One function called")
    return youtube

@this_is_dec //method 2 call a decorator
def test():
    print("i am a test function")


test()
```
