---
creation date: 2023-06-15 18:05
modification date: Thursday 15th June 2023 18:05:37
---

**Tags:** #css #button

#### Source:
[LJ](https://www.w3schools.com/css/css3_buttons.asp)

--------------------------------------

#### Explanation about it:

```
<button class="button" style="vertical-align:middle"><span>Hover </span></button>
```


```
.button {
  display: inline-block;
  border-radius: 4px;
  background-color: #f4511e;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 200px;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}
```

