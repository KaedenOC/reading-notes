# Putting It All Together

[React Docs - Thinking in React](https://react.dev/learn/thinking-in-react)

## Single Responsibility Principle

Think about splitting up design into components in different ways:

- The **single responsibility** principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

- **CSS** — consider what you would make class selectors for.

- **Design** — consider how you would organize the design’s layers.

### Build a Static Version

 Build a version that renders the UI from your data model without adding any interactivity.

- To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props(*Props are a way of passing data from parent to child*).

- We can either build "top down" or "bottom up" and its usually easier to go top down, but on bigger projects it can be easier to go bottom-up.

## Find the Representation of UI state

You need to let users change your underlying data model in order to make the UI interactive.

- **state** - minimal set of changing data that your app needs to remember. The most important principle for structuring state is to keep it DRY (Don’t Repeat Yourself).

- Does it remain unchanged over time? If so, it isn’t state.

- Is it passed in from a parent via props? If so, it isn’t state.

- Can you compute it based on existing state or props in your component? If so, it definitely isn’t state!

### Where State Should Live

- You can put the state directly into their common parent.

- Put the state into some component above their common parent.

- You can also create a whole new component to store state if you can't find a component.

## Higher Order Functions

[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

Functions that operate on other functions, either by taking them as arguments or by returning them.

EX: defining an arrow function and returning a boolean value depending on whether m is > n.

``` javascript

function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true

```

### The .map() Method With Higher Order Functions

The map method transforms an array by applying a function to all of its elements and building a new array from the returned values.

``` javascript

function map(array, transform) {
  let mapped = [];
  for (let element of array) {
    mapped.push(transform(element));
  }
  return mapped;
}
```

## array.reduce() Method

[CodeFellows Reduce Overview](https://codefellows.github.io/code-301-guide/curriculum/class-05/challenges/)

arr.reduce( (accumulator,value,index) => {...}, initialvalue)

- **.reduce()** -  Iterates over an array and returns the last version of the “accumulator”.

- It takes a callback function as its first argument which is called for each element in the array during the iteration.

- Callback function receives three parameters: the accumulator, the current value, and the current index of the element being processed.