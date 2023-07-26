#Basics #Class #Object #Python 

#### Source: [Class and objects](https://www.learnpython.org/en/Classes_and_Objects)

**Objects are an encapsulation of variable and function into single entity. Objects get their variables and functions from classes.**

**Class have related function and data**

```
class GK:
    def __init__(self, name, age, work):
        self.name = name
        self.age = age
        self.work = work

Gokul =  GK("Gokul", 26, "Sysadmin")

print(Gokul.name)

```

**Object is a data that we gave and get from class

![[Pasted image 20230412211230.png]]

##### Example2:
```
class ex1:
    str1="Gk"

    def function(self):
        print("This is class")

myobj =  ex1()

print (myobj.str1)
myobj.function
```

![[Pasted image 20230412213048.png]]


#### Test:

```
# define the Vehicle class
class Vehicle:
    name = ""
    kind = "car"
    color = ""
    value = 100.00
    def description(self):
        desc_str = "%s is a %s %s worth $%.2f." % (self.name, self.color, self.kind, self.value)
        return desc_str

# your code goes here
car1 = Vehicle()
car1.name = "Fer"
car1.color = "red"
car1.kind = "convertible"
car1.value = 60000.00

car2 = Vehicle()
car2.name = "Jump"
car2.color = "blue"
car2.kind = "van"
car2.value = 10000.00

# test code
print(car1.description())
print(car2.description())
```

![[Pasted image 20230412213713.png]]
