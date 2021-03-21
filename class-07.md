### HTML & JavaScript
## Table of content

**Tables**

**Functions, Methods, and Objects**

# Tables

A Tables : represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.

The <table> element is used to create a table. The contents of the table are written out row by row.
   
It is followed by one or more <td> elements (one for each cell in that row).
  
At the end of each cell you use a closing </td> tag.

*Example :*

```bash
<table>
<tr>
<td>15</td>
<td>15</td>
<td>30</td>
</tr>
</table>
```
 
The <th> element is used just like the <td> element but its purpose is to represent the heading for either a column or a row.

The rowspan attribute can be used on a <th> or <td> element to indicate how many rows a cell should span down the table.

The headings of the table should sit inside the <thead> element.
  
The body should sit inside the <tbody> element.The footer belongs inside the <tfoot> element.
  
The border attribute was used on both the <table> and <td> elements to indicate the width of the border in pixels.
  
*Example :*

```bash
<table border="2" bgcolor="#efefef">
<tr>
<th width="150"></th>
<th>Withdrawn</th>
<th>Credit</th>
<th width="150" bgcolor="#cccccc">Balance</th>
</tr>
```

# Functions, Methods, and Objects

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
 
Document Object Model

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

*Some notes for Functions, Methods, and Objects:*

- Functions allow you to group a set of related statements together that represent a single task.

- Functions can take parameters (informatiorJ required to do their job) and may return a value.

- An object is a series of variables and functions that represent something from the world around you.

- In an object, variables are known as properties of the object; functions are known as methods of the object.

- Web browsers implement objects that represent both the browser window and the document loaded into the browser window.

- JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.

- Arrays and objects can be used to create complex data sets (and both can contain the other).

















