### Source:
[YT](https://www.youtube.com/watch?v=eBTBG4nda2A&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=13)

### Explanation:

* To do something after particular time delay, we can achieve it by using setTimeout

```
function x() {
 var i = 1;
 setTimeout(function (){
   console.log(i)
 }, 3000);
 console.log("gk check")
}

x()

#Output
gk check
1 //Print after 3sec
```

* JS does not wait and execute setTimeout function, it will move immediately to next statement. 