#### Exercise:
**Convert two lists into a dictionary**
  Write a program to convert them into a dictionary in a way that item from list1 is the key and item from list2 is the value

#### Sample output:

![[Pasted image 20230423125519.png]]

#### Logic think:
* Get key and value list and add it
* We can use dictionary comprehension to achieve this thing

#### Program:

```
## Soultion1
keys = ['Ten', 'Twenty', 'Thirty']
values = [10, 20, 30]

Dict_new = {key:value for key,value in zip(keys,values)}
print(Dict_new)


####Soultion2
keys = ['Ten', 'Twenty', 'Thirty']
values = [10, 20, 30]

res_dict = dict(zip(keys, values))
print(res_dict)

```

#### Output:

![[Pasted image 20230423130129.png]]