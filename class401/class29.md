# Advanced State With Reducers

- [Extracting State Logic into a Reducer](https://react.dev/learn/extracting-state-logic-into-a-reducer)

## Benefits of Reducers

- **Centralized State Management**: A reducer helps in centralizing and organizing the logic for managing complex state within a component or a state container.

- **Predictable State Updates**: Follow a strict pattern where the current state and an action are passed to produce a new state. This pattern ensures that state updates are predictable and easy to reason about, making it simpler to track changes and debug issues.

- **Improved Code Readability**: You can encapsulate the logic for updating state in a concise and reusable manner by using a reducer.

In the context of a reducer, **actions** are plain JavaScript objects that represent an intention or an event that triggers a state update. They typically contain a type property to identify the type of action and may include additional payload data. When an action is dispatched, the reducer examines its type and performs the necessary state transformation based on the action's information.

**Immutability**: Setting state directly using useState replaces the entire state value, while using a reducer and actions encourages immutability. Reducers typically create a new state object by applying modifications to the previous state, ensuring that the original state remains unchanged.

**Explicit State Transitions**: With a reducer, the state transitions are explicitly defined and determined by the action type and payload.

The **reduce** function, often referred to as a "fold," combines elements of a list into a single value by applying a specified operation repeatedly. Similarly, useReduce in the context of React hooks implies reducing a sequence of actions into a new state value.

## Switching From useState to useReducer

- If your **component's state management becomes more complex**, involving multiple related values and intricate update rules, using a reducer can help in handling the complexity more efficiently.

- When you have **multiple components** that need access to the same state or when you need to synchronize state updates across different parts of your application, using a reducer allows you to manage the shared state more effectively.

- If you **require middleware functionality**, such as logging, API calls, or other side effects, during state updates, using a reducer can provide a more structured approach.

> The decision to switch to useReducer should be based on the complexity and specific needs of your application. For simpler state management scenarios, useState may be sufficient and more straightforward.

## Additional Resources

[useReducer hook](https://react.dev/reference/react/useReducer)

[Keeping Components Pure](https://react.dev/learn/keeping-components-pure)

[Queueing a Series of State Updates](https://react.dev/learn/queueing-a-series-of-state-updates)
