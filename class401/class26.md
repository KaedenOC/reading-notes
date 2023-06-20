# Component Based UI

[React Quick Start](https://react.dev/learn)

## Building Blocks Of A React App

- **Components** - React is a component-based library, which means that the UI is broken down into reusable, self-contained components. Components can be either functional or class-based, and they encapsulate the logic and rendering of a specific part of the UI.

- **State** - represents the data that can change in a React component. It is managed internally by the component and can be updated using the setState method.

- **Props** - inputs that are passed to a component from its parent component. They allow data and functionality to flow downwards from parent components to child components.

- **JSX** - allows you to write HTML-like code within JavaScript. It provides a way to define the structure and content of React components. JSX makes it easier to describe the UI hierarchy and renders elements efficiently.

## HTML Element Vs React Component

- standard tags provided by the **HTML** language, such as `<div>, <span>, <h1>,` etc. HTML elements describe the structure and content of a web page and are primarily used for static rendering.

- **React Components** are JavaScript functions or classes that return JSX elements. React components are reusable, composable, and allow dynamic rendering based on state and props. They encapsulate functionality and can be rendered to create HTML elements in the DOM.

## JSX

- **JavaScript XML** - syntax extension for JavaScript that allows you to write HTML-like code within JavaScript. It provides a concise and familiar way to define the structure and content of React components.

- *Readability* - resembles HTML, making it easier for developers to understand and visualize the structure of the UI.

- *Component composition* - compose components hierarchically, similar to nesting HTML tags.

- *Integration* - embed JavaScript expressions directly within the markup, making it convenient to use variables, perform calculations, or execute functions dynamically.

- **Embedding JSX** - `const name = "John";
const element = <h1>Hello, {name}!</h1>;`

- the name variable is embedded within the JSX using curly braces.

## Iteration and Conditional Logic

- **Iteration** - Methods to iterate over an array and dynamically generate JSX elements. This allows you to render lists of items efficiently.

- **Conditional** - Render JSX based on certain conditions. (ternary/ifs/etc). Allows you to show or hide components or elements based on the state or props.

React responds to a user's inputs through event handling. You can attach event listeners to React components, such as onClick, onChange, etc., and define corresponding event handler functions. When a user interacts with a component, such as clicking a button or typing in an input field, the event is triggered, and the associated event handler function is executed.

## useState

- Indicates that a React component manages data with a Hook.

- **Hooks** - Functions that allow functional components to have state and other React features. The useState hook specifically is used to declare state variables in functional components.

## Sharing Data

- **lifting state up** - Share data between two React components.  If the two components have a parent-child relationship, you can lift the shared data to a common ancestor component and pass it down as **props** to the child components. This way, both components can access and update the shared data through props.

[Render and Commit](https://react.dev/learn/render-and-commit)

## 3 Steps To Refreshing A React UI

- **Trigger(Initial Render)** - When the app starts the initial render is triggered.

- **Commit** - React uses a process called reconciliation to efficiently update only the parts of the DOM that have changed.

- **Reconciliation** - Aims to minimize the number of actual DOM manipulations, optimizing performance.

To trigger updates to a component after the **initial render**, you update the component's state or receive new props. When the state or props of a component change, React automatically triggers a re-rendering of the component.

React does not recreate **DOM nodes** on every re-render. Instead, it updates the existing DOM nodes with the necessary changes. React's **reconciliation** identifies the differences between the previous virtual DOM and the new virtual DOM and selectively applies those changes to the actual DOM. This approach is more efficient than recreating the entire DOM from scratch.

## React Updates DOM Now What?

- React has committed the changes, the browser performs the layout process to calculate the size and position of elements based on the updated DOM. After layout, the browser performs the **paint** operation, which involves rendering the updated elements onto the screen.

### Additional Resources

[Your First Component](https://react.dev/learn/your-first-component)

[Importing and Exporting Components](https://react.dev/learn/importing-and-exporting-components)

[Writing Markup with JSX](https://react.dev/learn/writing-markup-with-jsx)

[sass cheatsheet](https://devhints.io/sass)

[react cheatsheet](https://devhints.io/react)

### Learning Goals

Hooks.. and state management.
