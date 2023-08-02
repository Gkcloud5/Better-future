---
creation date: 2023-08-02 23:36
modification date: Wednesday 2nd August 2023 23:36:35
---

**Tags:** #JS 

### Source:
[JS](https://javascript.info/array)

--------------------------------------
### Explanation about it:

* Array stored ordered collections

```
#Declare

let arr = new Array();
let arr = [];

let fruits = ["Gk1", "Gk2", "Gk3"]
#accessing it
fruits[0]
fruits[1]
fruits[2]

#replace
fruits[1] = 'Gk replace'

#Add a new one
fruits[3] = "Gk new 3"
```

* Array can store elements of any type

```
let any_arr = [ 'Gk1', {name: "gokul"}, true, function() { console.log("inside array function")}]
```


#### Methods:

```Javascript
#push - Add elements to the end
#pop - Takes element from end

let fruits_new = ["Apple", "orange"]
fruits_new.pop() // Apple
fruits_new.push("Guva") //Apple, Guva

#shift - Extract first element and return it
fruits_new.shift() //Guva

#Add element in beginning
fruits_new.unshift("Apple 2", "Orange 2")
```

#### Loops:

```
let arr_loop = ["Gokul1", "Gokul2", "Gokul3"]
for (let i = 0; i < arr_loop.length; i++) {
  console.log(arr_loop[i]);
}
```

```
for (let fruit of arr_loop) {
  console.log(fruit)
}
```

```
let
```
hj