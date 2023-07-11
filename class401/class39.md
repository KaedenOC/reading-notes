# Redux - Additional Topics

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/introduction/getting-started)

## Redux Toolkit

- Library built on top of Redux that aims to simplify the development experience and address some common concerns associated with using Redux. It provides a set of utilities and abstractions that help streamline Redux setup, reduce boilerplate code, and improve developer productivity.

- Boilerplate Reduction, Immutable State Updates, Built-in Redux DevTools Integration, and Opinionated Approach.

`configureStore()` - function provided by redux toolkit to create a Redux store with sensible defaults and configurations. It combines several commonly used Redux store setup steps, such as applying middleware, enabling the Redux DevTools extension, and setting up additional enhancers. It simplifies the store creation process and reduces the amount of setup code required.

`createSlice()` - function is used to define a "slice" in Redux Toolkit. A slice represents a logical portion of your application state and includes the corresponding reducer, actions, and selectors.

- takes an initial state, a set of reducer functions, and an optional name for the slice.

- generates action creators and action types based on the provided reducers, reducing the amount of manual setup required.

- can be added to the Redux store using `configureStore()`.

Ex:

``` javascript
import { createSlice } from '@reduxjs/toolkit';

const counterSlice = createSlice({
  name: 'counter',
  initialState: 0,
  reducers: {
    increment(state) {
      return state + 1;
    },
    decrement(state) {
      return state - 1;
    },
  },
});

export const { increment, decrement } = counterSlice.actions;
export default counterSlice.reducer;
```

## MobX

[MobX](https://mobx.js.org/getting-started.html)

- **State management library** for JavaScript applications. It enables you to create reactive applications by automatically tracking and updating state changes in a transparent manner.

- Provides a simple and intuitive API that allows you to define observable state, track dependencies, and reactively update your user interface.

- MobX ensures consistency in state updates through its core concept of observables and reactions.

- **Observables** - core building blocks. Represent values that can be observed and automatically tracked for changes.

- **Reactions** - mechanisms by which MobX tracks dependencies and triggers updates when the observed state changes.

- Define Observable State, Create Computed Values, Build Components, React to State Changes

[Tutorial](https://redux-toolkit.js.org/tutorials/overview)

- MobX takes care of tracking dependencies, updating the user interface efficiently, and ensuring consistency in the state throughout your application.

- MobX enables a reactive programming model where your user interface reacts automatically to changes in state.

## Additional Resources

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

[HookState](https://hookstate.js.org/)
