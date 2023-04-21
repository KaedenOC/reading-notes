# In Memory Storage

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

## Call

- A **call** refers to the execution of a function in JavaScript. Whenever a function is called, the JavaScript interpreter places it on the top of the call stack and executes it.

- Execute one piece of code at a time. Therefore, only one call can happen at once. **(single threaded).**

- **Last In, First Out** - (LIFO), last function that was pushed onto the call stack is the first one to be popped off and executed.

 ``` javascript
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();

```

- **Stack Overflow** - When the call stack exceeds its maximum size, and this can happen if a function calls itself recursively without a proper exit condition, causing an infinite loop.

[JavaScript error messages](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

- **Reference Error** - when a variable or function is referenced that does not exist.

- **Syntax Error** - When there is a mistake in the structure of the code. Missing or incorrect punctuation, misspelled keywords, or incorrect use of operators.

- **Range Error** - When a value is outside the range of legal values.

- **Type Error** - When a value is not of the expected type.

- **Breakpoint** - Point in the code where execution can be paused, allowing developers to inspect the state of the program and debug any issues.

- **debugger** -  Tool that allows developers to pause the execution of the code and inspect the state of the program at a specific point.

## Additional Resources

[JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)
