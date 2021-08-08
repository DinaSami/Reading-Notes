## Component Based UI

### Review, Research, and Discussion

Name 5 Javascript UI Frameworks (other than React)?

- Bootstrap
- Vue
- Ruby on Rails
- Svelte
- Angular

What’s the difference between a framework and a library?

A framework determines the architecture of an app. A library contributes, when called, within that architecture. 

<hr>

### Terms

Rendering: displays application in browser.

Templates: "isolate UI interaction client-side with minimal http requests to the server".Improve speed of rendering. 

State: Lines of code within the render(), within an ES6 class, that are in curly braces and have a reference "this". State is a property of the class constructor.  This constructor takes in props and calls super.
<hr>

### Preparation Materials

Why JSX?
React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Embedding Expressions in JSX
In the example below, we declare a variable called name and then use it inside JSX by wrapping it in curly braces:

```
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;

ReactDOM.render(
  element,
  document.getElementById('root')
);
```
Rendering Elements
Elements are the smallest building blocks of React apps.

An element describes what you want to see on the screen:

```
const element = <h1>Hello, world</h1>;
```
Updating the Rendered Element
React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.


