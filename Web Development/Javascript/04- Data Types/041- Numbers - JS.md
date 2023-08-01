---
creation date: 2023-08-01 23:47
modification date: Tuesday 1st August 2023 23:47:59
---

**Tags:** #JS 

### Source:
[Num](https://javascript.info/number)

--------------------------------------

### Explanation about it:

* Regular numbers in JS stored in 64-bit format

#### Methods in num:

```
let num1 = 255;
console.log("num to str", num1.toString(), typeof(num1))
num1.toString()
console.log(typeof(num1))
#Rounding
let num2 = 1.234
console.log("round", Math.round(num*100) / 100);
console.log("round2", num2.toFixed(1));

let sum_int = 0.1 + 0.2;
console.log(sum_int.toFixed(2));
console.log(sum_int.toFixed(5));

```

* `isFinite` converts its arguments to a number and returns true, if it's regular number.

```
let imt_num3 =  "45"
console.log(typeof(imt_num3), typeof(isFinite(imt_num3)))
isFinite(imt_num3)
console.log(typeof(imt_num3), imt_num3)
```

![[Pasted image 20230802000243.png]]

![[Pasted image 20230802000403.png]]
