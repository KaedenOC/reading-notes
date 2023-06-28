# Context API - Behaviors

[Scaling Up with Reducer and Context](https://react.dev/learn/scaling-up-with-reducer-and-context)

- By combining the **useReducer** and **useContext** hooks, you can simplify state management and make it more scalable. The useReducer hook in React allows you to manage state by defining a reducer function that takes in the current state and an action, and returns the new state. This helps in organizing and centralizing state-related logic. By dispatching actions to the reducer, you can modify the state in a predictable and controlled manner.

- The **useContext** hook provides a way to access a context that you have created using the createContext function. Context allows you to share data across the component tree without having to pass props explicitly at each level. When you combine useContext with useReducer, you can create a centralized state management system that can be accessed and modified by any component in your application.

- To use them together: first define a context using createContext, then create a provider component that wraps your application or a specific portion of it. The provider component uses the useReducer hook to manage the state and provides the state and dispatch function to the context value. Any component that needs to access or modify the state can use useContext to consume the state and dispatch actions to the reducer.