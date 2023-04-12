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

