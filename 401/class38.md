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

- combined reducers : 

### Preparation Materials












