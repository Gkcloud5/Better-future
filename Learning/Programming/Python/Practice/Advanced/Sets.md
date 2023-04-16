#Advanced #sets

#### Source:
[Sets](https://www.learnpython.org/en/Sets)
[Youtube](https://www.youtube.com/watch?v=TYPiYLlKIPk)

**Sets are lists with no duplicate entries. let's say you want to collect a list of words used in a paragraph**

Set is immutable object

Set does not have index

```
print(set("My name is GK and i am a hope guy, my friend name is ragu".split()))
```

![[Pasted image 20230416125841.png]]

##### intersection:

```
a = set(["GK", "Hope", "Hardwork"])
b = set(["patience", "dedication", "GK"])

print(a.intersection(b))
print(b.intersection(a))
```
![[Pasted image 20230416130207.png]]

**Same name in two lists

##### symmetric difference:
```
print(a.symmetric_difference(b))
print(b.symmetric_difference(a))
```

![[Pasted image 20230416130347.png]]


##### difference:

```
print(a.difference(b))
print(b.difference(a))
```

![[Pasted image 20230416130451.png]]


##### union:
```
print(a.union(b))
```
![[Pasted image 20230416130556.png]]

##### add a value in set:
```
a.add()
```