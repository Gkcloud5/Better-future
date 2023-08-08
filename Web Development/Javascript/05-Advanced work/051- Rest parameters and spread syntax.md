---
creation date: 2023-08-04 00:34
modification date: Friday 4th August 2023 00:34:59
---

**Tags:** #JS 

#### Source:
[JS](https://javascript.info/recursion)

--------------------------------------

### Explanation about it:

#### Rest Parameters:
* A function can be called with any number of arguments, no matter how it is defined.

```
function sumAll(...args) {
  let sum = 0;
  for (let arg of args) sum += arg;
  return sum;
}

console.log(sumAll(1));
console.log(sumAll(1,2));
console.log(sumAll(1,2,3));
```

![[Pasted image 20230807225317.png]]


##### Spread syntax:

* Get a element from array

```
let arr = [3, 5, 1];
console.log(Math.max(...arr));
```

![[Pasted image 20230807230110.png]]

