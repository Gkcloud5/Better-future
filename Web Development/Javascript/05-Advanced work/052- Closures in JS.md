---
creation date: 2023-08-07 23:10
modification date: Monday 7th August 2023 23:10:59
---

**Tags:** #JS

#### Source:
[Closures](https://www.youtube.com/watch?v=qikxEIxsXco)

--------------------------------------

### Explanation about it:

```
function x(){
  var a=7;
  function y(){
	  console.log(a);
  }
  y();
}
x();
```

- Above example, 7 is a closure.
- 