---
creation date: 2023-07-24 22:37
modification date: Monday 24th July 2023 22:37:12
---

**Tags:** #JS 

#### Source:
[JS](https://javascript.info/logical-operators)

--------------------------------------

#### Explanation about it:

##### ||(OR):

```
result = a || b;
console.log( true ||  true)
console.log( false || true)
console.log( true || false)
console.log( false || fale)
```

![[Pasted image 20230724223953.png]]

* Any one is true then condition is true

##### && (AND)

```
console.log(true && true)
console.log(false && true)
```

* Only true when both true

![[Pasted image 20230724224245.png]]

##### !(NOT)

```
console.log( !true )
console.log( !0 )
```

![[Pasted image 20230724224412.png]]


##### ??:

```
console.log(height ?? 100) 
let height = 0;
console.log(height ?? 100)
```