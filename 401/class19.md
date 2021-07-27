## AWS: API, Dynamo and Lambda

### Review, Research, and Discussion

- List the AWS Database offerings and talk about the pros and cons of each:
- 
Amazon Relational Database Service or Amazon RDS is a managed cloud database service from AWS. It is a service designed to simplify the creation, operation, management, and scaling of a relational database for use as an application backend.

- What’s the difference between a FIFO and a standard queue?
Standard queues provide best effort ordering meaning they try to output data in which the order they come in but occasionally it will output out of order. FIFO is strictly first in first out meaning it exactly one processing and always outputs in order.

- How can the server be assured a message was properly received?
The message is stored on the queue until another component called a consumer retrieves the message and does something with it.
The client (usually a browser) opens a connection to the server and sends a request. The server processes the request, generates a response, and closes the connection if it finds a Connection: Close header. Headers may provide various information about the request or the client body data.

### Terms

- Serverless API - An application that has a cloud prvider such as AWS API Gateway that dynamically manages the allocataion and provisioning of servers for the app. The API runs in a stateless compute container that is event triggered.
- Triggers - Procedures that are stored in a database and are fired when an event happens. 
- Dynamo vs Mongo - Although similar in many ways, Mongo can be deployed anywhere and Dynamo is only available on AWS. Dynamo is a fully managed AWS service as opposed to Mongo being seld installed and self managed. Dynamo uses tables, items and attributes, and Mongo uses JSON like objects. Dynamo has access to many more AWS services to develop a complete app.
- Dynamoose vs Mongoose - Dynamoose is a modeling tool used for Dynamo and acts very similarily to the way Mongoose does with Mongo. Dynamoose allows the use of a schema and CRUD operations.

### Preparation Materials

AWS SQS vs SNS:

SNS (Simple Notification Service):

Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.

SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

SQS (Simple Queue Service):

Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.
SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can’t be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later.


