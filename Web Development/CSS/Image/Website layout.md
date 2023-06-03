#### Source:
[w3](https://www.w3schools.com/css/css_website_layout.asp)


![[Pasted image 20230601234540.png]]


#### Header:

```
<!-- Layout -->
<div class="header_top">
  <h1>Header</h1>
</div>


<div class="topnav">
  <a href="">Link1</a>
  <a href="">Link2</a>
  <a href="">Link3</a>
</div>

<div class="row">
  <div class="column">
     <h2>Column 1</h2>
     <p>Column 1 content</p>
  </div>
  <div class="column">
    <h2>Column 2</h2>
    <p>Column 1 content</p>
 </div>
 <div class="column">
  <h2>Column 3</h2>
  <p>Column 1 content</p>
</div>

<div class="footer">
  <h1>footer</h1>
</div>
```

```
.header_top {
  margin-top: 20px;
  background-color: #cccaca;
  padding: 20px;
  text-align: center;
}

.topnav{
  overflow: hidden;
  background-color: #272525;
}

.topnav a {
  float: left;
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

.topnav a:hover {
  background-color: aliceblue;
  color: #272525;
}

.column {
  float: left;
  width: 33.33%;
  padding: 15px;
}
.row::after {
  content: "";
  display:table;
  clear:both;
}

@media screen and (max-width:600px) {
  .column {
    width: 100%;
  }
}

.footer {
  display: grid;
  background-color: #cccaca;
  padding: 20px;
  text-align: center;
}
```

