#### Source:
[TP](https://www.tutorialspoint.com/css/css_tables.htm)

![[Pasted image 20230523233237.png]]


```
table.one { 
 border-collapse: collapse
}

table.two{
  border-collapse: separate;
}

td.a {
  border-style: dotted;
  border-width: 3px;
  border-color: blue;
  padding: 10px;
}
td.b {
  border-style: solid;
  border-width:3px;
  border-color: green;
  padding: 10px
}

<body>
 <table class="one">
	 <caption>Collapse border example</caption>
	 <tr><td class = "a"> Cell A collapse example</td></tr>
	 <tr><td class = "b"> Cell B Collapse Example</td></tr>
</table>
<br />

<table class = "two">
  <caption>Collapse border example 2</caption>
  <tr><td class = "a"> Cell A separate example</td></tr>
  <tr><td class = "b"> Cell B separate example</td><tr>
</table>
</body>
```