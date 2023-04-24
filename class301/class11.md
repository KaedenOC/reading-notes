# MongoDB and Mongoose

## nosql vs sql

[nosql vs sql Reading](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

- **SQL** - Relational Databases, table based databases, predefined schema, vertically scalable,  **structured query language**, not best fit for hierarchical data storage.

- **NoSQL** - primarily called as non-relational or distributed database, document based, key-value pairs, graph databases or wide-column stores, dynamic schema for unstructured data, horizontally scalable, queries are focused on collection of documents, **Unstructured Query Language**, not good fit for complex queries, fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.

## SQL

- SQL databases are a good fit for data that has a well-defined structure and relationships between tables.

- Real World Example: A business that has customers which contains information about the customers.

## NoSQL

- Good fit for unstructured or semi-structured data.

- Real world example: Social Media platform's user-generated content database, which contains posts, comments, and likes.

- **Hierarchical data storage** is best handled by a NoSQL database, specifically a document-oriented database.

- **NoSQL** - designed to scale horizontally, by adding more commodity servers, rather than vertically, by adding more powerful hardware. Handle large volumes of data and traffic without compromising performance.

[sql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

## SQL and NoSQL

- **SQL** stands for **Structured Query Language**.

- **Relational database** - type of database that organizes data into one or more tables with a predefined structure. Works with tables and relationships between tables.

- **Schema** - blueprint or a plan for how a database is organized, which includes the tables, fields, and relationships between them.

- **NoSQL**  non-relational database that stores and retrieves data in a way that does not use tables with a fixed schema.

- NoSQL databases work by storing data in flexible, unstructured ways, using various data models.

- **MongoDB** - document-oriented NoSQL database, which stores data in collections of JSON-like documents that can have varying structure.

- MongoDB is more flexible than SQL because it does not have a fixed schema and can store data in a variety of ways.

- NoSQL may lack data integrity that is ensured by SQL databases.