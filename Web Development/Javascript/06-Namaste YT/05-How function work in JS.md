---
creation date: 2023-08-09 23:05
modification date: Wednesday 9th August 2023 23:05:26
---

**Tags:** #JS

#### Source:
[YT](https://www.youtube.com/watch?v=gSDncyuGw0s&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=5)

--------------------------------------

#### Explanation about it:

```
var x = 1;
a();
b();
console.log(x)

function a() {
    var x = 10;
    console.log(x)
}

function b(){
    var x=100;
    console.log(x)
}
//Output
10
100
1
```