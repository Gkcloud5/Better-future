#### Exercise:
**Concatenate two lists in the following order**

#### Expected output:

![[Pasted image 20230423123633.png]]

#### Logic think:
* Need to pass a first list and add a values in second list
	* First list first word + second list both words then need to add another word in second list

#### Program:

```
#Soultion1
list1 = ["Hello ", "take "]
list2 = ["Dear", "Sir"]
word = []
for i in list1:
    for j in list2:
        word.append(i+j)
print(word)
```

```
#Soultion2
list1 = ["Hello ", "take "]
list2 = ["Dear", "Sir"]

res = [x + y for x in list1 for y in list2]
print(res)

```

#### Output:

![[Pasted image 20230423124629.png]]