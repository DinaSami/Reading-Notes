### JavaScript
## Table of content

**Error Handling & Debugging**

Execution contexts and hoisting : Each time a script enters a new execution context, there are two phases of activity:

1.Prepare : - The new scope is created.   - Variables, functions, and arguments are created.   - The value of the this keyword is determined

2.Execute : - Now it can assign values to variables  - Reference functions and run their code  - Execute statements

In the interpreter, each execution context has its own va ri ables object.It holds the variables, functions, and parameters available within it.Each execution context can also access its parent's v a ri ables object.

If a JavaScript statement generates an error, then it throws an exception.At that point, the interpreter stops and looks for exception-handling code.

Errors objects : Error objects can help you find where your mistakes are and browsers have tools to help you read them.


How to deal with Errors ? Now that you know what an error is and how the browser treats them,there are two things you can do with the errors:

- DEBUG THE SCRIPT TO FIX ERRORS                                 

- HANDLE ERRORS GRACEFULLY

**Debugging** is about deduction: eliminating potential causes of an error.

The JavaScript console will tell you when there is a problem with a script,where to look for the problem, and what kind of issue it seems to be.

*Some notes for DOM tree:*

- Debugging is the process of finding errors. It involves a process of deduction.

- The console helps narrow down the area in which the error is located, so you can try to find the exact error.

- JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.

- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.


