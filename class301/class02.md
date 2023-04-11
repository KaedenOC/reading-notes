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

