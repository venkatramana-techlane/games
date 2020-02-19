# Games
Storing the details about the Games played by the participants and scores earned.

# Architecture

![](images/AWS%20Architectture.PNG)

# S3

Simple Storage Service, shortened to S3, is one of the oldest services in AWS. S3 stores objects, whatever they may be, and allows you to easily configure who can see them. S3 stores your objects in whichever region you select, which can be important for legal or regulatory reasons. In S3, objects are the fundamental storage structure. An object is basically a file and metadata.

The metadata is used by S3 and includes things like file type and modified date, as well as any custom metadata added. S3 doesn't care what type of object it is, and the maximum file size limit is essentially a joke except in the most extraordinary circumstances.


# AWS CloudFront

CloudFormation is a tool offered by Amazon to use configuration data to create and configure resources in AWS. Almost any AWS resource can be created using CloudFormation, from a security group to an EC2 Auto Scaling group. CloudFormation allows you to perfectly create groups of resources over and over again due to the static nature of the templates used to create those resources.

The key tool in CloudFormation is a template. A CloudFormation template is just a JSON document that contains the configuration information for AWS resources and how they relate. You can create this template document as a file and check it into version control to track changes to your infrastructure and make it easy to roll back if needed. These templates can often be massive documents when you have a large amount of infrastructure to create. 

# AWS Lambda

# API Gateway

# DynamoDB

# AWS Cognito

