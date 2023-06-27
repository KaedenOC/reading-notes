# Context API

[Choosing the State Structure](https://react.dev/learn/choosing-the-state-structure)

## Principles for structuring state

1. **Group related state** - If you always update two or more state variables at the same time, consider merging them into a single state variable.

2. **Avoid contradictions in state** - When the state is structured in a way that several pieces of state may contradict and “disagree” with each other, you leave room for mistakes. Try to avoid this.

3. **Avoid redundant state** - If you can calculate some information from the component’s props or its existing state variables during rendering, you should not put that information into that component’s state.

4. **Avoid duplication in state** - When the same data is duplicated between multiple state variables, or within nested objects, it is difficult to keep them in sync. Reduce duplication when you can.

5. **Avoid deeply nested state** - Deeply hierarchical state is not very convenient to update. When possible, prefer to structure state in a flat way.

> The goal behind these principles is to make state easy to update without introducing mistakes. Removing redundant and duplicate data from state helps ensure that all its pieces stay in sync.

[Passing State Deeply with Context](https://react.dev/learn/passing-data-deeply-with-context)

## Contexts

- **prop drilling** - Occurs when you need to pass data through multiple layers of components in React. Contexts provide a way to share data across the component tree without the need to explicitly pass it down as props at each level.

- **useContext** - You can try prop drilling before useContext. Prop drilling involves passing the necessary data through component props from the top-level component down to the components that need it.

- **useReducer** - Complements useContext for complex applications. While useContext is primarily used for accessing context values, useReducer provides a way to manage complex state logic within a context.

> useReducer is a hook that allows you to handle state updates through a reducer function, similar to how Redux works. It helps in managing more advanced state management patterns and handling complex actions and state transitions.

## Additional Resources

[Sharing State Between Components](https://react.dev/learn/sharing-state-between-components)

[Preserving and Restting State](https://react.dev/learn/preserving-and-resetting-state)
