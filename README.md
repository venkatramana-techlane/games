# Games
Storing the details about the Games played by the participants and scores earned.

# Architecture

![](images/AWS%20Architectture.PNG)

# S3 
- S3 stands for Simple Storage Service.
- It provides object storage through a web service interface.
- Each object is stored as a file with its metadata included and is given an ID number.
- Objects uploaded to S3 are stored in containers called “Buckets”, whose names are “unique” and they organize the Amazon S3 namespace at the highest level.
- These buckets are region specific.
-  can assign permissions to these buckets, in order to provide access or restrict data transaction.
- Applications use this ID number to access an object.
- Developers can access an object via a REST API.
- Supports upload of objects.
- Uses the same scalable storage infrastructure that Amazon.com uses to run its global e-commerce network.
- Designed for storing online backup and archiving of data and applications on AWS.
- Its mainly designed with the minimal features that can easily set and also to create the web-scale computing in an easy way.

Storage classes provided :
1. Standard
2. Standard_IA i.e., Standard Infrequent Access
3. Intelligent_Tiering
4. OneZone_IA
5. Glacier
6. Deep_Archive

- RRS i.e., Reduced Redundancy Storage (Not recommended by AWS)
- Data access is provided through S3 Console which is a simple web-based interface.
- Data stored can be either Public or Private based on user requirement.
- Data stored can be encrypted.
- We can define life-cycle policies which can help in automation of data transfer, retention and deletion.
- Amazon Athena can be used to "query" S3 data as per demand.


# AWS CloudFront
- Amazon CloudFront is a content delivery network (CDN) offered by AWS.
- CDN provide globally-distributed network of proxy servers which cache content, i.e., web videos or other bulky media, more locally to consumers, thus improving access speed for downloading the content.
- CloudFront service works on pay-as-you-go basis.
- CloudFront works with origin server i.e., S3, EC2 where the content is stored, and is pushed out to multiple CloudFront servers as content is requested.
- When CloudFront is enabled, the content is stored on the main S3 server.
- Copies of this content are created on a network of servers around the world called CDN.
- Each server within this network is called an Edge server, which will only have a copy of your content.
- When a request is made to the content, user is provided from the nearest edge server.
- CloudFront has features similar to dynamic site acceleration, a method used to improve online content delivery.
- CloudFront accelerates the delivery of dynamic content by moving it closer to the user to minimize internet hops involved in retrieving the content.
- CloudFront's Web distribution support "Progressive" download i.e., data from S3 is cached and then streamed without disruptions.
- Due to this the user cannot move front or back in the video i.e., the video is processed bit by bit.
- CloudFront's Web distribution support "Streaming" i.e., it allows users to directly watch without any download.
- Due to this the user can move front or back in the video, and the latency is very less i.e., the latency is based on the size of the file and the customer Internet bandwidth.
- This service is beneficial for those developing a website that distributes a lot of content that needs to scale-up.
-   It helps reduce costs and improve the performance of a website by providing high data transfer speeds, low latency

# AWS Lambda
1.	AWS Lambda service allows you to run code without provisioning or managing dedicated servers. 
2.	In other words, Lambda will be called Serverless Computing.
3.	The interesting feature about lambda is you only need to pay for the compute time you consume and no need to pay when your code is not running.
4.	you can run code for virtually any type of application with zero administration with the help of AWS Lambda functions.
5.	Just upload your code to Lambda and it will take care of everything required to run and scale your code with high availability
6.	We can set triggering events for our lambda function when to run or when to get triggered.
7.	Lambda currently supports various languages such as java, python, node js, c, etc using which you can write your lambda function.


# API Gateway
- Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. 
- APIs act as the front door for applications to access data, business logic, or functionality from your backend services. 
- API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, CORS support, authorization and access control, throttling, monitoring, and API version management. 
- Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.      
- AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume.
- With Lambda, you can run code for virtually any type of application or backend service - all with zero administration. Just upload your code and Lambda takes care of everything required to run and scale your code with high availability. You can set up your code to automatically trigger from other AWS services or call it directly from any web or mobile app.    


# DynamoDB
- DynamoDB is fast and flexible NoSQL database and it's for applications that need consistent single digit millisecond latency at any scale.And it's a fully managed database and it supports both document and key value data models.
- It has a really flexible data model.So that means that you don't need to define your database schema upfront and it has really reliable performance as well.
- And all of these attributes make it a really good fit for mobile gaming, ad-tech, IoT and many other applications.
DynamoDB Tables:
DynamoDB tables consist of 
1. Item (Think of a row of data in a table).
2. Attributes ((Think of a column of data in a table).
3. Supports key-value and document data structures.
4. Key= the name of the data.  Value= the data itself.
5. Document can be written in JSON, HTML or XML.
DynamoDB- Primary Keys:
- DynamoDB stores and retrieve data based on Primary key
- There are 2 types of Primary Key. Partition Key - Unique attribute
- Value of the partition key is input to an internal hash function which determines the partition or physical location of which the data is stored.
- If you are using the partition key as your Primary key, then no items have the same Partition key.
- Composite Keys (Partition Key + Sort Key) in Combination.
- 2 items may have same partition key but they must have a different sort key.
- All items with the same partition key are stored together, then sorted according to the sort key value.
- Allows you to store multiple items with the same partition keys.

