---
creation date: 2023-07-26 00:18
modification date: Wednesday 26th July 2023 00:18:09
---

**Tags:** #JS 

#### Source:
[Object](https://javascript.info/object)

--------------------------------------

### Explanation about it:

* JS have 8 datatypes
	* Seven of them are called "primitive", because their values contain only a single thing
		* It will be string or number
	* Objects are used to store keyed collections of various data and more complex entities.
* Object created with figure baskets `{..}`
	* key:value
		* key is a string
		* value can be anything

```
let user = new Object(); //Object constructor syntax
let user = {}; //Literal syntax
```


![[Pasted image 20230727223650.png]]


##### Literals and properties:

```
let user3 = {
  name: "John",
  age: 30
};

console.log(user3.name)
console.log(user3.age)
```

![[Pasted image 20230727223923.png]]


##### Add a value inside object:

```
user3.isAdmin = true;

console.log(user3)
```

![[Pasted image 20230727224413.png]]


##### Delete value in object:

```
delete user3.age
console.log(user3)
```

![[Pasted image 20230727224451.png]]


##### Computed properties:

```
let fruit = "apple"
let bag = {
    [fruit]: 5,
};

console.log(bag)
console.log( bag.apple );
```

![[Pasted image 20230727230121.png]]

* we can assign key value dynamically by using square brackets

##### `in` operator:

```
"key" in object
```

```
let user = { name: "John", age:30 };

console.log( "age" in user );
console.log( "blabla" in user );
```

![[Pasted image 20230727231132.png]]


##### `for..in` loop:

```
for (key in object) {
}

let user_for = {
  name: "John",
  age: 30,
  isAdmin:true
}

for (let key in user_for) {
 console.log(key)
 console.log(user_for[key])
}
```

![[Pasted image 20230727231540.png]]


