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