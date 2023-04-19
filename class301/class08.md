# API's

[API Design Best Practices](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)

## What Is REST?

- **REST** -  Representational State Transfer. It is an architectural style for designing web services.

- REST APIs are designed around resources, which can be any type of object, data, or service that can be accessed

- Identifier of a resource is a unique string that identifies a specific resource. For example, in a REST API for a blog, a blog post might be identified by its ID.

- GET, POST, PUT, PATCH, and DELETE are the most common **HTTP verbs**.

- URIs should be based on the resources they identify.

- Good URI's should be descriptive, unique, and based on the resource it identifies.

>Ex: '/users'

- **Chatty URI's** are considered a bad thing because they can lead to slow performance. These require multiple requests to perform a single operation.

- **successful GET request** - will return a status code of 200 OK.

- An **unsuccessful GET request** - returns a status code of 404 Not Found.

- A **successful POST request** - returns a status code of 201 Created.

- A **successful DELETE request** - returns a status code of 204 No Content.

## Additional Resources

[RegExr](https://regexr.com/)

[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)

[Regex 101](https://regex101.com/)
