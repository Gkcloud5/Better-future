#### Source:
[W3](https://www.w3schools.com/css/css3_2dtransforms.asp)


* `transform` is a property name.
* 2D transformation methods:
	* translate()
	* rotate()
	* scaleX()
	* scaleY()
	* scale()
	* skewX()
	* skewY()
	* skew()
	* matrix()

```
<div class="transistion">
  <div class="transistion_rotate">
     <h1>Rotate() Method</h1>
     <p>rotate method rotates an element clockwise or counter-clockwise</p>
   </div>
</div>
```

```
.transistion {
  margin-top: 20px;
  width:300px;
  height:100px;
  background-color:yellow;
  border:1px solid black;
}

.transistion_rotate{
  transform: rotate(30deg);
  background-color:rgb(123, 224, 154);
}
```

