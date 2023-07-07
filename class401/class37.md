# Redux - Combined Reducers

[Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

## Why Create Multiple Reducers?

- **Modularity**: Multiple reducers allow you to break down your application's state management into smaller, more manageable pieces.

- **Separation of concerns**: Different reducers can focus on different aspects of your application's state.

- **Scalability**: As your application grows in complexity, having multiple reducers makes it easier to add new features or modify existing ones without impacting the entire state management logic.

## Combining Multiple Reducers

Use the **combineReducers** function provided by Redux. This function takes an object as an argument, where each key represents a slice of the state and its corresponding value is the reducer responsible for managing that slice.

**Managing state** as an immutable object is a fundamental principle in Redux. It means that the state should not be directly mutated, but rather a new state object should be created whenever a change occurs.

- Predictability, Pure Functions,

## combineReducers

[Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

**combineReducers** is a utility function in Redux that simplifies the process of creating reducers when writing a Redux application.

- The combineReducers function assembles the new state tree by invoking each individual reducer with a slice of the state and the dispatched action. Each reducer is responsible for managing a specific slice of the state.

- **Initial state** when using combineReducers, you can define the initial state for each individual reducer. Each reducer can have its own initial state, and the combineReducers function will combine them into a single initial state object.

[Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

**Splitting reducing functions** into separate reducers allows you to organize your codebase more effectively. Each reducer can focus on managing a specific part of the state, making it easier to understand, test, and maintain.

- Splitting reducers enables your application to scale and handle increased complexity. By breaking down the state management into smaller, more manageable pieces, you can easily add or modify features without affecting the entire state management logic.

- The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to **createStore**.

- Naming reducers consists of a descriptive name that indicates the portion of the state they manage.

