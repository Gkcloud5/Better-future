#### Source:
[W3](https://www.w3schools.com/css/css_form.asp)

```
<h2>Responsive Form</h2>

<div class="container">
  <form action="linuxjourney.com">

    <div class="row">
       <div class="col-25">
           <label for="fname">First Name</label>
       </div>
       <div class="col-75">
          <input type="text" id="fname" name="firstname" placeholder="Your first name">
       </div>
    </div>

    <div class="row">
      <div class="col-25">
         <label for="lname">Last Name</label>
      </div>
      <div class="col-75">
         <input type="text" id="lname" name="lastname" placeholder="Enter Last name">
      </div>
    </div>

    <div class="row">
      <div class="col-25">
        <label for="country">Country</label>
      </div>
      <div class="col-75">
         <select id="country" name="country">
            <option value="india">India</option>
            <option value="Canada">Canada</option>
            <option value="USA">USA</option>
         </select>
      </div>
    </div>

    <div class="row">
      <input type="submit" value="Submit">
    </div>

  </form>
</div>
```


```
<!-- CSS -->
/* Form*/

* {
  box-sizing: border-box;
}

input[type=text], select {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}

input[type=submit] {
  background-color: #04AA6D;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
  margin-top: 15px;
}

input[type=submit]:hover {
  background-color: #45a049;
 
}

.container {
  border-radius: 5px;
  background-color:#f2f2f2 ;
  padding: 20px;
}

.col-25{
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

.row::after {
  content: "";
  display: table;
  clear: both;
}

@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
```

