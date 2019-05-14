## Differences between Traditional and Cloud Computing Environments

* IT assets as Provisioned resources
* Global, available and scalable capacity
* Higher level Managed Services
* Built-in Security
* Architecting for Cost
* Operations on AWS
  * Migrations
  * Solutions Refactored
  * Solution rearchitected

## Design Principles

* **Scalability**
  * Scalling Vertically: Increase capacity of individual resource
  * Scalling horizontally: Increase the number of resources
* **Stateless Applications**: one interaction one session, this kind of applications can grow horizontally without problems.
* **Distribute Load to Multiple Nodes**: 
  * Push model: Elastic Load Balancing
  * Pull model: Event driven workload using SQS or streaming solutions
* **Stateless Components**: Deal with session information saving it on client site or browser and in case of use server side use DynamoDB for it. In case of large files storage needed use S3 or EFS.
* **Stateful Components**: For state components the way to achieve an horizontal scalling is adding load balancing with session affinity among different nodes.
* **Implement Session Affinity**: Use sticky sessions features of an Application Load balancer to bind user's session to a specific instance. 
* **Distributed Processing**: For very large amount of data processing it's a good practice divide the task into small chunks of data that can be distributed into different instances. 
* **Implement Distributed Processing**: Offline batch jobs can be horizontally scaled using distributed data processing engines such as AWS batch, AWS Glue or apache hadoop.

## Disposable Resources Instead of Fixed Servers

In Aws you have the freedom to work with the machines that you need dynamically. There are some recommendations to be applied to instanciated Compute Resources:

**Bootstrapping**: When a resource is launched it starts with the default configuration, you can execute your own bootstrapping actions which are scripts that install software or copy data to bring that resource to a particular state. 

**Golden Images**: Certain resources such us EC2, RDS and EBS can be launched from a golden image whic is a snapshot of a particular state of that resource. 

**Containers** Another popular option is Docker. Docker allows you to package a piece of software in a Docker image that helps you to instanciate containers across a cluster of EC2 instances.

**Hybrid**: You are able to combine the different approaches.

## Infraestructure as a Code

AWS allows to define your assests at code level. Cloud formation templates gives you the possibility to create and manage, provision and update a collection of resources using an orderly and predictable fashion using programatically tools. 

## Automation

Consider to introduce different kind of automation into your application architecture to ensure more resiliency, scalability and performance. The different options are:

**Serverless Management and Deployment** AWS CodePipeline, CodeBuild and CodeDeploy will help you to automate you serverless deployments

**Infraestructure Management and Deployment** Elastic Beanstalk will help to deploy your application without and worries about the underlaying insfraestructure.  EC2 autorecovery will help you to monitor instances and automatically recover them.

## Alarms and Events

CloudWatch is the main service for alarms. CloudWatch sends message using SNS

## Loose Coupling

When the complexity increasesis desirable that the whole architecture can be splitted into small pieces loosely coupled. In order to achieve this wen need:

**Well defined interfaces**: interaction between component using agnostic interfaces like RESTful APIs.

**Amazon API Gateway** it will help to create, publish manage and monitor APIs. 

## Service Discovery

Thinking on a microservice environment is fundamental that the service can be discoverabled by other services. The simplest way to do this can be with a EC2 instance that has a record of services combined with DNS and private Route 53 zones. 

Other option is to use a service registration and discovery method to allow retrieval of the endpoint IP addresses and port number for any service. 

## Asynchronous Integration

This is another form of loose coupling between services. Instead of chain calls to different services we add a new layer in the middle to break the coupling between services. This layer can be implemented using Amazon SQS, Kinesis, step functions or lambdas fired by specific events.

## Distributed System Best Practices

It is very important to manage the failure of a component in a graceful manner. The use of services like Route 53 DNS failover feature will help you to monitor service failure. 

## Serverless Architecture

Serverless architectures can reduce the operational complexity of running applications. It is possible to build both event-driven and synchronous services for mobile, web, analytics, CDN business logic, and IoT without managing any server infrastructure. These architectures can reduce costs because you don’t have to manage or pay for underutilized servers, or provision redundant infrastructure to implement high availability. 

## Databases

With traditional IT infrastructure, organizations are often limited to the database and storage technologies they can use. There can be constraints based on licensing costs and the ability to support diverse database engines. On AWS, these constraints are removed by managed database services that offer enterprise performance at opensource cost. As a result, it is not uncommon for applications to run on top of a polyglot data layer choosing the right technology for each workload.

* Relational Databases
* NoSQL Databases
* Data Warehouse
* Search
* Graph Databases

## Managing increasing Volume of Data

Traditional data storage and analytics tools can no longer provide the agility and flexibility required to deliver relevant business insights. That’s why many organizations are shifting to a data lake architecture. A data lake is an architectural approach that allows you to store massive amounts of data in a central location so that it's readily available to be categorized, processed, analyzed, and consumed by diverse groups within your organization. 

##Removing Single Points of Failure

Production systems typically come with defined or implicit objectives for uptime. A system is highly available when it can withstand the failure of an individual component or multiple components, such as hard disks, servers, and network links. To help you create a system with high availability, you can think about ways to automate recovery and reduce disruption at every layer of your architecture. THis can be achieved by:

* Introduce redundancy
* Detect Failure

## Durable Data Storage

Your application and your users will create and maintain a variety of data. It is crucial that your architecture protects both data availability and integrity. Data replication is the technique that introduces redundant copies of data. It can help horizontally scale read capacity, but it also increases data durability and availability. Replication can occur in a few different modes.

* Synchronous replication
* Asynchronous replication
* Automated Multi-Data center Resilience
* Fault Isolation and Traditional Horizontal Scaling

## Optimize For Cost

When you move your existing architectures into the cloud, you can reduce capital expenses and drive savings as a result of the AWS economies of scale. By iterating and using more AWS capabilities, you can realize further opportunity to create cost optimized cloud architectures. 

* Right Size
* Elasticity
* Take advantage of variety of purchase options

## Caching

Caching is a technique that stores previously calculated data for future use. This technique is used to improve application performance and increase the cost efficiency of an implementation. It can be applied at multiple layers of an IT architecture.

* Application Data Caching
* Edge Caching

## Security

Most of the security tools and techniques that you might already be familiar with in a traditional IT infrastructure can be used in the cloud. At the same time, AWS allows you to improve your security in a variety of ways. AWS is a platform that allows you to formalize the design of security controls in the platform itself. It simplifies system use for administrators and your IT department, and makes your environment much easier to audit in a continuous manner.

* Use AWS features for Defense in Depth like WAF
* Share Security Responsibility model
* Reduce Privileged access
* Security as code using cloud front templates for example
* Real-Time Auditing