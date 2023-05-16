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
