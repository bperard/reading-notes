# 419

## AWS SQS vs SNS

- What is the difference betweeen SQS and SNS?  
The main difference between SQS and SNS is in the way they handle messages. SQS is a queue-based messaging system, while SNS is a topic-based messaging system. In other words, with SQS, messages are stored in a queue until they are processed by the consumer, whereas with SNS, messages are sent to subscribers who have registered to receive messages on a particular topic.

- What are some use cases for both SNS and SQS?  
SQS is typically used when there is a need for asynchronous communication between different parts of a system, or when there is a need to decouple different components of an application.

SNS is typically used when there is a need for real-time communication between different components of a system, or when multiple subscribers need to be notified of events occurring on a particular topic.

## AWS SNS and SQS

- Describe how to use SQS and SNS in a “fanout” pattern.  
To use SQS and SNS in a fanout pattern, you would use SNS to publish messages to a topic and then configure multiple SQS queues as subscribers to that topic. This way, when a message is published to the topic, it is delivered to all subscribed SQS queues, and each queue can process the message independently.

- Explain how “push notifications” work, using SNS.  
Create an SNS topic for the push notifications. Create a platform application endpoint for the client device, such as an iOS or Android app.
Register the endpoint with SNS and subscribe it to the SNS topic. When a push notification needs to be sent, publish a message to the SNS topic. SNS delivers the message to the registered endpoint, and the client device displays the notification.

## SQS and SNS Basics

- How might a large scale, distributed application make use of a Queue system like SQS?  
By using SQS, different components of a distributed application can communicate asynchronously, without being tightly coupled. For example, if one component needs to send a message to another component, it can do so by placing the message in an SQS queue. The other component can then consume messages from the queue at its own pace, without the need for synchronous communication between the two components.
