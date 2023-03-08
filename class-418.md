# 418

## AWS API Gateway Overview

- What is Amazon API Gateway?  
Amazon API Gateway is a fully managed service provided by Amazon Web Services (AWS) that enables developers to create, deploy, and manage APIs (Application Programming Interfaces) at any scale.

- Why is Amazon API Gateway an important part of the Serverless ecosystem?  
Amazon API Gateway is an important part of the Serverless ecosystem because it enables developers to build serverless applications that can be accessed through RESTful APIs.

- How does API Gateway integrate with other AWS services?  
AWS Lambda: API Gateway can be used to trigger Lambda functions in response to incoming requests.

**Amazon S3**: API Gateway can be used to create RESTful APIs that expose S3 objects.**Amazon DynamoDB**: API Gateway can be used to create APIs that allow users to perform CRUD (Create, Read, Update, Delete) operations on DynamoDB tables. **AWS IAM**: API Gateway can be integrated with IAM to control access to APIs at the user and role level. **AWS CloudTrail**: API Gateway can be configured to log all API calls to CloudTrail, which can be used for auditing and compliance purposes.

## AWS API Gateway

- What are the some benefits of using Amazon API Gateway?  
Scalability, cost-Effective, security, integration with other AWS services, API Versioning, caching, and API Monitoring.

- What two API types might you choose from?  
REST APIs and WebSocket APIs

## AWS DynamoDB Guide

- What is DynamoDB?  
DynamoDB is a fully managed NoSQL database service provided by Amazon Web Services.

- Under what circumstances would you recommend DynamoDB over MongoDB?  
When you need a fully managed service, when you need high availability and scalability, when you need low latency, and when you need predictable pricing.

## AWS DynamoDB

- Explain to a non-technical friend how DynamoDB works.  
DynamoDB is a database service provided by AWS that allows you to store and retrieve data in a way that is fast, reliable, and scalable. DynamoDB is designed to be "serverless", which means that you don't have to worry about setting up and managing the infrastructure that runs the database. DynamoDB is also a NoSQL database. This means it uses a key-value store, which allows you to store and retrieve data using a unique identifier, or key.

## Dynamoose

- What is Dynamoose?  
Dynamoose is a modeling tool and object data modeling (ODM) library for Amazon Web Services' DynamoDB NoSQL database.

- What are some key features of Dynamoose?  
Simple and intuitive syntax, validation and type checking, middleware support, querying and pagination, support for transactions, and promise-based API.
