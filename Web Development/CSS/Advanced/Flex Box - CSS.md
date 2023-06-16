---
creation date: 2023-06-16 17:05
modification date: Friday 16th June 2023 17:05:10
---

**Tags:** #CSS #Flexbox

#### Source:
[YT](https://www.youtube.com/watch?v=phWxA89Dy94)

--------------------------------------

#### Explanation about it:

##### Flex-Container:

```
.flex-container{
display: flex;
}
```

![[Pasted image 20230616171105.png]]


```
<div class="flex-container">
   <div class="item">Item1</div>
   <div class="item">Item2</div>
   <div class="item">Item3</div>
   <div class="item">Item4</div>
   <div class="item">Item1</div>
   <div class="item">Item2</div>
   <div class="item">Item3</div>
   <div class="item">Item4</div>
</div>
```

```
.flex-container{
  border: 2px solid brown;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  /* justify-content: center; */
  justify-content: space-around;
  justify-content: space-between;
  align-items: center;
  align-content: space-between;
  align-content: space-around;
}

.item{
  border: 2px solid green;
  background-color: #cccaca;
  color: #f4511e;
  width: 200px;
}
```


![[Pasted image 20230616172629.png]]
