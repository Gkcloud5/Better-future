---
creation date: 2023-08-02 00:04
modification date: Wednesday 2nd August 2023 00:04:32
---

**Tags:** #JS 

#### Source:
[Str](https://javascript.info/string)

--------------------------------------

### Explanation about it:

* In JS textual data is stored as strings.

##### Quotes:

```
let single = 'single-quoted'
let double = "Double-quoted"

let backticks = `backticks`
```

```
function sum_str(a,b) {
  return a+b
}

console.log(sum_str(1, 2))
```


##### length:

```
#str.length

let str_value = "gokul length"
console.log(str_value.length)
```

![[Pasted image 20230802230728.png]]


```
#Accessing character
console.log(str_value[0]) //g
str_value.at(-1) //h
```

* Strings are immutable

```
'Gokul'.toUpperCase() //GOKUL
'Gokul'.toLowerCase() //gokul
.includes()
.startsWith()
.endsWith()
.slice(0,1)
.substring(2,6)

```


