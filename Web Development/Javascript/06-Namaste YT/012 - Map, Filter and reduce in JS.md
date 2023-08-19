### Source:
[YT](https://www.youtube.com/watch?v=zdp0zrpKzIE&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=22)

### Explanation:

#### Map:

* Map function generally used to transform an array.
	* Change values inside array

```
const arr = [5,1,2,3,4]

function double(x) {
  return x*2;
}

const output = arr.map(double)

console.log(output)
```


### Filter:
* Used to filter a value inside an array

```
const arr = [5,1,2,3,4]

function isOdd(x) {
   return x % 2;
}

const output = arr.filter(isOdd)

#Output
[5,1,3]
```


### Reduce:
* It used place where take all elements in array and get single value from array.
* reduce(accumulator, current)
	* Accumulator --> Accumulate value that get from every iteration

```
//Sum or max
const arr = [5,1,2,3,4]

const output = arr.reduce(function (acc, curr) {

})
```