## Hook

### Review, Research, and Discussion

Why do we not need more .html pages in a multi-page React app?

A React app consists of a single HTML file index.html. The views are coded in JSX format as components.Because React deals with components instead of pages.

If we wanted a component to show up on every page, where would we put it and why?

Inside the <BrowserRouter />, outside a <Route /> because we consider this component as static component so there is no need to be inside <Route/> .

What does routing do with the components that were rendered when a new route is requested?

Routing is the ability to move between different parts of an application when a user enters a URL or clicks an element (link, button, icon, image etc) within the application.

What does props.children contain?

props.children to pass children elements directly into their output.

How do useState() and this.setState() differ?

we useState() to set states inside hooks ,but this.setState() to set states inside classes.

### Terms

State Hook : The state is an instance of React Component can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

Mounting and Un-Mounting : The mount command mounts a storage device or filesystem, making it accessible and attaching it to an existing directory structure. The umount command "unmounts" a mounted filesystem, informing the system to complete any pending read or write operations, and safely detaching it.

### Preparation Materials

Using the Effect Hook
Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

There are two common kinds of side effects in React components: those that don’t require cleanup, and those that do. Let’s look at this distinction in more detail.

Effects Without Cleanup

Sometimes, we want to run some additional code after React has updated the DOM. Network requests, manual DOM mutations, and logging are common examples of effects that don’t require a cleanup. We say that because we can run them and immediately forget about them. Let’s compare how classes and Hooks let us express such side effects.

Example Using Classes
In React class components, the render method itself shouldn’t cause side effects. It would be too early — we typically want to perform our effects after React has updated the DOM.

This is why in React classes, we put side effects into componentDidMount and componentDidUpdate. Coming back to our example, here is a React counter class component that updates the document title right after React makes changes to the DOM:

```
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }

  componentDidMount() {
    document.title = `You clicked ${this.state.count} times`;
  }
  componentDidUpdate() {
    document.title = `You clicked ${this.state.count} times`;
  }

  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          Click me
        </button>
      </div>
    );
  }
}
```
This is because in many cases we want to perform the same side effect regardless of whether the component just mounted, or if it has been updated. Conceptually, we want it to happen after every render — but React class components don’t have a method like this. We could extract a separate method but we would still have to call it in two places.
