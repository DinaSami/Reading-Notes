## AWS: S3 and Lambda

### Review, Research, and Discussion

Describe “The Cloud” :
"The cloud" refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world. By using cloud computing, users and companies don't have to manage physical servers themselves or run software applications on their own machines.

What is a container (as it relates to computers and servers)?
A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. 

What is auto-scaling?
AWS Auto Scaling monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. 

What is bandwidth?
Bandwidth is often mistaken for internet speed when it's actually the volume of information that can be sent over a connection in a measured amount of time – calculated in megabits per second (Mbps)

### Terms

* Server Instances:
  * Server instances refer to an instance of server deployment. For instance on AWS an instance can be created on a virtual machine that is hosting a server and then that instance can be stopped.

* Containers:
  * Containers are services that package software into units for development, shipment and deployment and can be used to hold files and other software used in online applications

* Cloud Services:
  * Cloud services refer to virtual machine services that are accessible through the internet. These services can be storage, web hosting, and other forms of computer activities that one uses an online computer for. Examples are AWS and Azure

* Cloud Architecture:
  * Cloud architecture refers to the components that are necessary for building a cloud and consist of a front-end, back-end, cloud based delivery, and ndetwork.

* AWS
  * AWS is Amazon Web Services and refers to Amazon's cloud computing services. They offer various services that range from S3 storage containers to Elastic Beanstalk which is able to host web applications

* EC2/Beanstalk vs. Heroku :
  * EC2 refers to the elastic computing service and beanstalk is a way to deploy applications in a way similar to Heroku. These two solutions offer roughly comparable services, SQL services on AWS are more secure, and Herokue offers more robust Dynos. At the same time Heroku is easier to use and setup but has greater price jumps with scaling.
 

### Preparation Materials

* AWS Lambda - The Ultimate Guide :

AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services.

Each Lambda function runs in its own container. When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS. Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity. Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running. The customers then get charged based on the allocated memory and the amount of run time the function took to complete.

When building Serverless applications, AWS Lambda is one of the main candidates for running the application code. Typically, to complete a Serverless stack you’ll need:

- a computing service;
- a database service; and
- an HTTP gateway service.

Some of the most common use cases for AWS Lambda that fit these criteria are:

Scalable APIs. When building APIs using AWS Lambda, one execution of a Lambda function can serve a single HTTP request. Different parts of the API can be routed to different Lambda functions via Amazon API Gateway. AWS Lambda automatically scales individual functions according to the demand for them, so different parts of your API can scale differently according to current usage levels. This allows for cost-effective and flexible API setups.

Data processing. Lambda functions are optimized for event-based data processing. It is easy to integrate AWS Lambda with datasources like Amazon DynamoDB and trigger a Lambda function for specific kinds of data events. For example, you could employ Lambda to do some work every time an item in DynamoDB is created or updated, thus making it a good fit for things like notifications, counters and analytics.

Task automation. With its event-driven model and flexibility, AWS Lambda is a great fit for automating various business tasks that don’t require an entire server at all times. This might include running scheduled jobs that perform cleanup in your infrastructure, processing data from forms submitted on your website, or moving data around between different datastores on demand.

