---
creation date: 2023-07-21 22:40
modification date: Friday 21st July 2023 22:40:12
---

**Tags:** #JS 

#### Source:
[JS](https://javascript.info/types)

--------------------------------------

#### Explanation about it:

* A value in JS is always of certain type

##### Number:
```
let n = 123;
n = 12.345
```

##### String:
```
let str = "Hello"
let str2 = 'Single quote'
console.log(str, str2);
```

##### Boolean:
```
let nameField = true;
console.log(nameField);

let isGreate = 4 > 1;
console.log(isGreate)
```

##### Null value:

* `null` value does not belong to any of the types 
```
let age = null;
```

##### undefined:
* meaning of `undefined` is value is not assigned

```
let age=100;
age = undefined;
console.log(age);
```


##### Objects and symbols:

* Objects are used to store collections of data and more complex entities
* symbol type is used to create unique identifiers for objects.

##### typeof operator:

```
typeof undefined
typeof 0
typeof 10n
typeof true
typeof "foo"
typeof Symbol("id")
typeof Matc
typeof null
typeof alert
```

![[Pasted image 20230721232628.png]]
