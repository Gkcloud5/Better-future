#Basics #Dictionaries

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
Gk = {"name": "Gokul", "age": 26}
for name, age in Gk.items():
    print("My name %s and my age is %d" %(name, age))

```