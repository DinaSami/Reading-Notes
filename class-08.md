## CSS

### Table of content

**Layout**

**What is Layout Grids?**

Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page.

![grid](https://xd.adobe.com/ideas/wp-content/uploads/2020/04/css-grid-layout-tutorial.jpg)

**What is CSS Frameworks?**

CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on.

**What is Multiple style sheet?**

Some web page authors split up their CSS style rules into separate style sheets. For example, they might use one style sheet to control the layout and another to control fonts,colors and so on. SO You can include multiple CSS files in one page.

*Example :* 

```bash
<head>
<title>Multiple Style Sheets - Import</title>
<link rel="stylesheet" type="text/css"
href="css/styles.css" />
</head>
```
Multiple Style Sheets (link)

*Example :* 

```bash
<title>Multiple Style Sheets - Link</title>
<link rel="stylesheet" type="text/css"
href="css/site.css" />
<link rel="stylesheet" type="text/css"
href="css/tables.css" />
<link rel="stylesheet" type="text/css"
href="css/typography.css" />
</head>
```

*The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)*
*Grids help create professional and flexible designs.*

(position:static) : In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do notneed a CSS property to indicate that elements should appear in normal flow.

(position:relative) : Relative positioning moves an element in relation to where it would have been in normal flow.

(position:absolute) : When the position property is given a value of absolute,the box is taken out of normal flow and no longer affects the position of other elements on the page.

(position:fixed) : Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.

*Example :* 

```bash
h1 {
position: fixed;
padding: 10px;
}
p {
position: absolute;
width: 450px;}
#p {
position: relative;
top: 10px;}
```





 






