#Basics #Dictionaries #Python 

#### Source: [Dictionaries](https://www.learnpython.org/en/Dictionaries)

* A dictionary is a data types similar to arrays, but works with keys and values instead of indexes.
* Each value stored in a dictionary can be accessed using a key, which is any type of object(string, number, list)
```
Gk = {}
Gk["regno"] = 175
Gk["age"] = 26
Gk["name"] =  "Gk-Hope"

print(Gk)
```

![[Pasted image 20230412215712.png]]

#### Iterating over dictionaries:

```
Gk1 = {"Gk": 26, "Hope": 28}
for name, age in Gk1.items():
    print("My name %s and my age is %s" %(name, age))

```

**Number(age) also string here

![[Pasted image 20230412220611.png]]


#### Dictionaries add and remove:

```
###add a object

stud = {
   "Gk" : 12
   "Hope": 16
}

stud["hardwork"] = 1

del stud["Hope"]
print(stud)
```

![[Pasted image 20230412221520.png]]

