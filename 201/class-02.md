### HTML & CSS & JavaScript
## Table of content

**1. TEXT**

- Headings and paragraphs

- Bold, italic, emphasis

- Structural and semantic markup

**2. Introducing CSS**

- What CSS does?
- How CSS works?
- Rules, properties, and values

**3. Basic JavaScript Instructions**

- What is script?
- what is a variable?
- what is array?
- 
**3. Decisions and Loops**
- DECISIONS
- Loops
- operators
# TEXT

- Headings and paragraphs

HTML has six "levels" of headings, called h1 , h2 ...etc.

*Example :*

```bash
   <h1>Table of Content</h1>
```
To create a paragraph, surround the words that make up the paragraph with an opening <p> tag and closing </p> tag.

```bash
   <p>This is a paraghraph</p>
```

- Bold, italic, emphasis

Bold :  By enclosing words in the tags <b> and **</b>** we can make characters appear bold.
Italics : By enclosing words in the tags **<i>** and **</i>** we can make characters appear italic.

- Structural and semantic markup

*Some examples for semantic markup:*

The <sup> element is used to contain characters that should be superscript such as the suffixes.

The <sub> element is used to contain characters that should be subscript.

The <hr> element To create a break between themes — such as a change of topic in a book.

The <em> element indicates emphasis that subtly changes the meaning of a sentence.

The <blockquote> element is used for longer quotes that take up an entire paragraph.

The <address> element has quite a specific use: to contain contact details for the author of the page.

------------------------------------
# Introducing CSS

- What CSS does?
- 
CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

- How CSS works?

CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed.

- Rules, properties, and values
- 
A CSS rule contains two parts: a selector and a declaration.

```bash
p {
font-family: Arial;}
```

CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon.

```bash
h1, h2, h3 {
font-family: Arial;
color: yellow;}
```
We can use external CSS using The <link> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page.

```bash
<link href="css/styles.css" type="text/css" rel="stylesheet" />
```
Also we can use internal CSS using The <style> element should use the type attribute to indicate that the styles are specified in CSS.

```bash
<style type="text/css">
body {
font-family: arial;
background-color: rgb(185,179,175);}
h1 {
color: rgb(255,255,255);}
</style>
```
------------------------------------
#  Basic JavaScript Instructions

- What is script?
 
A script is a series of instructions that a computer can follow one-by-one.Each individual instruction or step is known as a statement.

- what is a variable?

A script will have to **temporarily store** the bits of information it needs to do its job. It can store this data in variables.
 
```bash
quality = 3;
x = 2;
```
- Data type in JV
 
JavaScript distinguishes between numbers, strings, and true or false values known as Booleans.

1.Numeric : The numeric data type handles numbers.
2.String : The strings data type consists of letters and other characters.
3.Boolean : Boolean data types can have one of two va lues: true or false.

- what is array?

An array is a special type of variable. It doesn't just store one value; it stores a list of values.
 
You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array).

- what is Expressions?

An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions.

```bash
var color = 'beige';

var area = 3 * 2;
```

#  Decisions and Loops
 
- DECISIONS : Using the results of evaluations, you can decide which path your script should go down.

- LOOPS : There are also many occasions where you will want to perform the same set of steps repeatedly.

These are Loops:
 
 * For : if you need to run code a specific number of times , use a **FOR** LOOP.

 * While : if you do not know how many times the code should run , you can use **WHILE** loop.

 * Do While : this loop is very similar to the **while** loop.


- operators

- Logical operators
  
  *Comparison operators usually return single values of true or false. Logical operators allow you to compare the results of more than one comparison.*
  
  These are Logical operators:
  
 * Logical And ( && )

* Logical Or ( )

* Logical Not ( ! )


- comparison operators
- 
- These are comparison operators:

* Equal to ( == )

* Not equal to ( !=)

* Strict equal to ( === )

* Strict not equal to ( !==)

* Greater than ( > )

* Less than ( < )

* Greater than or equal to ( >= )

* Less than or equal to ( <= )









