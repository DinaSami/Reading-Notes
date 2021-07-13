##  Event Driven Architecture

### Review, Research, and Discussion

- What is the difference between FIFO and a standard queue is that in a FIFO queue the order of the data matters and in a standard queue it does not. 
- A server be assured a message was properly received if that message emits an event akin to 'recieved' that is sent to the server. 
- What classic design pattern is best represented by event driven programming -- event loop. 
- How do you test an event driven system? To test an event driven system you could come up with assertions that were based on the events emitted during the event loop. 

### Terms

- FIFO Queue: First in first out queue.  Order matters.

- Pub/Sub: "an asynchronous messaging service that decouples services that produce events from services that process events".

### Preparation Materials

What are the benefits of using Amazon SNS?

Amazon SNS offers several benefits making it a versatile option for building and integrating loosely-coupled, distributed applications:

Instantaneous, push-based delivery (no polling)
Simple APIs and easy integration with applications
Flexible message delivery over multiple transport protocols
Inexpensive, pay-as-you-go model with no up-front costs
Web-based AWS Management Console offers the simplicity of a point-and-click interface


What is Amazon Simple Notification Service (Amazon SNS)?

Amazon Simple Notification Service (Amazon SNS) is a web service that makes it easy to set up, operate, and send notifications from the cloud. It provides developers with a highly scalable, flexible, and cost-effective capability to publish messages from an application and immediately deliver them to subscribers or other applications. It is designed to make web-scale computing easier for developers. Amazon SNS follows the “publish-subscribe” (pub-sub) messaging paradigm, with notifications being delivered to clients using a “push” mechanism that eliminates the need to periodically check or “poll” for new information and updates. With simple APIs requiring minimal up-front development effort, no maintenance or management overhead and pay-as-you-go pricing, Amazon SNS gives developers an easy mechanism to incorporate a powerful notification system with their applications.

How does Amazon SNS work?

It is very easy to get started with Amazon SNS. Developers must first create a “topic” which is an “access point” – identifying a specific subject or event type – for publishing messages and allowing clients to subscribe for notifications. Once a topic is created, the topic owner can set policies for it such as limiting who can publish messages or subscribe to notifications, or specifying which notification protocols will be supported (i.e. HTTP/HTTPS, email, SMS). Subscribers are clients interested in receiving notifications from topics of interest; they can subscribe to a topic or be subscribed by the topic owner. Subscribers specify the protocol and end-point (URL, email address, etc.) for notifications to be delivered. When publishers have information or updates to notify their subscribers about, they can publish a message to the topic – which immediately triggers Amazon SNS to deliver the message to all applicable subscribers.

