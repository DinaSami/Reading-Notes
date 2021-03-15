### HTML Lists, CSS Boxes, JS Control Flow
## Table of content

**1. LIST**

- Ordered list
- Unordered lists
- Definition lists
- Nested list

**2. BOXES**

- limited width
- limited height
- Border width
- Border style
- border-image
- Rounded corners

**3. Basic JavaScript Instructions**

- Array
- Decisions and Loops
 
# lIST

- Ordered list : The ordered list is created with the <ol> element.
*Each item in the list is placed between an opening <li> tag and a closing </li> tag.

 *Example :*
 ```bash
 <ol>
<li>Chop potatoes into quarters</li>
<li>Mix in the milk mixture</li>
</ol>
```
- Unordered lists : The unordered list is created with the <ul> element.
*Each item in the list is placed between an opening <li> tag and a closing </li> tag.*

 *Example :*
 
 ```bash
 <ul>
<li>1kg King Edward potatoes</li>
<li>100ml milk</li>
</ul>
```

- Definition lists : The definition list is created with the <dl> element.
*<dt> is used to contain the term being defined and <dd> is used to contain the definition.*
*Example :*
  
```bash
<dl>
<dd>A technique by which the scales are removed
from the skin of a fish</dd>
</dl>
```
- Nested list : You can put a second list inside an <li> element to create a sublist or nested list.
*Example :*
  
```bash 
<ul>
<li>Pastries
   <ul>
     <li>Croissant</li>
     <li>Mille-feuille</li>
   </ul>
 </li>
 </ul>
```

# BOXES

- limited width : the *min-width* property specifies the smallest size a box and the *max-width* property indicates the maximum width a box.
*Example :*

```bash 
td.description {
min-width: 450px;
max-width: 650px;}
```

- limited height : to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-height and max-height properties.
*Example :*

```bash
h2 {
color: #0088dd;
border-bottom: 1px solid #0088dd;}
```

- Border width : The border-width property is used to control the width of a border.
*Example :*

```bash
p.one {
border-width: 2px;}
p.two {
border-width: thick;}
```

- Border style : to control the style of a border using the border-style property.
*Example :*

```bash
p.one {border-style: solid;}
p.two {border-style: dotted;}
```

- border-image : This property applies an image to the border of any box.
*Example :*

```bash
p.one {
border-image: url("images/dots.gif")
11 11 11 11 stretch;}
```

- Rounded corners : the ability to create rounded corners on any box.
*Example :*

```bash
p {
border-radius: 10px;}
```
----------------------------------------------------------
# Basic JavaScript Instructions

- Array :  is a special type of variable. It doesn't just store one value; it stores a list of values.
*Example :*

```bash
var colors;
colors ['white', 'black', ' custom '];

var el document.getElementByld('col ors');
el . textContent = col ors[O];
```

- Switch statement : starts with a variable called the switch value.Each case indicates a possible value for this variable and the code that should run if the 
variable matches that value.
*Example :*

```bash
switch (level) {
case 'O ne ':
title= 'Level 1 ' ;
break;

case 'Two':
tit 1 e = ' Level 2 ' ;
break;

default :
title= 'Test';
break;
{
```

- For Loops : A for loop is often used to loop through the items in an array.
*Example :*

```bash
var scores= [24. 32, 17]; 
var arraylength scores .l ength;
var roundNumber = O;
var msg ''; //Message
var i ;
for (i = O; i < arraylength; i++) {
roundNumber = (i + l);
msg += 'Round ' + roundNumber + ' : ';
msg += scores[i] + '<br / >' ;
{
document .getElementByid( ' answer') .i nnerHTML msg;
```

- While Loop : This loop will continue to run for as long as the condition in the parentheses is true.
*Example :*

```bash
var i = l ;
var msg = ' ' ;
while (i < 10) {
msg += i + ' x 5 = ' + (i * 5) + '<br I>';
i++;
{
```

- Do While loop : the statements in the code block come before the condition.
*Example :*

```bash
var i = l;
var msg :'';
do {
msg += i + ' x 5 = ' + (i * 5) + '<br I>' ;s
i++;
} wh il e ( i < 1) ;
document .getEl ementByl d(' answer').innerHTML = msg;
{
```


