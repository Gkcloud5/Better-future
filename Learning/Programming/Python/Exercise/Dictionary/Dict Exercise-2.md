#### Exercise:
**Merge two python dictionaries into one**

#### Sample output:

![[Pasted image 20230423135812.png]]

#### Logic think:
* concatenate two dictionary
* If any value common in both dictionary then need to print that value only once.
* python have special function for this kind of operation `update` 

#### Program:

```
#Soution-1

dict1 = {'Ten': 10, 'Twenty': 20, 'Thirty': 30}
dict2 = {'Thirty': 30, 'Fourty': 40, 'Fifty': 50}

# copy second dictionary into first dictionary
dict1.update(dict2)
# printing the updated dictionary
print(dict1)


## Soultion-2
dict1 = {'Ten': 10, 'Twenty': 20, 'Thirty': 30}
dict2 = {'Thirty': 30, 'Fourty': 40, 'Fifty': 50}
dict3 = {**dict1, **dict2}
print(dict3)
```

#### Output:

![[Pasted image 20230423140505.png]]
