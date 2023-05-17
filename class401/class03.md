# Express REST API

[Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

## ES6 Classes

- **Classes** are a template for creating objects.

- Class declarations cannot be hoisted. They must be declared before they are used in the code.

- Contextual "this" refers to the current object that is being operated on within a method or constructor of a class. Access and modify the properties and methods of the current object. Use "this" to refer to the object you're working with in the code.

[Using Express Routing](https://expressjs.com/en/guide/routing.html)

## Express

- **Routing** refers to the process of defining how an application responds to client requests for specific URLs (or routes). app.get() to handle GET requests and app.post to handle POST requests. app.use() to specify middleware as the callback function.

- **Route Path** refers to the URL pattern or pattern matching mechanism used to define the specific URL(s) that a route handler should be associated with. **Route Method** refers to the HTTP method (such as GET, POST, PUT, DELETE, etc.) that a route handler should respond to.

> Ex: `app.get('/users', handler)` defines a route handler that will be executed when a GET request is made to the '/users' URL path.

- **next** - add as a param to a route handler or middleware when you want to pass control to the next middleware function in the chain. (function provided by express) when you want to perform some processing or validation in a middleware and then pass control to the next middleware or route handler. When passed, must call it to ensure that the execution flow proceeds to the next middleware or route handler.

[Express Routing](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4)

- **Express Router** - Provided by the Express framework that allows you to create modular and reusable sets of routes. Organize and group routes. 

- call an instance of the `express.Router()`, apply routes to it, and then tell our application to use those routes.

- **Route Middleware** - Used to perform additional processing or operations on a request or response object before it reaches the final route handler. Check if a user is authenticated, logging data for analytics, or anything else we’d like to do before we actually spit out information to our user.

## Reflection

- Looking forward to learning about express (modular) routing. 