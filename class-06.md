### JavaScript
## Table of content

**Object Literals**

**Document Object Model**

# Object Literals

What is Object? Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

*Example :*

```bash
var hotel = {
name: 'Quay',
rooms : 40,
booked: 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
 ```
 
# Document Object Model

Wha is The Dom Tree ? it is a model of a web page , as a browser loads a web page , it creates a model of that page. The model is called a DOM tree , and it is stored in the browsers memory .is consists of four main types of nodes.

*Example :*

```bash
<html>
<body>
<di v id="page">
<hl id="header">List</hl>
<h2>Buy groceries</h2>
<ul>
<li id="one" class="hot"><em>fresh</em> figs</li>
<li id="two" class="hot">pine nuts</l i>
<l i id="three" class="hot">honey</l i>
<l i id="four">balsamic vinegar</l i>
</ ul>
<script src="js/l i st. js "></scri pt>
</ div>
</ body>
</ html>
```

How to work with the DOM tree?

Accessing and updating the DOM tree involves two steps:

1.Locate the node that represents the element you want to workwith.

2.Use its text content, child elements and attributes.

How to access elements? DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes.

Selecting elements using ID attributes :

This method has one parameter :
- The value of the id attribute on
- The element you want to select.

*Example :*

```bash
II Select the element and store it in a variable.
var el = document.getElementByid('one');
II Change the value of the class attribute.
el.className ='cool ' ;
```

Selecting elements using CLASS attributes :

The method has one parameter:
- The class name which is given : in quotes within the parentheses after the method name.
*Example :*

```bash
var elements = document .getEl ementsByClassName('hot');
if (e lements .l ength> 2) {
var el = elements[2];
el.className = 'cool';
}
```

Selecting elements using TAG NAME attributes :

The element name is specified as a parameter, so it is placed inside the parentheses and is contained by quote marks.
*Example :*

```bash
var elements = document.getElementsByTagName('li '); 
if (elements.length> O) {
var el = elements[O];
el.className = 'cool';
}
```
*Some notes for DOM tree:*

- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes: document nodes,element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one node, it will always return a Nadel i st.
- From an element node, you can access and update its content using properties such as textContent and i nnerHTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and child elements that are siblings of each other.
- In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree .
