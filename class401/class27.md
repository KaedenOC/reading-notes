# useState Hook

[Thinking in React](https://react.dev/learn/thinking-in-react)

Break the UI into a component hierarchy:  Identify the different components needed for the user interface and their organization in a hierarchical structure. Build a static version of the UI: Identify the minimal (but complete) representation of UI state: minimal set of data that the UI needs to render and operate. Add state to the minimal representation: Identify where the state should live: Determine the components that need access to the state and find the closest common ancestor for them.

[State: A Component’s Memory](https://react.dev/learn/state-a-components-memory)

Local variables don't have built-in mechanisms for managing state and updating the UI accordingly. A local variable doesn't provide a way to track changes and trigger updates in the UI. React components need to maintain their state and react to changes to provide a dynamic and responsive user interface.

## useState

The argument to the useState hook in React is the initial state value. It defines the starting value for the state variable. The useState hook returns an array with two elements: the current state value and a function to update the state value.

- To access state from Component B in Component A, you need to lift the state up to a common ancestor component of A and B. This means moving the state and its update functions to a higher-level component that both A and B are descendants of. The state can then be passed down as props to Component A and Component B, allowing them to access and use the state values.

## Additional Resources

[Passing Props to a Component](https://react.dev/learn/passing-props-to-a-component)

[Rendering Lists](https://react.dev/learn/rendering-lists)

[State as Snapshot](https://react.dev/learn/state-as-a-snapshot)

[useState hook](https://react.dev/reference/react/useState)
