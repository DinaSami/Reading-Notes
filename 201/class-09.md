## html & JavaScript
### Table of content

**Forms**
**Lists, Tables & Forms**
**Events**

#### Forms
How Forms work A user fills in a form and then presses a button to submit the information to the server.

Form controls live inside a <form> element. This element should always carry the action attribute and will usually have a method and id attribute too.
  
Every <form> element requires an action attribute. Its valueis the URL for the page on the server that will receive the information in the form when it is submitted.
*Example :*
  
 ```bash
<form action="http://www.example.com/subscribe.php"
method="get">
<p>This is where the form controls will appear.
</p>
</form>
```
The <input> element is used to create several different formcontrols. The value of the type attribute determines what kind of input they will be creating.
*Example :*

 ```bash
<form action="http://www.example.com/login.php">
<p>Username:
<input type="text" name="username" size="15"
maxlength="30" />
</p>
</form>
```
*Types of inputs :*

- type="radio" Radio : buttons allow users to pick just one of a number of options.
 
- type="checkbox" :  Checkboxes allow users to select (and unselect) one or more options in answer to a question.
 
- A drop down list  box :  (also known as a select box) allows users to select one option from a drop down list.
 
- multiple options : You can allow users to select multiple options from this list by adding the multiple attribute with a value of multiple.

- type="submit" : The submit button is used to send a form to the server.


### Lists, Tables & Forms

The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker).

You can specify an image to act as a bullet point using the list-style-image property.

*Example :*

 ```bash
ul {
list-style-image: url("images/star.png");}

ol {
list-style-type: lower-roman;}
```

*some propereties to style Tables:*

- width to set the width of the table.

- padding to set the space between the border of each table cell and its content.

- text-transform to convert the content of the table headers to uppercase.

- text-align to align the writing to the left of some table cells and to the right of the others.

- :hover to highlight a table row when a user's mouse goes over it.

*Some notes for Lists, Tables & Forms:*

- List markers can be given different appearances using the list-style-type and list-style image properties.

- Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.

- Forms are easier to use if the form controls are vertically aligned using CSS.

- Forms benefit from styles that make them feel more interactive.

### Events

When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code.Together these steps are known as event handling.

1.Select the element node(s) you want the script to respond to.

2.Indicate which event on the selected node(s) will trigger the response.

3.State the code you want to run when the event occurs.

When an event occurs, the event object tells you information about the event, and the element it happened upon.

Event Delegation : Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.

User interface events : User interface CUI) events occur as a result of interaction with the browser window rather than the HTML page contained within it, e.g., a page having loaded or the browser window being resized.


































