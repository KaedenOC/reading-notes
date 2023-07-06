# Application State With Redux

[Dan Abramov Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)

## Redux

Redux is a predictable state management library for JavaScript applications, primarily used with frameworks like React. It provides a centralized and predictable way to manage the state of an application, making it easier to develop complex applications with consistent and maintainable state behavior.

- The first principle of Redux is the **single source of truth**. It means that the state of your entire application is stored in a single JavaScript object called the "store." This makes it easier to manage and track changes in your application's state.

- **store** - an object that holds the application state and provides a way to dispatch actions, which are plain JavaScript objects describing what happened in your application.

- **reducers** - pure functions that specify how the application's state should change in response to an action. They take the current state and an action as input and return a new state.

When using the **createStore** function in Redux, it provides several methods to interact with the store.

- **getState**(): This method is used to retrieve the current state of the Redux store. It returns the current state object.

- **dispatch(action)**: This method is used to dispatch an action to the Redux store. It triggers the execution of the corresponding reducer function and updates the state based on the action.

- **subscribe(listener)**: This method allows you to register a listener function that will be called whenever the state in the store is changed. It provides a way to react to state changes and update the user interface accordingly.

## combineReducer()

- utility function provided by Redux that allows you to combine multiple reducers into a single reducer function. In Redux, as your application grows, you might have multiple reducers to handle different parts of the state. combineReducers() takes these individual reducers and creates a new reducer that can handle the entire state.

## Additional Resources

[worlds easiest guide to redux](https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)

[testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

[Redux Docs](https://redux.js.org/)
