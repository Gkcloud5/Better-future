---
creation date: 2023-06-06 22:59
modification date: Tuesday 6th June 2023 22:59:07
tag: 
---

#### Source:
[LJ](https://www.w3schools.com/css/css3_transitions.asp)

--------------------------------------

#### Explanation about it:

```
<div class="transistion-move">
     <p>Transistion</p>
</div>
```

```
div.transistion-move {
   width:100px;
   height:100px;
   background: red;
   transition: width 2s, transform 2s;
   transition-timing-function: linear; 
   
}

div.transistion-move:hover {
   width: 300px;
   transform: rotate(180deg)
}
```

