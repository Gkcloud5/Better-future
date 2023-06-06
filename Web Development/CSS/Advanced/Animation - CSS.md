#### Source:
[W3](https://www.w3schools.com/css/css3_animations.asp)

#### Explanation about it:

![[Pasted image 20230606232332.png]]

```
<div class="animation">
  <p>Animation</p>
</div>
```


```
.animation {
  width: 100px;
  height: 100px;
  background: red;
  position: relative;
  animation-name: example;
  animation-duration: 10s;
  text-align: center;
  padding: 15px;
  animation-iteration-count: infinite;
}

@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  30%  {background-color:yellow; left:600px; top:0px;}
  50%  {background-color:blue; left:600px; top:500px;}
  75%  {background-color:green; left:0px; top:500px;}
  100% {background-color:red; left:0px; top:0px;}
}
```