#### Source:
[Overview](https://web.dev/learn/html/overview/)


#### About HTML:

* Hyper Text Markup Language, is the backbone of the web, providing the content, as well as the structure of the content, that you see displayed in your web browser.
* [Dom](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
	* Document object model
	* It connects web pages to scripts or programming languages by representing the structure of a document such as HTML.
	* It is programming interface for web documents. it represents the page so that programs can change the document structure, style and content.

![[Pasted image 20230510192128.png]]

* CSS provide the look and feel or presentation layer of the page.
* JavaScript is behavior's layer, often


### Elements:

* HTML consists of a series of elements, which use to enclose.

![[Pasted image 20230511233452.png]]


#### Types of elements:

1. Replaced
2. Non-replaced

##### Non-replaced elements:

* Non-replaced elements have opining and closing tag that surround them.
* paragraph, header tag are example for it

##### Replaced and void elements:

* Replaced elements are replaced by objects.
* `<img>, <input>` are example for replaced elements

```
<input type="range">
<img src="name.img" alt="img tag">
```


### Attributes:

* Attributes provide information about the element

![[Pasted image 20230511234118.png]]

**Example:**

```
<img src="name.img" alt="img tag" ismpa />
```

In above example we have 3 attributes, `src, alt, ismap`.


### Appearance of elements:

* Default appearance of semantic elements is set by user-agent stylesheets.

```
<h1>This header has both <strong>strong</strong> and <em>emphasized</em> content</h1>
```

### Elements, attributes and JavaScript:

* DOM is the data representation of the structure and content of the HTML document.
* As the browser parses HTML, it creates a javascript object every element and section of text encountered. these objects are called nodes
	* Element nodes
	* Text nodes
