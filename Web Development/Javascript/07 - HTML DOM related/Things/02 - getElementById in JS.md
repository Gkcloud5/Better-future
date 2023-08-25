
[JT](https://www.javascripttutorial.net/javascript-dom/javascript-getelementbyid/)

`document.getElementById()`

* It returns an Element object that represents an HTML element with an `id` that matches a specified string.

```
#syntax
const element = document.getElementId(id);
```

```js
<p id="message">A paragraph get element id example</p>
<p id="getExam"></p>

<script>
let p_element = document.getElementById('message').innerHTML
document.getElementById('getExam').innerHTML='content added from script'+ p_element
</script>
```

![[Pasted image 20230826013125.png]]
