# Component Lifecycle / useEffect Hook

[useEffect hook](https://react.dev/reference/react/useEffect#reference)

The `useEffect` hook is used to handle side effects in functional components. Any code that needs to be executed outside the scope of the component's render method, such as fetching data from an API, subscribing to events, manipulating the DOM, or setting up timers.

- It takes two arguments: a function that represents the effect's logic and an optional array of dependencies. Logic function is executed after the component has rendered and whenever any of the dependencies change.

- If you’re not trying to synchronize with some external system, you probably don’t need an Effect.

- The return value from the effect's logic function is important when cleanup is required. If the effect's logic function returns a cleanup function, React will invoke that function before running the effect again or unmounting the component. This cleanup function is used to clean up any resources, event listeners, or subscriptions created by the effect.

- returns `undefined`.

## Additional Resources

[Responding to Events](https://react.dev/learn/responding-to-events)

[Conditional Rendering](https://react.dev/learn/conditional-rendering)

[Updating Arrays in State](https://react.dev/learn/updating-arrays-in-state)

[Updating Objects in State](https://react.dev/learn/updating-objects-in-state)