#### Source:
[TP](https://www.tutorialspoint.com/css/what_is_css.htm)

* CSS --> Cascading style sheets.
* Css handles a look and feel part of a web page.
* Using CSS, you can control of the text, style fonts, spacing


#### [Syntax](https://www.tutorialspoint.com/css/css_syntax.htm)

* **Selector**: A selector is a html tag at which a style will be applied.
* **Property:** attribute of html tag.
* **Value:** values are assigned to properties, example color, value, ..

![[Pasted image 20230522191041.png]]

```
table{
border : 2px solid blue;
}
```

```
### Universal selector
*{
color: gray;
}
```

```
#class selector
.class {
 color: black;
}
```

```
#selector+attribute
h1.black{
color:black
}
```

```
#child selector
<div class="parent">
  <h2>Parent inside content</h2>
  <p>example paragraph line</p>
</div>

.parent > h2 {
  color: blue;
}
.parent > p {
color: yellow;
}
```