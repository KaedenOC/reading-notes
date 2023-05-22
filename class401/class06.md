# Authentication

[Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

## Safely Hash and Store A Password

- Creating an account or setting a password uses a process called hashing. A one-way function that takes your password as input and produces a unique string of characters as output. This also looks completely different than your password. 

## Bcrypt

Bcrypt is a widely used and trusted algorithm designed specifically for password hashing. It is known for its security and resistance to attacks.

- used to safely hash and store a password.

- known for its security and resistance to attacks.

- **salting** - adds a random value, called a salt, to your password before hashing it. This salt makes it more difficult for attackers to crack the passwords using precomputed tables or rainbow tables.

- intentionally slow, making it computationally expensive for attackers to crack passwords through brute-force or dictionary attacks.

- automatically handles the generation and management of salts.

- can ensure that even if the database is compromised, the original passwords remain secure and cannot be easily reversed or exploited by attackers.

## Auth

[Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)

A simple authentication scheme used in HTTP to provide a basic level of access control for web resources. It involves sending a username and password as part of the request headers to authenticate a user's identity.

- **Authorization Header** - `Authorization: Basic <base64-encoded-username:password>` used to carry the authentication credentials.

- server receives the basic auth request, and decodes the Base64-encoded string to retrieve the username and password.

## OWASP

[OWASP auth cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

**Authentication** is the process of verifying the identity of a user or entity accessing a system or application. It ensures that only authorized individuals or entities can gain access to protected resources.

- User provides their credentials, such as a username and password. Application verifies the credentials to determine if they are valid.

- If credentials are valid, the user can access the application.

- **HTTP Error Messaging** - errors that occur should respond with appropriate HTTP status codes.

- *401 Unauthorized* - user's credentials are missing or invalid. It informs the client that authentication is required.

- *403 Forbidden* - returned when the user's credentials are valid but they are not authorized to access the requested resource.

- **HTML Error Messaging** - These messages should be clear and helpful, informing the user about the nature of the error and guiding them on how to resolve it.

- These error messages can help improve the user experience and potential security vulnerabilities.

## Bookmark and Review

[bcrypt docs](https://www.npmjs.com/package/bcrypt)

### Additional Questions

I'm looking forward to learning more about Authentication. I remember touching on Auth0 a bit in 301, and would like to learn more.

- "cryptographic hash and cypher algorithms" in the class README for us to be able to define. This sounds interesting.
