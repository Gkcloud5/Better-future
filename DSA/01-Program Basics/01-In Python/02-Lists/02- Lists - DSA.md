---
creation date: 2023-07-19 18:09
modification date: Wednesday 19th July 2023 18:09:06
---

**Tags:** #DSA 

#### Source:
[YT](https://www.youtube.com/watch?v=efkCQKiFTUc&list=PLhP5RsB7fhE28lfOcyi9JB31mrBSf4wgL&index=8)

--------------------------------------

### Explanation about it:

#### Indexing:

* It's based on zero based.
* It stored in contiguous memory location
	* Starts with 0
* Backward indexing
	* it starts with -1 -2 -3

```
lst = [1,2,3]

print(lst[0])
```

![[Pasted image 20230719181455.png]]

##### Mutability:

* It means we can alter or made change inside given list
	* Add one new variable from list
	* Remove any variable from list
	* tuple, string, integer is not mutability

##### Traversal:

* We can iterate a list one by one

```
lst = [1,2,3]
for i in lst:
    print(i)
```

![[Pasted image 20230719182124.png]]

### List Functions:

##### length()

* `len()`
```
lst = [1,2,3]
print(len(lst))
```

![[Pasted image 20230719182236.png]]

```
lst = [1,2,3]
print(min(lst))
print(max(lst))
```

![[Pasted image 20230719182428.png]]


##### Append():
* it used to add a element in last
 
```
lst = [1,2,3]
lst.append(4)
print(lst)
```

![[Pasted image 20230719183413.png]]

##### insert():
* Add a element with position value
* It expect two arguments
	* 1st --> Position of index
	* 2nd --> value that need to add

```
lst = [1,2,3]
lst.insert(0,4)
print(lst)
```

![[Pasted image 20230719184114.png]]

##### extend():
* Add multiple value at end

```
lst1 = [1,2,3]
lst2 = [2,3,4]
lst1.extend(lst2)
print(lst1)
```

![[Pasted image 20230719184202.png]]

##### Nested list:

* List inside list

```
#[1,2,3,[1,2,3]] 
```

##### remove()
* It remove value that we give
	* First occurance

```
lst = [1,2,3,1]
lst.remove(1)
print(lst)
```

![[Pasted image 20230719185215.png]]


##### Pop()
* remove element based on index

```
lst = [1,2,3,1]
element = lst.pop(2)
print(lst)
print(element)
```

![[Pasted image 20230719185818.png]]


##### Sort()
* make order of given list

```
lst = [1,3,4,2,6,3]
lst.sort()
print(lst)
lst.sort(revers=True)
print(lst)
```

![[Pasted image 20230719190041.png]]

#### Create a list:

```
lst = list('Troll Geek')
print(lst)
```

![[Pasted image 20230719190209.png]]

