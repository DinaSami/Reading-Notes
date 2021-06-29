## Data Modeling

### Name 3 advantages to test driven development
Anticipating bugs, refactoring code (easier to identify where bugs are), tests serve as documentation.

### In what case would you need to use beforeEach() or afterEach() in a test suite
When you have to do something repeatedly for many tests for example, initialize a function.

### What is the downside of test driven development
Maintaining tests.  Can be seen as "slowing down" development, though, I would think the long range benefits would outweigh the short term. 

### What's the primary difference between ES6 Classes and Constructor/Prototype Classes
ES6 classes is like a container that holds the constructor and the methods associated with your instantiated object.  

###Why REST?
The WRRC is inherently stateless. Using REST creates states -  which is like creating knowledge of actions that happened before the client made the request and what will or should happen after the response is sent back to the client.  REST is used when you are talking to your API (vs. CRUD which is used when you are talking to a database)

### Define

*Functional Programming* is based more on calculations and returning a mathemetical value. "What to solve" versus "how to solve". This is also supported in Javascript. 

*Object-Oriented Programming (OOP)* can be used to describe Javascript.  Objects are a data structure that hold properties that liken to "real world objects" which have properties and methods.

*class* is like a constructor on steroids.  In addition to instantiating an object based on properties included in the constructor within the class, this syntax also allows for methods to be connected to instantiated objects.

*super* allows you to invoke functions from the parent object. This makes medium sense with calling static methods, but less sense when using while extending classes.

*this* the contextual this is in reference to an instantiated object.

*TDD* test driven development is a way of developing code to pass tests first. In TDD before any implementation code is written at all, a test is created and then code is written to pass that test and THEN it is developed and refactored.

*Continuous Integration* helps to integrate changes into main code base.  It is a workflow strategy that helps ensure that everyone's local changes integrate and merge conflicts are reduced.  The server builds and tests the code to determine if it works and if it can be merged with the main branch.

*REST* representational state transfer.

*Data Model* represents parts of data and defines that way that data interacts with each other and with the structure they are placed in.

### Term

- Middleware
- Request Object
- Response Object
- Application Middleware
- Routing Middleware
- Test Driven Development
- Behavioral Testing

### Preview

[sql v nosql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
<br>
[nosql v sql](thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
<br>
[nosql modeling techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)

**Got Clarity**
-SQL v. noSQL databases
**Want to Learn More**
- super and extends
- more testing methods that come with jest 
**Most Excited to Try**
working with a database with meaningful data

### SQL vs NoSQL Database Differences Explained with few Example DB

Most of you are already familiar with SQL database, and have a good knowledge on either MySQL, Oracle, or other SQL databases. In the last several years, NoSQL database is getting widely adopted to solve various business problems.

### NOSQLdata modeling techniques

NoSQL databases are often compared by various non-functional criteria, such as scalability, performance, and consistency. This aspect of NoSQL is well-studied both in practice and theory because specific non-functional properties are often the main justification for NoSQL usage and fundamental results on distributed systems like the CAP theorem apply well to NoSQL systems.  At the same time, NoSQL data modeling is not so well studied and lacks the systematic theory found in relational databases. In this article I provide a short comparison of NoSQL system families from the data modeling point of view and digest several common modeling techniques.



