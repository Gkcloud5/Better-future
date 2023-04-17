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
    print("Test function")
```