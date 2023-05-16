#### Source:
[Structure](https://web.dev/learn/html/document-structure/)


### Add to every HTML document:

#### <!DOCTYPE html>

* It is instruction that informs browser or HTML parser about the version of HTML being used in the document.

#### `<html>`

*  It is root element for an HTML document. it is the parent of `<head>` and `<body>`

```
<!DOCTYPE html>  
<html lang="en-US">  
<head>  
</head>  
<body>  
</body>  
</html>
```

#### Required components inside the `<head>`:

* Document metadata
* Document title
* Character set
* Viewport
* Description
* base URL
* stylesheet links
* icons

##### Character encoding:

```
<meta charset="utf-8" />
```

* For to support wide range of character.

##### Document Title:

```
<title>Machine Learning Workshop</title>
```

##### ViewPort metadata:

```
<meta name="viewport" content="width=device-width" />
<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=1" />
```

* It helpful for site responsiveness.

#### Outline:

```
<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="utf-8" />  
<title>Machine Learning Workshop</title>  
<meta name="viewport" content="width=device-width" />  
</head>  
<body>  
  
</body>  
</html>
```

#### Adding a CSS in head:

* we have a 3 ways to add css in html

```
<style>  
@import "styles.css" layer(firstLayer);  
</style>
```

```
<style>  
:root {  
--theme-color: #226DAA;  
}  
</style>
```


```
<style contenteditable style="display: block; font-family: monospace; white-space: pre;">  
head { display: block; }  
head * { display: none; }  
:root {  
--theme-color: #226DAA;  
}  
</style>

```

##### Favicon:

```
<link rel="icon" sizes="16x16 32x32 48x48" type="image/png" href="/images/mlwicon.png" />
```


##### Script:

```
<script>  
document.getElementById('switch').addEventListener('click', function() {  
document.body.classList.toggle('black');  
});  
</script>
```

* It used to include a javascript.