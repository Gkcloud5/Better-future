---
creation date: 2023-07-10 22:22
modification date: Monday 10th July 2023 22:22:27
---

**Tags:** #bootstrap 

#### Source:
[Forms](https://www.w3schools.com/bootstrap4/bootstrap_forms.asp)

--------------------------------------

#### Explanation about it:

```
<div class="container">
    <h2>Form validation</h2>
    <form action="/form_action" class="was-validated">
        <div class="form-group">
          <label for="uname">User name</label>
          <input type="text" class="form-control" id="uname" placeholder="Enter username" name="uname" required>
          <div class="valid-feedback">Valid.</div>
          <div class="invalid-feedback">Please fill out this field</div>
        </div>
        <div class="form-group">
           <label for="pwd">Password:</label>
           <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd" required>
           <div class="valid-feedback">Valid.</div>
            <div class="invalid-feedback">Please fill out this field.</div>
        </div>
        <div class="form-group form-check">
            <label class="form-check-label">
            <input class="form-check-input" type="checkbox" name="remember" required> I agree on blabla.>
            <div class="valid-feedback">Valid.</div>
        <div class="invalid-feedback">Check this checkbox to continue.</div>
         </label>
        </div>
        <button type="submit" class="btn btn-primary">Submit</button>
    </form>
</div>
```

![[Pasted image 20230710223713.png]]
