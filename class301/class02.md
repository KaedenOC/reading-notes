# State and Props

[React Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

## Component Lifecycle Events

React lets you define components as classes or functions. *Lifecycle Events* are the methods that you can use on components.

### Phases of Component Lifecycle

- **Mounting** - *The first thing to happen in the lifecycle of React* When an instance of a component is being created and inserted into the DOM.

- **Updating** - Anytime a component is updated or state changes then it is rerendered.

- **Unmounting** - The final phase of the lifecycle if called when a component is being removed from the DOM.

Put the following things in the order that they happen: *constructor*, *render*, *componentDidMount*, *React updates*, and *componentWillUnmount*.

- **componentDidMount** - this event occurs when this component has been loaded to the screen (added to the DOM). It is often used for side effects such as data fetching, subscriptions, or other setup that needs to happen after the component is visible on the screen.


### Diagram

Based off the diagram, I believe that 'render' happens first.

## React State and Props

**props** - Props can be used to pass a wide variety of data types. Some are: 

- Primitive data types

- Objects

- Arrays

- Functions

- JSX elements

**state** - Refers to an object that holds the data that a component needs to manage and track over time.  State is mutable and can be changed over time, and when the state of a component changes, React will automatically re-render the component to reflect the updated state.

### Difference Between State and Props

- *state* is used inside the component and inside only, and *props* is used outside the component and is being passed in.

- *state* will be used to manage component specific data that can change. Components utilizing state will maintain their own data and trigger re renders to reflect updated data to the UI.

> user input, fetched data, or UI interactions.

### Additional Resources:

[React Docs - State and Lifecycle](https://legacy.reactjs.org/docs/state-and-lifecycle.html)

[React Docs - handling events](https://legacy.reactjs.org/docs/handling-events.html)

[React Tutorial through ‘Developer Tools’](https://react.dev/learn/tutorial-tic-tac-toe)

[React Bootstrap Documentation](https://react-bootstrap.github.io/)

[Boootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)

[Bootstrap Shuffle - a class “sandbox”](https://bootstrapshuffle.com/classes)

[Netlify](https://www.netlify.com/)