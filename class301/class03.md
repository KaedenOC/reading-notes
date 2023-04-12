# Passing Functions as Props

[React Docs - lists and keys](https://legacy.reactjs.org/docs/lists-and-keys.html)

## .map() Method

- **.map()** is used on arrays and returns a new array.

- We want to use the .map() method when building collections of elements and include them in JSX (JSX stands for JavaScript XML) using curly braces.

``` javascript

const numbers = [1, 2, 3, 4, 5];<br>
const listItems = numbers.map((number) =>
 <li>{number}</li>
);
```

## Basic List Component

Usually you would render lists inside a *component*.

- When creating lists of elements, we will want to include a **"key"** which is a special string attribute.

``` javascript

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li key={number.toString()}>
      {number}
    </li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

```

- **key** - Help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

- Best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data.

[The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

## The Spread Operator

Useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into functions arguments.

> Syntax: (...)

### What Can Spread Do?

- *Copying an Array*.

``` javascript

const myArray = [1, 2, 3, 4, 5];
const copiedArray = [...myArray];
console.log(copiedArray);

```

- *Concatenating or combining arrays.*

``` javascript

const array1 = [1, 2, 3];
const array2 = [4, 5, 6];
const combinedArray = [...array1, ...array2];
console.log(combinedArray);

```

- Using Math functions.

- Using an array as arguments.

- *Adding an item to a list.*

``` javascript

const myArray = [1, 2, 3, 4, 5];
const newItem = 6;
const newArray = [...myArray, newItem];
console.log(newArray);

```

- *Combining Objects.*

``` javascript

const obj1 = { name: 'Kaeden', age: 25 };
const obj2 = { city: 'New York', country: 'USA' };

const combinedObj = { ...obj1, ...obj2 };
console.log(combinedObj);

```

## Passing Functions Between Components

[How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

- In the video the developer start off by defining a function within the parent component to pass to its child component.

- Increment passes in name from the object that will look like name: 'bob'.  Then need to iterate through the array, without modifying it, the developer uses the .map method to create a new array 'ppl'. The developer passes in 'p' into the map method for 'people' and checks if the name matches the name thats passed in and then increments the count. Then returns p. Then updates the state.

- You pass a method from a parent component into a child component by defining the method in the parent component then pass it as a prop in the child component.

- The child component invokes a method that was passed to it by a parent component by calling the method like in a regular javascript function.

``` javascript

this.props.increment();

```

### Additional Resources

[React Tutorial through ‘Declaring a Winner’](https://react.dev/learn/tutorial-tic-tac-toe)

[React Docs - Lifting State Up](https://legacy.reactjs.org/docs/lifting-state-up.html)