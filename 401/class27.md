## Hook

### Review, Research, and Discussion

How does React differ from vanilla JS/HTML/CSS?

Basically, with React, we can manage to keep the UI and the state synchronized with each other. In Vanilla JS, if you have to change the state, you would need to update the UI. One small mistake and your UI could be out of sync with your data. Code organization and re-

What is the primary difference between a function component and a class component?

 and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components
 
### Terms
 
Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI


A child component is a more specific part inside a parent component. Example would be a parent component being a PERSON. ARMS and LEGS are child components of it

### Preparation Materials

What is a Hook? A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

When would I use a Hook? If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component.

```
1:  import React, { useState } from 'react';
 2:
 3:  function Example() {
 4:    const [count, setCount] = useState(0);
 5:
 6:    return (
 7:      <div>
 8:        <p>You clicked {count} times</p>
 9:        <button onClick={() => setCount(count + 1)}>
10:         Click me
11:        </button>
12:      </div>
13:    );
14:  }
```
useState is a Hook.We call it inside a function component to add some local state to it. React will preserve this state between re-renders. useState returns a pair: the current state value and a function that lets you update it. You can call this function from an event handler or somewhere else. It’s similar to this.setState in a class, except it doesn’t merge the old and new state together.

Hooks API Reference
Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

- Basic Hooks

useState
useEffect
useContext

- Additional Hooks

useReducer
useCallback
useMemo
useRef
useImperativeHandle
useLayoutEffect
useDebugValue


