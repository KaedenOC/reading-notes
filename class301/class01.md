# Introduction to React and Components

## Component Based Architecture

[Component Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

### What Is A Component?

A small piece of code that fills a certain part of the user interface that you're building with react.

- It is a software object, intended to interact with other components.

- It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

### Characteristics of Components

- **Reusability** - designed to be reused in different situations, and some components may be designed for a specific task.

- **Replaceable** - may be freely substituted with other similar components.

- **Not context specific** - designed to operate in different environments and contexts.

- **Extensible** - extended from existing components to provide new behavior.

- **Encapsulated** - refers to the practice of hiding the internal details of a component from the outside world.

- **Independent** - designed to have minimal dependencies on other components.

### Advantages

- **Ease of deployment** - it is easier to replace existing versions with no impact on the other components or the system as a whole.

- **Reduced cost** - The use of third-party components allows you to spread the cost of development and maintenance.

- **Ease of development** - allow the ability to implement well-known interfaces. Allowing development without impacting other parts of the system.

## Props

[What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)

### What Is Props?

Props is a keyword which stands for properties and is being used for passing data from one component to another.

- Data with Props are being passed one way from parent to child.

- Props are read-only, data coming from a the parent child should not be changed by child components.

- A Prop is an Object.

### Interpolation

Define our own attributes and assign values with interpolation.

> Ex: ``` <ChildComponent someAttribute={value} anotherAttribute={value}/> ```

### Using Props

How to use Props in React.

- Firstly, define an attribute and its value(data)

- Pass it to child component(s) by using Props.

- Render the Props Data.

- Props can only be passed to components in one way.. that is (parent to child).


### Additional Resources:

- [React Tutorial through 'Passing Data Through Props'](https://react.dev/learn/tutorial-tic-tac-toe)

- [React Docs - Hello World](https://legacy.reactjs.org/docs/hello-world.html)

- [React Docs - Introducing JSX](https://legacy.reactjs.org/docs/introducing-jsx.html)

- [React Docs - Rendering Elements](https://legacy.reactjs.org/docs/rendering-elements.html)

- [React Docs - Components and Props](https://legacy.reactjs.org/docs/components-and-props.html)