# AWS: Events

[AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

## Simple Queue Service

*Difference between SQS and SNS*:

**SQS**: SQS is a fully managed message queuing service. It enables you to decouple the components of a distributed system by allowing them to communicate asynchronously. Messages are stored in a queue and can be retrieved by one or more consumers.

**SNS**: SNS is a fully managed publish-subscribe messaging service. It allows you to send messages to multiple subscribers, known as endpoints, through various protocols such as HTTP/S, email, SMS, or even AWS Lambda. SNS follows a push-based model, where a single message is delivered to multiple subscribers simultaneously.

*Use cases for SQS and SNS*:

**SQS**: SQS is suitable for use cases where you need reliable and scalable message queuing. Some examples include decoupling application components, handling background jobs, distributing tasks to multiple workers, and building event-driven architectures.

**SNS**: SNS is useful when you want to send messages or notifications to multiple subscribers at the same time. It is commonly used for broadcasting messages to mobile devices (push notifications), distributing event notifications, triggering AWS Lambda functions, and sending notifications via email or SMS.

[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

*Using SQS and SNS in a "fanout" pattern*:

The **fanout pattern** refers to broadcasting a message to multiple endpoints using SNS.

- Create an SNS topic
- Subscribe multiple SQS queues or other endpoints (e.g., HTTP/S, email) to the SNS topic.
- When a message is published to the SNS topic, it will be delivered to all subscribed endpoints simultaneously, including the SQS queues.

*How push notifications work using SNS*:

- Configure SNS to use the appropriate push notification platform

- Obtain the device token or registration ID for each mobile device and register them with SNS.

- When you want to send a push notification, publish a message to the SNS topic associated with the mobile devices.

- SNS will use the device tokens/registration IDs to deliver the push notification to the respective devices through the push notification service.

[SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

*Large-scale, distributed applications and SQS*:

SQS can be used to handle communication between various components or microservices in a large scale distributed application.

- A web application can send requests to an SQS queue, which is then processed by multiple worker instances asynchronously.
- Different microservices can communicate by exchanging messages through SQS queues, enabling loose coupling and scalability.
- SQS can act as a buffer to handle bursts of traffic or spikes in demand.
- Helps in decoupling different components, making the system more resilient and fault-tolerant.


## Additional Resources

[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)
[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)
