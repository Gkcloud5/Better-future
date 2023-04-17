#Advanced #Closures

#### Source:
[Closure](https://www.learnpython.org/en/Closures)
[Youtube](https://www.youtube.com/watch?v=1ZN90qk80l0)

##### Nested function:
 Nested function is a function defined inside another function. it's very important to note that the nested functions can access the variables of the enclosing scope.

##### Non-local variable:
  Outer function variable only read only when we execute it in local function.

```
def transmit_to_space(message):
    "This is the enclosing function"
    def data_transmitter():
        "The nested function"
        print(message)

    data_transmitter()

print(transmit_to_space("Test message"))
```

![[Pasted image 20230417175235.png]]

##### Example 2:
```
def transmit(message):
    def data_transfer():
        print(message)
    return data_transfer

fun2 = transmit("Gk is a hope guy")
fun2()
```

![[Pasted image 20230417175656.png]]


##### Example 3:
```
def outer_function(msg):
    data = msg
    def inner_function():
        print(data)
    inner_function()

outer_function("Gk")
```

![[Pasted image 20230417180618.png]]

##### Example 4:
```
def outer_function(msg):
    data = msg
    def inner_function():
        print(data)
    return inner_function

func = outer_function("Gk")
del outer_function
func() //func stored a value after outer function deleted
try:
   outer_function()
except:
   print("Outer function is deleted")

```
![[Pasted image 20230417181344.png]]

