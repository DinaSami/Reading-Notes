## Redux - Additional Topics

### Review, Research, and Discussion

##### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

##### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

 Redux provides you with an elegant approach to manage the state of a JavaScript application. Its infrastructure is based on functional foundations and lets you easily build testable code. However, the flow of Redux tasks to manage the state of an application is completely synchronous: dispatching an action immediately generates the chain of calls to middlewares and reducers to carry out the state transition.
 
 
### Terms

middleware : is software that enables one or more kinds of communication or connectivity between two or more applications or application components in a distributed network. ... There are many types of middleware. Some, such as message 

thunk : is a subroutine used to inject a calculation into another subroutine. Thunks are primarily used to delay a calculation until its result is needed, or to insert operations at the beginning or end of the other subroutine.


### Preparation Materials

The Redux core docs  contains the primary tutorials for learning Redux, including how to use Redux Toolkit and React-Redux together.

MobX is unopinionated and allows you to manage your application state outside of any UI framework. This makes your code decoupled, portable, and above all, easily testable.

a simple, scalable and battle tested state management solution. This tutorial will teach you all the important concepts of MobX in ten minutes. MobX is a standalone library, but most people are using it with React and this tutorial focuses on that combination.

MobX makes state management simple again by addressing the root issue: it makes it impossible to produce an inconsistent state. The strategy to achieve that is simple: Make sure that everything that can be derived from the application state, will be derived. Automatically.






















