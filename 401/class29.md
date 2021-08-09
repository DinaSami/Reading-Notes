## Advanced State with Reducers

### Review, Research, and Discussion

How can we ensure that an effect hook runs only once?

but empty array or nothing so That will ensure the useEffect only runs once.so it works like componentDidMount.

Can useState() update more than one state variable at the same time?

 You could combine the loading state and data state into one state object and then you could do one setState call and there will only be one render. Note: Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely 

Is useState() synchronous?

useState and setState both are asynchronous. ... Even though they are asynchronous, the useState and setState functions do not return promises. Therefore we cannot attach a then handler to it or use async/await to get the updated state values.

### Terms

State Hook : The state is an instance of React Component can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

Component Lifecycle : We are born, grow, and then die. Almost everything follows this cycle in its life, and React components do as well. Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle.

### Preparation Materials

How does useReducer work?
useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX — indeed, it can sometimes be an outright better option.

For those who may be unfamiliar with Redux, we’ll explore this concept a bit further. There are three main building blocks in Redux:

- A store — an immutable object that holds the applications state data
- A reducer — a function that returns some state data, triggered by an action type
- An action — an object that tells the reducer how to change the state. It must contain a type property, and it can contain an optional payload property

```
const initialState = { count: 0 }

const [state, dispatch] = useReducer(reducer, initialState)
```

The reduce() method in JavaScript executes a reducer function on each element of the array an and then returns a single value.
