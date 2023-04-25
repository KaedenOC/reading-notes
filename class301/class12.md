# CRUD

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

## Status Codes

- **100's** - Informational. Indicates that the request was received and the process is continuing.

- **200's** - Success. Indicates that the request was successful.

- **300's** - Redirection. Indicates that further action is needed to complete the request.

- **400's** - Client Error. Indicates that there was an error on the client side.

- **500's** - Server Error. Indicates that there was an error on the server side.

- **202** - That the request has been accepted for processing, but the processing has not been completed yet.

- **308** - That the resource has been moved permanently to a new location and the client should update its URL.

- If an update didn't return data to a client, you would use the status code **204** No Content.

- You would use the status code **410** Gone, if a resource used to exist but no longer does.

- **403** -  'Forbidden' - The client does not have permission to access the requested resource.

## Build With Node.js, Express, and MongoDB

- We need to pull our MongoDB database string out of our server and put it into our .env file for security reasons, as we don't want to expose sensitive information in our code.

- **Middleware** is a function that sits between the client and the server and can modify the request or response as needed. It can also perform other tasks, such as logging or authentication.

- **app.use(express.json())** is middleware that allows our server to parse incoming requests with JSON.

- The **/:id** in a route is a parameter that allows us to access a specific resource based on its ID.

- **PUT** is used to update an entire resource, while PATCH is used to update only part of a resource.

- Set a default value for a field using the "default" property in the schema definition.

- **500** error status code means that there was a server error and the request could not be completed.

- Difference between a status 200 and a status 201 is that a 200 status code means that the request was successful, while a 201 status code means that the request was successful and a new resource was created as a result.