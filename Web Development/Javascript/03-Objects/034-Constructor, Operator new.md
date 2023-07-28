---
creation date: 2023-07-29 00:01
modification date: Saturday 29th July 2023 00:01:27
---

**Tags:** #JS 

#### Source:
[new](https://javascript.info/constructor-new)

--------------------------------------

### Explanation about it:

* constructor functions and the `new` operator will help to create a similar objects

##### Construction function:

* First letter should be in capital
* executed only with `new` operator

```
function User(name) {
   this.name = name;
   this.isAdmin = false;
}

let user_new_construct = new User("gk")
console.log(user_new_construct)

```

![[Pasted image 20230729000600.png]]


##### Create object with function:

```
let user_func_obj = new function() {
   this.name = "Gk func object";
   this.isAdmin = false;
}

console.log(user_func_obj)
```

![[Pasted image 20230729000929.png]]

