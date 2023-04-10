#string #Basics 

#### Source: [string operations](https://www.learnpython.org/en/Basic_String_Operations)

**Strings can be defined as anything between quotes

```
str1="Gk"
str2='Hope'
```

##### Length of string:
```
str1= "Hello world!"
print(len(str1))
```

![[Pasted image 20230410235216.png]]

##### Index in string:
```
str1="Gk is a Hope guy"
print(str1.index(o))
```

![[Pasted image 20230411000109.png]]
* This only takes first instance

##### Count in string:
```
str1="Gk is a Hope guy and Gk is working hard for better future"
print(str1.count("e"))
```
![[Pasted image 20230411000407.png]]


##### Slice a string:
```
str1="Hello all myself gokul, i am learning python now"
print(str1[3:9])
```
![[Pasted image 20230411000603.png]]
* Output from index 4 to 8

##### reveres a string:
```
str1="welcome to my page"
print(str1[::-1])
```

##### Check string starts and end with particular line:
```
str1="it's me gokul"
print(str1.startswith("Hello"))
print(str1.endswith("thanks"))
```

##### Split a string:
```
str1="Gk hope guy"
str2=str1.split(" ")
print(str2)
```