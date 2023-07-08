---
creation date: 2023-07-08 22:27
modification date: Saturday 8th July 2023 22:27:03
---

**Tags:** #bootstrap 

#### Source:
[Collapse](https://www.w3schools.com/bootstrap4/bootstrap_collapse.asp)

--------------------------------------

#### Explanation about it:

```
<div class="container">
   <h1>Accordion example</h1>
   <div id="accordion">
       <div class="card">
            <div class="card-header">
                <a class="card-link" data-toggle="collapse" href="#collapseOne">
                Collapsible 1</a>
            </div>
            <div id="collapseOne" class="collapse show" data-parent="#accordion">
               <div class="card-body">
                  Testin accordion contents
                </div>
            </div>
       </div>
       <div class="card">
      <div class="card-header">
        <a class="collapsed card-link" data-toggle="collapse" href="#collapseTwo">
        Collapsible Group Item #2
      </a>
      </div>
      <div id="collapseTwo" class="collapse" data-parent="#accordion">
        <div class="card-body">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        </div>
      </div>
    </div>
   </div>
</div>
```

![[Pasted image 20230708224350.png]]

