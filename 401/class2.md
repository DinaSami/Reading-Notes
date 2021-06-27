##  Express

### Difference between PUT and PATCH

PUT and PATCH are both HTTP request methods.  The PUT method updates a resource in its entirety making it so that all future requests to that resource reflect changes updated thru a PUT method. The PATCH method includes information for only partially modifying the resource.  This means that when you make that request again it will not necessarily reflect the changes of the previous PATCH mehod. (Can someone confirm if I am undestanding this correctly?)


**Provide 3 links to services or tools that allow you to 'mock' an API for development like json-server**
Postman, Nock, Mockserver.

**Compare and contrast Swagger and APIDoc.js.  Which HTTP status codes should be sent with each type of (un)successful API call?**
Swagger website and can be thought of an alternative to Postman.  When you create and make a request in the swagger site, you will see the console.logs in your terminal when that request is executed.

APIdoc.js is a node module that "creates a documentation from API descriptions in your source".  Though, I am not totally sure what that means.  But, what I am guessing is that this is an alternative to simulating a production environment for developers without running code in the browser.

**Compare and contrast SOAP and ReST**
REST stands for representational state transfer and is pretty much what we have been doing with the GET, PUT, POST, DELETE HTTP request verbs.  It is a flexible way to access web services in contrast to SOAP (Simple Object Access Protocol) which delivers messages using XML (extensible mark up language) and does not require the use of HTTP which REST does.

**Define Terms: Web Server, Express, Routing, WRRC**
*Web Server* is made up of hardware and software which together "uses HTTP and other protocols to respond to client requests made thru the web.  Main job is to display website content thru storing, processing and delivering webpages to users". https://whatis.techtarget.com/definition/Web-server

*Express* is a JavaScript framework/tool that help us handle HTTP requests.  It is a JS framework for building APIs and servers.  It is an API tool on teh backend. 

*Routing* is essentially creating paths and associated them with functions so that when a particular route is hit it invokes its respective function. 

*WRRC* the web request response cycle explains the flow of how the client makes a request to the server and the server's response to the client with the information requested.

**Skim Prep Materials**
*What 3 things had you heard about previously and now have better clarity on?*
- Test Driven Development

*Which 3 things are you hoping to learn more about in the upcoming lecture/demo*
- middleware
- CRUD

*What are you most excited about trying to implement or see how it works?*
- Testing and using curl in the terminal to test server. 
