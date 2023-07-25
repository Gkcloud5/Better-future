---
creation date: 2023-07-24 22:53
modification date: Monday 24th July 2023 22:53:28
---

**Tags:** #JS 

#### Source:
[JS](https://javascript.info/function-basics)
[NJS](https://www.youtube.com/watch?v=gSDncyuGw0s&pp=ygUdamF2YXNjcmlwdCBmdW5jdGlvbnMgbmFtYXN0YWU%3D)

--------------------------------------

### Explanation about it:

* Functions are the main building blocks of the program.
* They allow the code to be called many times without repetition.

```
function showMessage() {
	console.log("this is shoeMessage value")
}

showMessage();
```

![[Pasted image 20230724225537.png]]


##### Passing argument + Default argument:

```
function passMsg(from, text="default msg") {
  console.log(from, ":", text)
}

passMsg("gokul")
```

![[Pasted image 20230724233521.png]]


### Function Expressions:

* Syntax that we used before is called a Function Declaration

```
function sayHi(){
    console.log("Function executed without call")
}

let func = sayHi;

func()

let test1 = function() {
   console.log("test1")
}
```

![[Pasted image 20230725222007.png]]



### Callback functions:

```
ask(questions, yes, no)
```

```
function ask(question, yes, no) {
	if (confirm(question)) yes()
	else no();
}

function showOk(){
	console.log("pressed yes")
}



ask("do you agree?", showOk, showCancel)
```