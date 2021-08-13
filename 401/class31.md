## Context API

### Review, Research, and Discussion

- Describe use cases useState() vs useReducer()?

useReducer() is a method from the React Hooks API, similar to useState but gives you more control to manage the state. It takes a reducer function and initial state as arguments and returns the state and dispatch method

useReducer() is an alternative to useState() which gives you more control over the state management and can make testing easier. All the cases can be done with useState() method, so in conclusion, use the method that you are comfortable with, and it is easier to understand for you and colleagues.

- Why do custom hooks need the use prefix?

Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.

- What do custom hooks usually do?

Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

- Using any list of custom hooks, research and name one that you think will be useful in your applications?

(useScript) --> useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.

- Describe how a hook that fetches API data might work?

The App component shows a list of items (hits = Hacker News articles). The state and state update function come from the state hook called useState that is responsible to manage the local state for the data that we are going to fetch for the App component. The initial state is an empty list of hits in an object that represents the data. No one is setting any state for this data yet.

We are going to use axios to fetch data, but it is up to you to use another data fetching library or the native fetch API of the browser. If you haven't installed axios yet, you can do so by on the command line with npm install axios. Then implement your effect hook for the data fetching

### Terms

reducer: A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently

### Preparation Materials

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

When to Use Context?

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component:

```
class App extends React.Component {
  render() {
    return <Toolbar theme="dark" />;
  }
}

function Toolbar(props) {
  // The Toolbar component must take an extra "theme" prop
  // and pass it to the ThemedButton. This can become painful
  // if every single button in the app needs to know the theme
  // because it would have to be passed through all components.
  return (
    <div>
      <ThemedButton theme={props.theme} />
    </div>
  );
}

class ThemedButton extends React.Component {
  render() {
    return <Button theme={this.props.theme} />;
  }
}
```

Before You Use Context

Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This default value can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue.

It might feel redundant to pass down the user and avatarSize props through many levels if in the end only the Avatar component really needs it. It’s also annoying that whenever the Avatar component needs more props from the top, you have to add them at all the intermediate levels too.








