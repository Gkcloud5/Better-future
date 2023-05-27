#### Source:
[TP](https://www.tutorialspoint.com/css/css_media_types.htm)

#### Media rule:

```
@media print{
 body {
  font-size: 10pt
  }
}

@media screen {
  body {
   font-size: 12pt
   }
}

@media screen, print {
  body {
    line-height: 1.2
   }
}

@media screen and (min-width: 480px) {
   body {
     background-color: pink;
   }
}
```