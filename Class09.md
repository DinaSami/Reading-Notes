# Concepts of Functional Programming with JS

- Functional Programming - a style of building app structure that focuses more on the mathematical functions and less on changing state and mutable items.

- Pure functions - zero side effects and must return the same result as the given args.No external object given to the function. We want to set args. directly, not use global scoped variables.
         
        - Random number generators make a function impure
        - If we have a function that has a += 1 counter within, this is impure since it's result is changing. Set the function to always return a value + one and set a counter outside of the function will make it pure as the pure function will always return value + 1.
        - Pure functions are isolated, stable, sonsistent, etc.

- Benefits - Easier to test. Easy to memorize your functions.

- Review - Immutable means that something cannot be changed. The work around is to create a new object.

- Recursion - divide and conquer. Separating your problem into smaller pieces. Let your function work in the same way always, form the variables to fit the mold of the function. Keeping your variable unchanged.

- Referential tranperency - if the functions always returns the same result for the same given input. Easy to memorize your functions.

        pure function + immutable (variable, object, data) = referential transperency

- Functions as first class entities - treated as a value, used for data.

        - function is referred to from the constants and vars.
        - pass as param to other funcs.
        - returns as result from outside funcs.

- Higher-order functions - takes one to multiple funcs. as args or the result is the return of a function. filter, map, and reduce.

- filter() - expects a true or false value to see if whether or not the element is included in the result. 

        - imperative - creates a new empty array.
        - declaritive - less breakable and fewer moving parts.
        - (GREAT EXAMPLES IN DOCS.)


- map() - applies a function to it's elements, returns a new set of values that are returned. (SEE EXAMPLES)

- reduce() - take in data, return it consolidated or combining it.


# Fun with Refactoring 


- Reactoring your code so it appears and works more solidly is huge, but you can also do too much refactoring to the point where it hinders the functionality of your script.

- hash function - this function maps and sets under the hood.
