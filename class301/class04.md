# React and Forms

[React Docs - Forms](https://legacy.reactjs.org/docs/forms.html)

## Controlled Components

In React, mutable state is typically kept in the state property of components, and only updated with **setState().**

- With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.

- React state be the “single source of truth”.

- With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.

### How do we target what the user is entering if we have an event handler on an input field?

```javascript
event.target.value

```

## Ternary Operator


[The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

- Shorten your if statements into one line of code with the conditional operator.

```javascript

person.driver = person.age >=16 ? 'Yes' : 'No';

condition ? value if true : value if false

```

- Condition is what you are testing. The result of your condition should be true or false.

- A **?** separates our conditional from our true value. Anything between the **?** and the **:** is what is executed if the condition evaluates to true.

- If your condition evaluates to false, any code after the colon is executed.

### Rewrite the following statement using a ternary statement:

```javascript

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

console.log(x === y ? true : false);

```

## Additional Resources

[React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)

[React Docs - conditional rendering](https://legacy.reactjs.org/docs/conditional-rendering.html)