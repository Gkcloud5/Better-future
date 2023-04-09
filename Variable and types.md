#Basics 

#### Source: [Variable and types](https://www.learnpython.org/en/Variables_and_Types)

**Python is completely object oriented and not "statically typed". you do not need to declare variable before using them or declare their type. Each variable in python is an object.**


#### Numbers:
* Python supports two type of numbers
	* Integer
	* Floating
```
num=7
print(num)

#Declare a float value
float_value=8.0
print(float_value)
float_value=float(7)
print(float_value)
```

##### Output:
![[Pasted image 20230409191311.png]]

#### Strings:
* It defined either single quote or a double quote

```
my_str1='Gk'
print(my_str1)

my_str2="Gkloud"
print(my_str2)
```

If you use double quote then you can add single quote inside a content easily

```
mystring = "Don't worry about apostrophes"
print(mystring)
```

##### Operators executed in string and numbers:

```
first=1
second=2
third=first+second
print(third)
```

```
str1='GK'
str2='Hope'
str3=str1+str2
print(str3)
```

![[Pasted image 20230409192057.png]]

##### Assigning one or more variable at same time

```
a, b = 3, 4
print(a, b)
```

**Mixing operators between numbers and strings is not supported**

```
# This will not work!
one = 1
two = 2
hello = "hello"

print(one + two + hello)
```

![[Pasted image 20230409192122.png]]
