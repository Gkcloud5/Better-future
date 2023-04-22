#### Exercise:
**Concatenate two lists index-wise**
	Write a program to add two lists index-wise. Create a new list that contains the 0th index item from both the list, then the 1st index item, and so on till the last element. and leftover items will get added at the end of the new list.

#### Example output:

![[Pasted image 20230422232819.png]]

#### Logic think:
* Need to get a values from index and add it later store in one index

#### Program:

```
#### Soultion 1:
list1 = ["M", "na", "i", "Ke"]
list2 = ["y", "me", "s", "lly"]

list1_len =len(list1)
list2_len =len(list2)

len = list1_len
#print(len)
if list1_len < list2_len:
    len = list2_len
    #print("inside if", len)
word1 = ""
word2 = ""
list = []
for i in range(0,len):
    word1 = list1[i]
    word2 = list2[i]
    word = word1+word2
    list.append(word)
    #print(list)

print(list)
```

```
#### Soultion 2:
list1 = ["M", "na", "i", "Ke"] 
list2 = ["y", "me", "s", "lly"]
list3 = [i + j for i, j in zip(list1, list2)]
print(list3)
```

#### Output:
![[Pasted image 20230423001916.png]]
