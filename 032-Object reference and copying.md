---
creation date: 2023-07-27 23:17
modification date: Thursday 27th July 2023 23:17:35
---

**Tags:** #JS 

### Source:
[JS](https://javascript.info/object-copy)

--------------------------------------

### Explanation about it:

* Primitive data type only copy a data to new variable
* In object can reference a value to new variable

```
let user_ref = { name: "John" }
let admin = user_ref;

admin.name = 'Gk1'
user_ref.age = 27

console.log(user_ref)
console.log(admin)
```

![[Pasted image 20230727232600.png]]


##### Cloning and merging, object.assign:

```
let user_org = {
   name: "John",
   age: 30
};

let clone = {}

for (let key in user) {
   clone[key] = user_org[key];
}

clone.name = "Gk1";

console.log(clone)
console.log(user_org)
```