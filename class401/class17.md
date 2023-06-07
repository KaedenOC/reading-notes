# AWS: S3 and Lambda

[AWS S3](https://aws.amazon.com/s3/)

- **Amazon S3** - Amazon Simple Storage Service, is a scalable cloud storage service provided by AWS. It allows you to store and retrieve large amounts of data over the internet. Great for object storage, files, images, videos.

- **Some Use Cases For S3** - Data Backup and Recovery, Data Archiving, Static Website Hosting, and Content Distribution.

- **Benefits**: Scalability - scale to store any amount of data, Durability and Availability - designed to provide high durability, ensuring that your data is protected against failures, Security - robust security features to protect your data, Cost-Effectiveness - flexible pricing options based on the storage class, access patterns, and data transfer.

[AWS Lambda Basic](https://www.serverless.com/aws-lambda)

- **AWS Lambda** - serverless computing service provided AWS. It allows you to run your code without provisioning or managing servers. Lambda automatically scales your applications in response to incoming requests or events, ensuring that you pay only for the compute time you actually consume.

- **What Is A lambda** - a function

- **Some Use Cases For AWS Lambda** - Event-Driven Processing, Real-time File Processing, Web and Mobile Backend, and Data Transformation.

## "SERVERLESS"

It's like having a personal chef who prepares the food you need whenever you want it, without you having to worry about cooking or cleaning up afterwards.

[CDN](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)

**Content Delivery Network** - distributed network of servers located in various data centers around the world.

## How Does A CDN Work?

A visitor requests a website or its content, the request is routed to the nearest edge location in the CDN network. The CDN server in that location caches and stores a copy of the content. Requests for the same content from other visitors in the same region can be served directly from the nearby edge server without needing to go back to the origin server where the website is hosted.

- **Benefits** - Improved Website Performance - By caching content closer to the end-user, a CDN reduces the distance and time it takes for content to travel. Global Content Delivery - across different regions globally allows for efficient content delivery. Scalability - can handle high traffic loads and sudden spikes in demand by distributing the load across multiple servers. Load Balancing - can intelligently distribute traffic among multiple servers to balance the load and prevent individual servers from becoming overwhelmed.


```javascript

//trigger for the lambda: upload a json file.

//json file ---> S3 Bucket ---> lambda ----> return result back to S3
//need putObject and getObject

```