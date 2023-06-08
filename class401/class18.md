# AWS: API, Dynamo and Lambda

[AWS API Gateway Overview](https://www.serverless.com/guides/amazon-api-gateway)

*Amazon API Gateway* - allows developers to create, publish, monitor, and secure APIs (Application Programming Interfaces) for their applications. It acts as a gateway or entry point for clients to access backend services or resources securely.

- It plays a big role in serverless ecosystem because it enables developers to build serverless architectures easily. Serverless computing is an approach where developers can focus on writing code without worrying about server provisioning, scaling, or infrastructure management.

API Gateway integrations:

- **AWS Lambda**: API Gateway can directly trigger Lambda functions, allowing you to build serverless APIs easily.

**AWS Identity and Access Management** (IAM): API Gateway integrates with IAM to provide authentication and authorization mechanisms for API access control.

**AWS Cognito**: API Gateway can be integrated with Cognito, which is AWS's user authentication service, to manage user sign-up, sign-in, and access control for APIs.

**AWS S3**: API Gateway can integrate with Amazon S3 to directly proxy requests to S3 buckets, enabling you to expose S3 resources via APIs.

**AWS DynamoDB**: API Gateway can be used to create APIs that interact with DynamoDB, AWS's managed NoSQL database service.

[AWS API Gateway](https://aws.amazon.com/api-gateway/)

*Amazon API Gateway Benefits*:

- **API Management**: It provides a centralized platform for managing APIs, including versioning, access control, monitoring, and analytics.

- **Scalability**: API Gateway automatically scales to handle high traffic loads, ensuring that your APIs can handle a large number of concurrent requests.

- **Security**: It offers various security features, such as authentication and authorization mechanisms, encryption, and protection against common web exploits.

*Amazon API Gateway API Types*:

- **REST APIs**: (Representational State Transfer) use HTTP methods like GET, POST, PUT, DELETE to interact with resources.

- **WebSocket APIs**: Real-time bidirectional communication between clients and servers over a persistent connection.

[AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

*What Is DynamoDB*?

- Fully managed NoSQL database service provided by AWS. Designed to handle large amounts of structured and semi-structured data with high scalability and performance.

- Powerful choice for applications with variable and unpredictable workloads.

- Predictable Performance, Massive Scalability, and Serverless Integration.

[AWS DynamoDB](https://aws.amazon.com/dynamodb/)

**DynamoDB** is like a magical bookshelf where you can store a huge number of books without worrying about running out of space. It can quickly find any book you want to read and lets you read it without waiting.

[Dynamoose](https://dynamoosejs.com/getting_started/Introduction)

*What Is Dynamoose*?

- open-source modeling library for Node.js that simplifies working with DynamoDB. Dynamoose provides an object-oriented interface for interacting with DynamoDB, allowing developers to define models, perform CRUD operations, and perform complex queries using familiar JavaScript syntax.

*Key Features of Dynamoose*:

- Dynamoose allows developers to define the data structure (schema) for their DynamoDB tables using JavaScript classes and data types.
