### HTML 
## Table of content

**1. Images**

**2. Color**

**2. Text**

# Images

To add an image into the page you need to use an <img> element. *src* This tells the browser where it can find the image file.
*alt* This provides a text description of the image which describes the image if you cannot see it.

*Example :*

 ```bash
<img src="images/quokka.jpg" alt="A family of
quokka" width="600" height="450" />
 ```

**Where to place image in your html?**

- Before a paragraph : The paragraph starts on a new line after the image.

- Inside the start of a paragraph : The first row of text aligns with the bottom of the image.

- In the middle of a paragraph : The image is placed between the words of the paragraph that it appears in.

 Align horizontally : The align attribute was commonly used to indicate how the other parts of a page should flow around an image.
 
 **Some tips for images in html:**
 
*The <img> element is used to add images to a web page.*

*You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.*

*You should save images at the size you will be using hem on the web page and in the appropriate format.*

*Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.*

# colors

The color property allows you to specify the color of text inside an element.

*The color property allows you to style your html webpage and to specify the color of text inside an element.*

You can specify any color in CSS in one of three ways:

* rgb values : These express colors in terms of how much red, green and blue are used to make it up.

* hex codes : These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign.

* color names : There are 147 predefined color names that are recognized by browsers.

![RGB](https://jsndesign.co.uk/jsn_content/uploads/2017/10/RGB.gif)


**Every color on a computer screen is created by mixing amounts of red, green, and blue.**

### Contrast

*When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.*

Three level of **Contrast** :

- Low Contrast : Text is harder to read when there is low contrast between background and foreground colors. 

- Medium Contrast : For long spans of text, reducing the contrast a little bit improves readability.

- High Contrast : Text is easier to read when there is higher contrast between background and foreground colors.

![CONTRAST](https://learn.g2.com/hs-fs/hubfs/color%20contrast%20on%20color%20wheel.png?width=500&name=color%20contrast%20on%20color%20wheel.png)


### HSL Colors

*CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values.*

What is HSL indicate to ?
 
+ Hue : Hue is the colloquial idea of color.

+ Saturation : Saturation is the amount of gray in a color.

+ Lightness : Lightness is the amount of white (lightness) or black (darkness) in a color.

![hsl](https://miro.medium.com/max/964/1*B2d44wTBqfygLEZ8ZTJXzg.png)

> Color not only brings your site to life, but also helps convey the mood and evokes reactions!

# text

font-family : The font-family property allows you to specify the typeface that should be used for any text inside the element.

font-size : The font-size property enables you to specify a size for the font.

@font-face allows you to use a font, even if it is not installed on the computer of the person browsing.

font-weight : The font-weight property allows you to create bold text.

font-style : If you want to create italic text, you can use the font-style property.

text-decoration : The text-decoration property allows you to specify the following values:none , underline ,overline ,line-through ,blink.



*Example :*

 ```bash
<style type="text/css">
body {
font-family: Georgia, Times, serif;}
font-size: 12px;}
</style>
```
 











 















