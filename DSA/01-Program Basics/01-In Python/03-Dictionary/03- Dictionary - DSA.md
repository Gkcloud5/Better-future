
---
creation date: 2023-07-19 19:12
modification date: Wednesday 19th July 2023 19:12:45
---

**Tags:** #DSA 

#### Source:
[YT](https://www.youtube.com/watch?v=1GbPDbHIOv4&list=PLhP5RsB7fhE28lfOcyi9JB31mrBSf4wgL&index=13)

--------------------------------------

#### Explanation about it:

* Generally it stored in key value pair
	* key:value   
		* Key should be in immutable data type
			* String
			* tuple
			* int
		* value will be any type
* we need to use `{ } curly braces` to declare value

```
D ={0:'Gk1', 1:'Gk2'}
fot i in D:  #print only key value
    print(i) 
```

![[Pasted image 20230719192039.png]]

* it's unordered one.

```
D ={0:'Gk1', 1:'Gk2'}
for i in D:
   print(i,D[i])
```

![[Pasted image 20230719192516.png]]


### Functions:

#### Add a element:

```
D = {0:'Gk1',1:'GK2'}
D[2] = 'Gk3'
D[5] = 'Gk5'
print(D)
```

![[Pasted image 20230719192658.png]]

![[Pasted image 20230719192808.png]]

#### Deleing a element:

```
D = {0:'Gk1',1:'GK2'}
D[2] = 'Gk3'
D[5] = 'Gk5'
print(D)
del D[1]
print(D)
```

![[Pasted image 20230719192949.png]]

```
D = {0:'Gk1', 1:'Gk2'}
D[2] = 'Gk3'
print(D)
element = D.pop(0)
print(element)
```

![[Pasted image 20230719204629.png]]


##### Update:

* let consider 2 dictionary
* we can combine two dictionary by using update

```
D = {0:'GK1', 1:'GK2'}
E = {2:'GK3', 3:'GK4'}
D.update(E)
print(D)
```

![[Pasted image 20230719204806.png]]