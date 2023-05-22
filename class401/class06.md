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


