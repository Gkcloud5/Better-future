#### Source:
[W3](https://www.w3schools.com/css/css_image_gallery.asp)


```
<div class="gallery">
  <img src="Images/computer.jpg" alt="" width="600" height="400">
  <div class="desc">Description 1</div>
</div>

<div class="gallery">
  <img src="Images/Studyroom.jpg" width="600" height="400">
  <div class="desc">Description 2</div>
</div>

<div class="gallery">
  <img src="Images/watch.jpg" width="600" height="400">
  <div class="desc">Description 3</div>
</div>

div.gallery {
  margin: 5px;
  border: 1px solid #ccc;
  float:left;
  width:30%;
 }

 div.gallery:hover {
  border: 1px solid #777;
 }

 div.gallery img{
  width: 100%;
  height: 200px;
 }

 div.desc {
  padding: 15px;
  text-align: center
 }
```