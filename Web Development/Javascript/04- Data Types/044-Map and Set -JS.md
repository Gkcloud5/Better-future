---
creation date: 2023-08-03 23:31
modification date: Thursday 3rd August 2023 23:31:04
---

**Tags:** #JS 

#### Source:
[JS](https://javascript.info/map-set)

--------------------------------------

### Explanation about it:

* Map is a collection of keyed data items
	* Just like an object

![[Pasted image 20230803235355.png]]

```
let map_test = new Map();

map_test.set('1', 'str1');
map_test.set(1,'num1');

console.log(map_test)
```

![[Pasted image 20230803235924.png]]


##### Iteration in map:

```
let receipMap = new Map([
 ['Carrot', 500],
 ['Tomato', 250],
 ['Onion', 150]
]);

for (let vegetable of receipMap.keys()){
	console.log(vegetable)
}

for (let amount of receipMap.values()) {
	console.log(amount)
}

for (let entryVal of receipMap) {
	console.log(entryVal)
}
```

![[Pasted image 20230804000502.png]]


### About set:

* Special type collection - set of values without keys.

![[Pasted image 20230804000728.png]]

```
let set_test = new Set()

let gk1 = { name: "gk1" }
let gk2 = { name: "gk2" }
let gk3 = { name: "gk3" }

set.add
```