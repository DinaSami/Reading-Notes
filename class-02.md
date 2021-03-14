### HTML & CSS
## Table of content

**1. TEXT**

- Headings and paragraphs

- Bold, italic, emphasis

- Structural and semantic markup

**2. Introducing CSS**

- What CSS does?
- How CSS works?
- Rules, properties, and values

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

