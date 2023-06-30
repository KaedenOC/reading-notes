# API Integration

[Review API Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/api-server/)

**Query String Parameter**: These parameters are appended to the end of the URL after a question mark (?). They are typically used to filter, sort, or paginate data and are optional.

**Path Parameter**: Path parameters are part of the URL path itself, represented by placeholders enclosed in curly braces. They are used to identify a specific resource or endpoint and are typically required.

## "Interface"

- It's like a secret door with a magic spell written on it. When someone (like a mobile app or website) wants to request information or perform specific actions, they say the magic word (send an API request) to the door, and it opens. The door understands the request, performs the necessary actions, and gives back the result, all using this special language (the API interface) they both understand.

[Review Auth Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/auth-server/)

## Middleware for Basic and Bearer Auth

- Middleware is a piece of software that sits between the client and the server and can intercept and process requests before they reach the main application logic.

- **Basic Auth**

The middleware intercepts incoming requests and checks if they have the Authorization header with a "Basic" authentication type.
If the header is present, the middleware extracts the Base64-encoded username and password.
The middleware then validates the credentials against the database or user store.
If the credentials are valid, the request is allowed to proceed; otherwise, the client receives a 401 Unauthorized response.

- **Bearer Auth**

The middleware intercepts incoming requests and checks if they have the Authorization header with a "Bearer" authentication type.
If the header is present, the middleware extracts the access token.
The middleware then validates the access token, ensuring it is not expired and has not been tampered with.
If the token is valid, the request is allowed to proceed; otherwise, the client receives a 401 Unauthorized response.

## Handshake for Implementing OAuth

- a secure way to grant access to your resources on one website to another website without sharing the user's credentials.

- User Wants to Grant Access, The Third-Party Application Redirects the User, User Authorizes the Request, OAuth Provider Issues an Authorization Code, The Third-Party Application Exchanges the Code for an Access Token, and Access Token Usage.

## RBAC Role Based Access Control

- Imagine Role-Based Access Control as a magical castle with different rooms, each guarded by a special key. In this castle, there are different roles or positions like "King," "Knight," and "Servant." Each role has a specific set of tasks and responsibilities. For example, the "King" can enter all the rooms, the "Knight" can access some rooms, and the "Servant" can only go to a few specific rooms.

Now, to open a door and enter a room, you need a unique key that matches the lock on that door. In our castle, the "King" has a master key that can open any door, the "Knight" has a key that opens some doors, and the "Servant" has their own key for their permitted rooms.

If you want to enter a room, you must show your identity and the key you possess. The castle's guards (the access control system) will check your role and the corresponding key. If your key matches the room's lock and you have the right role, they will allow you to enter.