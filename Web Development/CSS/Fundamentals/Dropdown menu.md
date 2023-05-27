#### Source:
[W3](https://www.w3schools.com/css/css_dropdowns.asp)

```
<div class="dropdown">
  <button class="dropbtn">Dropdown</button>
  <div class="dropdown-content">
      <a href="#">Link 1</a>
      <a href="#">Link 2</a>
      <a href="#">Link 3</a>
  </div>
</div>

<ul class="list_head">
  <li><a>Gk</a></li>
  <li><a>head</a></li>
</ul>

<style>
.dropbtn {
  background-color: green;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}

.dropdown{
  position: relative;
  display: inline-block;
}

.drodown-content a {
 color: black;
 padding: 12px 16px;
 text-decoration: none;
 display: block;
}

.dropdown-content a:hover {
    background-color: yellow;
 }
  
 .dropdown:hover .dropdown-content {
    display: block;
 }
  
 .dropdown:hover .dropbtn {
    background-color: orangered;
 }

 ul.list_head{
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow:hidden;
  background-color: gray;
 }

 .list_head > li {
   float:left;
 }

 .list_head > li a {
  display: inline-block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
 }

 .list_head > li a:hover {
  background-color: red;
 }
</style>

```