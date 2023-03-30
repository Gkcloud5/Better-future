#### Source: [Global and local](https://www.programiz.com/python-programming/global-local-nonlocal-variables)

In python we can declare a variable in 3 different scopes
* Local scope
* Global scope
* Non-local scope

**A variable scope specifies the region where we can access a variable.**

```
def add_numbers():
  sum= 5+4
```
* Here `sum` variable created a inside function, so it can only be accessed within it *local scope*

#### Local variables:
* When we declare a variable inside function, these variables will have a local scope, we cannot access them outside the function.

```
def greet():
  #local variable
  message = 'Hello'
  print('Local', message)

greet()

#Try to access message variable
print(message)
```

