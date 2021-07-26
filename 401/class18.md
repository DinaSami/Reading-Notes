## AWS: API, Dynamo and Lambda

### Review, Research, and Discussion

1- What are serverless functions?
A serverless function is a programmatic function written by a software developer for a single purpose.

2- If you were to create a system that emulated Lambda functions, how would you do it?
To create a Lambda function with the console

- Open the Functions page on the Lambda console.

- Choose Create function.

- Under Basic information, do the following:

- For Function name, enter my-function.

- For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.

- Choose Create function.

3- Describe how a CDN works
Over half of the internet’s traffic is served by a content delivery network (CDN). The goal of the CDN is to reduce latency – the delay between submitting a request for a web page and the web page fully loading on your device – by reducing the physical distance that the request has to travel.

### Terms

* Serverless Functions:
* 
  * Serverless functions can be thought of as micro-applications and micro-architecture. They are usually event triggered code and targeted code. One of the benefits is that functions can scale independently as needed.

* Cloud Storage:
* 
  * Cloud storage refers to file and data storage in the cloud or in other words on servers accessible through the internet. Examples of cloud storage are AWS S3 and iCloud by Apple.

* CDN:
* 
  * CDN refers to content delivery network. They are combinations of geographically located servers that allow for fast delivery of data. When a user accesses a cdn the servers which are located closest are activated. An example of CDN can be found in jQuery and Font Awesome

### Preparation Materials

What is Amazon API Gateway?
Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

How does API Gateway work?
API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

What is DynamoDB?
DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

reliable performance even as it scales;
a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
a small, simple API allowing for simple key-value access as well as more advanced query patterns.

Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

