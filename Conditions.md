#Basics #Conditions

#### Source: [Condition](https://www.learnpython.org/en/Conditions)

Python uses boolean logic to evaluate conditions. the boolean values true and false are returned when an expression is compared or evaluated.

```
num1=1
print(num1 == 2)
print(num1 == 1)
```
![[Pasted image 20230411200134.png]]

* == Comparison operator

#### Boolean operators:

* `and` ,`or` operators

```
name = "GK"
Age = 26
if name == "GK" and age = 26:
    print("My name is gokul and i am 26 year old")

if name == "GK" or name == "Hope"
    print(My name is GK)
```

![[Pasted image 20230411200651.png]]

##### "in" operator:
* `in` operator could be used to check if a specified object exists within an iterable object container.

```
name = "Gk"
if name in ["Gk", "Hope"]
    print("Your name is GK or Hope")
```

![[Pasted image 20230411201016.png]]

##### If...else...if condition:

```
str1 = False
str2 = True

if str1 is True:
    print($str1)
elif str2 is True:
    print("str2 value")
else:
	pass
```

![[Pasted image 20230411202030.png]]

##### is operator:
* It is not same as ``==`` operators, it print true only match address same like should be same object

```
num1 = 5
num2 =5

list1 = [1,2,3]
list2 = [1,2,3]

print(id(num1))
print(id(num2))

print(id(list1))
print(id(list2))
```