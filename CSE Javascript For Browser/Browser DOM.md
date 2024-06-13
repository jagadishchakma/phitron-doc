

--- start-multi-column: ID_2zxk
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Finding HTML Elements</p>

---
- ### document.getElementById()

<pre>






</pre>


---
- ### document.getElementsByClassname()

<pre>











</pre>
---
- ### document.getElementsByTagName()

<pre>










</pre>

---
- ### document.querySelector(css selector)
- ### document.querySelectorAll(css selector)

<pre>








</pre>

---
- ### element.children
- ### element.clossest(css selector)
- ### element.nextElementSibling
- ### element.previousElementSibling

<pre>















</pre>

---
# <p align="center">Finding HTML Objects</p>
---

- ### document.anchors
- ### document.body
- ### document.cookie
- ### document.domain
- ### document.forms
- ### document.head
- ### document.images
- ### document.title
- ### document.URL

---
# <p align="center">Getting or Changing HTML Elements</p>

---

- ### element.innerHTML ==getting content with html==
- or
- ### element.innerContent ==getting only code content ignore html==
- or
- ### element.innerText ==getting only browser display content==

- ### element.innerHTML = new html content ==changing==
- ### element.attribute_name = new value ==add or change attribute===
- or
- ### element.setAttribute(attribute_name,value) ==add or change attribute==


<pre>



</pre>
---

- ### element.style.property = new style ==changing style==

<pre>






</pre>

---
# <p align="center">Adding and Deleting Elements</p>
---

- ### document.createElement(element)
- ### element.remove()
- ### element.removeChild(child_element)
- ### element.append(newElement)
- ### element.appendChild(newElement)
- ### element.replaceChild(new,old)


--- column-break ---

# <p align="center">Examples</p>

---
```javascript
//html
<h1 id="title">Heading one</h1>

//js
let title = document.getElementById("title");
console.log(title)
```

---
```javascript
//html
<ul>
	<li class="list-item"> Item One </li>
	<li class="list-item"> Item two </li>
	<li class="list-item"> Item three </li>
	<li class="list-item"> Item four </li>
</ul>

//js
let lists = document.getElementsByClassName("list-item");
console.log(lists)
```

---
```javascript
//html
<h1>Heading One</h1>
<p>Paragraph </p>
<h1><Heading One/h1>
<p>Paragraph</p>


//js
let tags = document.getElementsByTagName("h1");
console.log(tags);
```

---
```javascript
//html
<h1>heading one</h1>
<h1>heading one one</h1>

//js
let tag = document.querySelector("h1");
console.log(tag);

let tags = document.querySelectorAll("h1");
console.log(tags);
```

---
```javascript
//html
<div>
    <p>paragraph</p>
     <ul>
         <li>item one</li>
         <li>item two</li>
         <li>item three</li>
         <li>item four</li>
     </ul>
    <h1>helo world</h1>
</div>

//js
let element = document.querySelector("ul")

console.log(element.children)
console.log(element.closest("div"))
console.log(element.nextElementSibling)
console.log(element.previousElementSibling)
```

---
# <p align="center">Examples</p>
---

```javascript
//Returns all <a> elements that have a name attribute
//Returns the <body> element
//Returns the document's cookie
//Returns the domain name of the document server
//Returns all <form> elements
//Returns the <head> element
//Returns all <img> elements
//Returns the <title> element
//Returns the complete URL of the document
```

---
# <p align="center">Examples</p>

---
```javascript
//html
<ul>
	<li class="list-item"> Item One </li>
	<li class="list-item"> Item two </li>
	<li class="list-item"> Item three </li>
	<li class="list-item"> Item four </li>
</ul>

//js
let element = document.getElementsByClassName("list-item")[0];
console.log(element.innerHTML);

element.innerHTML = "Changing Item";
```

---
```javascript
//html
<h1>Heading one</h1>

//js
let tag = document.getElementsByTagName("h1")[0];
tag.style.backgroundColor = "red";
```

---
# <p align="center">Example</p>
---


```javascript
//create an HTML element
//remove an html element
//remove an html child element
//add an html element
//add an html child element
// replace old html element via new html element
```



--- end-multi-column

