## Context API - Behaviors

### Review, Research, and Discussion

What are some good use cases for using the Context API for global state?

 use the Context API to store the data that does not change frequently. If the requirements of your project meet that criteria, you’re good to go. If you’re not sure, let’s dig deeper into this and find out why the frequency of updates matters so much.
 
How can you best test context?

The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).


### Terms

context : ontext is related to objects. It refers to the object to which a function belongs. When you use the JavaScript “this” keyword, it refers to the object to which function belongs. 

useContext() : "useContext" hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.

static context : Static context defines items that are needed to prepare executables, items such as the names and types of external variables and functions that will be available at run time as well as compilation modes like backwards compatibility, math mode, and so on. These items do 


### Preparation Materials













