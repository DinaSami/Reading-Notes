##  Express


### 3 real world cases where you'd want to change the request with custom  middleware
1. Login authentication
2. Logging data to get user insights
3. Error handling

### True or false: the route handler is middleware
False.  A route handler can make requests and get responses without middleware.  Middleware can be added to route handlers or other functions to alter/shape requests/responses.

### In what ways can a middleware function end the process and send data to the  browser?
Thru the use of the next().  Or, 500 errors.  If an error is triggered, it will end the WRRC and send the 500 message to the user thru the broswer.

### At what point in the request lifecycle can you "inject" middleware
Middleware can be injected to shape the way the request object.

### What can cause express to error with "Request headers send twice, cannot start a second response
This happens when you have more than one response being sent to your client. This happened to me when I had, erroneously, included a response statement in my validator function AND my app.get route.

### DEFINE
*Middleware* is code that can accompanies a request so as to modify the request object. 
*Request Object* is the data retrieved from the server.
*Response Object* is the data that is sent to the browser.
*Application Middleware* is associated with "app.use()" and is applied to the entire application.
*Test Driven Development* is development that is built created based upon its ability to pass a unit test.
*Behavioral Testing* is a way of describing the app in testing units or bench marks that can be communicated between an engineering team and other stakeholders, like a UX design team and is constructed more or less in sentences.

### Prep Materials
[Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
[Using Express Routing](https://expressjs.com/en/guide/routing.html)
[Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

### Better clarity?
- Super class calls (I think)
- Routes

### Hoping to learn more
- what would be the use cases of using a named v. unnamed class?
 
### Excited to try
- express.Router

### Term

-Middleware
-Request Object
-Response Object
-Application Middleware
-Routing Middleware
-Test Driven Development
-Behavioral Testing


### Classes

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.

A class expression is another way to define a class. Class expressions can be named or unnamed. The name given to a named class expression is local to the class's body. (it can be retrieved through the class's (not an instance's) name property, though).

Constructor

The constructor method is a special method for creating and initializing an object created with a class. There can only be one special method with the name "constructor" in a class. A SyntaxError will be thrown if the class contains more than one occurrence of a constructor method.

### Routing

Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).

```
var express = require('express')
var app = express()

// respond with "hello world" when a GET request is made to the homepage
app.get('/', function (req, res) {
  res.send('hello world')
})
```
Route methods

A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

The following code is an example of routes that are defined for the GET and the POST methods to the root of the app.

```
// GET method route
app.get('/', function (req, res) {
  res.send('GET request to the homepage')
})

// POST method route
app.post('/', function (req, res) {
  res.send('POST request to the homepage')
})
```

