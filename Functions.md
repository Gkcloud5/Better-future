#Basics #Functions

#### Source: [Functions](https://www.learnpython.org/en/Functions)

**Functions are a convenient way to divide your code into useful blocks, allowing us to order our code, make it more readable, reuse it and save some time.**

```
block_head:
    1st block line
    2nd block line
    ...
```

##### Example:

```
def my_function():
    print("Gk is hope")

my_function()
```


##### Passing arguments in function:
```
def func(name,age):
    print("my name is %s" %(name))
    print("My age is %d" %(age))

func(gokul,26)
```

![[Pasted image 20230411231003.png]]

##### return:

```
def add_num(a,b):
    return a + b

x = add_num(10,12)
print(x)
```

##### Test:
```
# Modify this function to return a list of strings as defined above
def list_benefits():
    return ["More organized code", "More readable code", "Easier code reuse", "Allowing programmers to share and connect code together"]

# Modify this function to concatenate to each benefit - " is a benefit of functions!"
def build_sentence(benefit):
    return benefit + " is a benefit of functions!"

def name_the_benefits_of_functions():
    list_of_benefits = list_benefits()
    for benefit in list_of_benefits:
        print(build_sentence(benefit))

name_the_benefits_of_functions()
```