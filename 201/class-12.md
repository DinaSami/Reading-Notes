## JavaScript
### Table of content

**Basic usage**
**Drawing shapes with canvas**
**Applying styles and colors**
**Drawing text**

The <canvas> element differs from an <img> tag in that, like for <video>, <audio>, or <picture> elements, it is easy to define some fallback content,
 to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers.
  
  *Example :*
  ```bash
  <canvas id="tutorial" width="150" height="150">
  </canvas>
  ```
 The <canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.
  In this tutorial, we focus on the 2D rendering context
  
  *Example :*
  ```bash
var canvas = document.getElementById('tutorial');
var ctx = canvas.getContext('2d');
```

Drawing rectangles

Unlike SVG, <canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines).
All other shapes must be created by combining one or more paths.
  
Drawing paths

Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color.
A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

- First, you create the path.

- Then you use drawing commands to draw into the path.

- Once the path has been created, you can stroke or fill the path to render it.

Applying styles and colors

Colors : If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

Transparency : In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes.

Line styles : There are several properties which allow us to style lines.

A lineWidth : This property sets the current line thickness. Values must be positive numbers. By default this value is set to 1.0 units.

Drawing text
The canvas rendering context provides two methods to render text:
- Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

- Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

Styling text  

- font = value 
- textAlign = value
- textBaseline = value
- direction = value


