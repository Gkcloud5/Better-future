---
creation date: 2023-07-28 00:00
modification date: Friday 28th July 2023 00:00:36
---

**Tags:** #JS 

#### Source:
[this](https://javascript.info/object-methods)

--------------------------------------

### Explanation about it:

* `this` used to access a information stored in the object

```Javascript

let user_this_ex = {
	name: "Gokul",
	age: 30,

	sayHi() {
	  console.log(this.name);
	}
};

user_this_ex.sayHi()
```

![[Pasted image 20230728235022.png]]

```
let user_ex1 = { name: "User_name" };
let admin_ex1 = { name: "Admin_name" };

function sayHiAll() {
	console.log(this.name)
}

user_ex1.f = sayHiAll;
admin_ex1.f = sayHiAll;

user_ex1.f();
admin_ex1.f();

admin_ex1['f']();
```

![[Pasted image 20230728235710.png]]

