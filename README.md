# Games
Storing the details about the Games played by the participants and scores earned.

# Architecture

![](images/AWS%20Architectture.PNG)

# S3

Simple Storage Service, shortened to S3, is one of the oldest services in AWS. S3 stores objects, whatever they may be, and allows you to easily configure who can see them. S3 stores your objects in whichever region you select, which can be important for legal or regulatory reasons. In S3, objects are the fundamental storage structure. An object is basically a file and metadata.

The metadata is used by S3 and includes things like file type and modified date, as well as any custom metadata added. S3 doesn't care what type of object it is, and the maximum file size limit is essentially a joke except in the most extraordinary circumstances.


# What is S3 ?
=================================
# S3 stands for Simple Storage Service.
It provides object storage through a web service interface.
*Each object is stored as a file with its metadata included and is given an ID number.
Objects uploaded to S3 are stored in containers called “Buckets”, whose names are “unique” and they organize the Amazon S3 namespace at the highest level.
These buckets are region specific.
You can assign permissions to these buckets, in order to provide access or restrict data transaction.
Applications use this ID number to access an object.
Developers can access an object via a REST API.
Supports upload of objects.
Uses the same scalable storage infrastructure that Amazon.com uses to run its global e-commerce network.
Designed for storing online backup and archiving of data and applications on AWS.
Its mainly designed with the minimal features that can easily set and also to create the web-scale computing in an easy way.

Storage classes provided are:
=================================

Standard
Standard_IA i.e., Standard Infrequent Access
Intelligent_Tiering
OneZone_IA
Glacier
Deep_Archive

RRS i.e., Reduced Redundancy Storage (Not recommended by AWS)
Data access is provided through S3 Console which is a simple web-based interface.
Data stored can be either Public or Private based on user requirement.
Data stored can be encrypted.
We can define life-cycle policies which can help in automation of data transfer, retention and deletion.
Amazon Athena can be used to "query" S3 data as per demand.


# AWS CloudFront

CloudFormation is a tool offered by Amazon to use configuration data to create and configure resources in AWS. Almost any AWS resource can be created using CloudFormation, from a security group to an EC2 Auto Scaling group. CloudFormation allows you to perfectly create groups of resources over and over again due to the static nature of the templates used to create those resources.

The key tool in CloudFormation is a template. A CloudFormation template is just a JSON document that contains the configuration information for AWS resources and how they relate. You can create this template document as a file and check it into version control to track changes to your infrastructure and make it easy to roll back if needed. These templates can often be massive documents when you have a large amount of infrastructure to create. 

# AWS Lambda

AWS Lambda is a way to run code without creating, managing, or paying for servers. You supply AWS with the code required to run your function, and you pay for the time AWS runs it.Your code can access any other AWS service or it can run on its own. While there are some rules about how long a function has to respond to a request, there’s almost no limit to what your Lambda can do.AWS will scale your code for you, depending on the number of requests it receives. 

# API Gateway

Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.

API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, CORS support, authorization and access control, throttling, monitoring, and API version management. API Gateway has no minimum fees or startup costs. You pay for the API calls you receive and the amount of data transferred out and, with the API Gateway tiered pricing model, you can reduce your cost as your API usage scales.

# DynamoDB

Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multiregion, multimaster, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications.

# AWS Cognito

Amazon Cognito lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily. Amazon Cognito scales to millions of users and supports sign-in with social identity providers, such as Facebook, Google, and Amazon, and enterprise identity providers via SAML 2.0.

