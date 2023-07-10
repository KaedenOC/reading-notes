# Redux - Asynchronous Actions

[async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)

## Redux Middleware

- Used to handle asynchronous actions in Redux applications. It sits between the dispatching of an action and the time it reaches the reducers, allowing us to intercept, modify, or delay actions as needed. Middleware provides a way to add additional functionality to Redux, such as handling asynchronous operations, logging, routing, or managing side effects.

**Redux Async Data Flow Diagram** - dispatch action, middleware intercepts it before it reaches the reducers. Middleware performs asynchronous operations(like API requests), and then dispatches actions with the requested data. Then these actions flow through the reducers, updates state, and triggers re-rendering of the UI with the new data.

- In Redux, we accommodate async operations by using middleware specifically designed for handling asynchronous actions, such as Redux Thunk or Redux Saga. These middleware provide a way to write action creators that can return functions instead of plain action objects. These functions can perform asynchronous operations and dispatch regular actions when the operations are complete. Middleware intercepts these functions, invokes them, and handles the async flow.

- Manage async logic seamlessly within the Redux data flow.

## Redux Thunk

[thunk middleware](https://github.com/reduxjs/redux-thunk)

- We want to use **Redux Thunk** when we want to write action creators that perform asynchronous operations, such as making API calls, before dispatching actions.

- We can use this middleware by returning a function instead of a plain action object from your action creators.

- Redux Thunk middleware allows you to write action creators that return a function instead of an action.

- When an action creator returns a function in Redux Thunk middleware, the function is intercepted and invoked by the middleware. Inside the function, you have access to the dispatch function, allowing you to dispatch actions. The dispatched actions flow through the middleware pipeline, reaching the reducers for state updates.
