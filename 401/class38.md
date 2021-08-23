## Redux - Asynchronous Actions

### Review, Research, and Discussion

##### How granular should your reducers be?

It is difficult to manage states that are deeply nested, so more reducers is better than only a few. Redux gives us combineReducers to let us define more precisely what our initial state will look like.

##### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

It depends on the implementation, it can cause errors if written poorly, or can result in clean firm code if done with caution.

##### Name a strategy for preventing the above?

redux thunk

### Terms

- store : A store holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it.

- combined reducers : The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.

### Preparation Materials

##### async actions 

In Part 5: UI and React, we saw how to use the React-Redux library to let our React components interact with a Redux store, including calling useSelector to read Redux state, calling useDispatch to give us access to the dispatch function, and wrapping our app in a <Provider> component to give those hooks access to the store.

So far, all the data we've worked with has been directly inside of our React+Redux client application. However, most real applications need to work with data from a server, by making HTTP API calls to fetch and save items.

In this section, we'll update our todo app to fetch the todos from an API, and add new todos by saving them to the API.
  
  By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

Earlier, we said that Redux reducers must never contain "side effects". A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like:

- Logging a value to the console
- Saving a file
- Setting an async timer
- Making an AJAX HTTP request
- Modifying some state that exists outside of a function, or mutating arguments to a function
- Generating random numbers or unique random IDs (such as Math.random() or Date.now())

##### redux thunk
  
There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. In this post, you will explore Redux Thunk.

Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.

Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.
  
 Using Redux Thunk in a Sample Application
The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.

Creating a new todo item normally involves first dispatching an action to indicate that a todo item creation as started. Then, if the todo item is successfully created and returned by the external server, dispatching another action with the new todo item. In the case where there’s an error and the todo fails to be saved on the server, an action with the error can be dispatched instead.
  
  








