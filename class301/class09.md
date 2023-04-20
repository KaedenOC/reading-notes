# Functional Programming

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

## What Is Functional Programming

- **Functional Programming** - programming paradigm, a style of building the structure and elements of computer programs and evaluation of mathematical functions and avoids changing-state and mutable data.

- **Pure Function** - Always returns the same output given the same inputs and does not have any side effects.

- Examine the inputs, outputs, and whether or not the function causes observable side effects.

- **What are the benefits of a pure function?** - They are easier to reason about and test. (output of the function is solely dependent on its inputs).

- **Immutability** - Unchanging over time or unable to be changed. State cannot change after it’s created.

- **Referral Transparency** - Property of a function that means the function can be replaced with its resulting value without changing the behavior of the program.

## Node.JS Cont.

[Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

- **Module** -  Can be a single file or a collection of files that contain related functionality. Reusable block of code.

- **require()** - Import a module into a file.

 ``` javascript 
 let counter = function(arr) {
  return 'there are ' + arr.length + ' elements in this array';
}

module.exports = counter;

```

'different file'

``` javascript

let counter = require('./count');
console.log(counter(['shaun', 'crystal', 'ryu']));

```

- The exports are the variables, functions, or objects that the module makes available for other parts of the program to use.
