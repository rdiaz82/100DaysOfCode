## Cloud Concepts and Technology

* Cloud computer is on-demand delivery of computer under a as pay as you go pricing model

* The 6 advantages of clouf computer are:

  1. Trade capital expense for variable expense (avoid high invesment in data center).

  2. Benefice from massive economies of scale, amazon build it own servers.
  3. Stop guessing about capacity: You use much power as you need.
  4. Increase your speed and agility. 
  5. Stop spending money maintaining data centers
  6. Go global in minutes!!

* Types of cloud computer

  1. **Infraestructure as a service** (AWS)
  2. **Platform as a services**: (GoDaddy) just upload your content and they manager the underlying hardware also Beanstalk is a good example
  3. **Software as a Service** (Lamda)

* Type of cloud computer deploying

  1. Public cloud: AWS, Azure...
  2. Hybrid mixture between public and private
  3. Private cloud, you manage your data center

* services included in the Cloud Practitioner Certification

  * AWS global infraestructure
  * Network
    * VPC
    * Route53
  * Compute
    * EC2
    * Lambda
  * Storage
    * S3
    * Glacier
  * Database
    * RDS
    * DynamoDB
  * Security
  * AWS Cost Management

## Around the World With AWS

*  **19 regions and 57 availabilty zones**
* in 2019 there will be added 5 more regions and 15 more availability zones
* **Availability zone = Data center**, in fact the could be formed by several data center but they are considered as only one AZ
* a Region is a geographical zone and is composed by two or more availability zones.
* GovCloud zone is used by US goverment and it can be used just for governamental applications with a lot of restrictions. 
* **Edge location** are endpoints for AWS which **are used for caching content**. Typically this consists of CloudFront, Amazon's Content delivery Network (CDN)
* Currently there are more Edge location than Regions, more than 150 Edge locations!

## Let's Log In To AWS-Lab

* Create an Account with a one year free tier with a lot of services included!
* The four levels for support are availabe at sign up process:
  * **Basic**: Comunnity forums
  * **Developer**: Support center response 12-24h (29$/month)
  * **Business**: 24x7 phone and 1 hour response (100$/month)
  * **Enterprise**: One Technical account manager and 15 minute response (15000$/month)
* N. Virginia is the oldest Region and all services all publish first in this region.
* The first task in the account should be use **CloudWatch** and enable to receive email if your free tier is near to reach its limit. 
* Also it is recomendable to create a billing alarm if your spent money reach 10$

## Let's Start to Cloud! Identity Access Management (IAM) 

* AIM allows to create users and groups
* The IAM is global so the configuration are not attached to any specifi region. 
* All the users can interact with AWS services in three different ways:
  1. Via the AWS Console
  2. Programatically using the comand line client
  3. Using SDKs
* Groups are simply a place to store your users with common permissions
* The root account is the email used to create the account but normally all user should have it own user and the root account should be used just for administration. 
* Virtual MFA device will use Google Authenticator to enable multi factor authentication for root user. 
* the sign in for user alias can be customized.
* For users there are two types of access:
  * Programmatic access: Enable access keyID and secret for the AWS API, CLI etc...
  * AWS Management Console access: Enable a password to access to AWS managmeent console.
* For permission management we have three different options:
  * Add user to an existing group
  * Copy permission from another user
  * Attach the permission policy as Json
* Amazon provides a lot of predesigned User groups that can be used as templates for your own groups. 
* User can also have some custom key/value tags to add your own information like department,
* Under of IAM you can define also your users password policy, type of characters, length, force password rotation, etc...

## S3 101

* S3 is Simple Storage Service, is one of the most old AWS services, released in 2006.
* The AWS definition: S3 provides developers and IT teams with secure, durable, highly-scalable object storage. Amazon S3 is easy to use with a simple web interface to store and retrieve any amount of data from anywhere on the web.
* S3 is a place to storage all your flat file videos, images, etc..
* S3 is object based, so you can install a SO on it. 
* The data are spread accross multiple devices and multiple facilities.
* the maxim file size is 5TB
* Files are storaged in Buckets, just a folder in the cloud. 
* The S3 is a universal namespace, so everytime you create a bucket, it name have to be unique globally. 
* The S3 url has this format: https://S3-zone.amazonaws.com/your_bucket
* When you upload a file to S3 you will receive a HTTP 200 code if the upload was successful
* S3 is a object based storage with the following information:
  1. Key: filename
  2. Value: Actual data converted into a sequence of bytes
  3. Version Id: Important for versioning
  4. Metadata: additional info about the file
  5. Subresources: **Find more info about this!!**
     1. Access Control List
     2. Torrent
* Data consistency in S3:
  * Read after Write consistency for PUTS of new objects
  * Eventual consistency for overwrite PUTS and DELETE (it can take some time to propagate). If you update and read you can get the old file because of propagation. 
* S3 is guarantied for 99.99% for S3
* Amazon garantee 99.9% of availabity
* S3 durability is 99.999999999% (11s 9)
* Tiered Storage Available
* LifeCycle Management you can decide what to do with yourfile after a time
* File Versioning
* Encryptation
* Secure data using Access Control List and Bucket Policies
* S3 Storage Classes
  1. S3 Standard: 99.9% availability 11 9's % durability, redundant across multiple devices in multiples facilities and disegnid to sustain the loss of two facilities zoncurrently
  2. S3-IA (Infrequently accessed). For data that are accessed less frequently but with rapid access when needed. Charged for retrieval fee. 
  3. S3 One-zone-IA. Lower cost option for infrequently access data without multiple Availability zones.
  4. S3 - Intelligent Tiering: Designed to optimise your cost automatically moving data 
  5. S3 Glacier: Secure, durable and low cost storage for data archiving. Retrieval time from minute to hours
  6. S3 Glacier Deep Archive: lowest cost with retrieval time of 12 hours.
* Your are chaged in the following ways:
  1. Storage
  2. Requests
  3. Storage Management pricing
  4. Data transfer pricing
  5. Transfer Acceleration
  6. Cross Region Replication pricing
* Transfer acceleration enable fast, easy and secure transfers of files over long distances between end users and S3 bucket. Transfer Acceleration takes advantages of Amazon CloudFront's globally distributed edge locations. As the data arrives at an edge location, data is routed to Amazon S3 over an optimized network path. 
* Cross Regions Replication allows you to have two buckets syncronized between different zones. 

## Let's create a S3 bucket!

* When you see your buckets on the console you are view them globally but  you can have buckets in individual regions.
* The bucket name should be DNS compliant.
* By default all bucket are protected so we need to disable protection to read/write
* Anything hosted on S3 is not public, so you need to specify the file to be public
* You can change your object properties on the fly.

## Let's create a Website static

* upload you content to the bucket
* Enable web hosting
* add a bucket policy to make all files publics
* Edit public access is disable by default so if you try to change the policy you get an error. You have to go to bucket option and disble this protection.
* S3 automatically scale accord with your demand and you can support high traffic using static websites. 

## Let's explore Cloud Front

* Cloud front is a content delivery network or CDN. is a system of distributed servers that deliver webpages and other web content based on the geographic location of the user, the origin of the webpage and a content delivery server.
* Edge locations. This is the location where the content can be cached. Separated from regions and Availability zones
* Origin: This is the origin of all files that the CDN will distribute (S3, EC2, elastic load balancer, route 53)
* Distribution: This is the name given the CDN which consists of a collection of edge locations.
* The normal operation is the following.
  1. A first user request a file to a edge location.
  2. if the edge location doesn't include the file, it is downloaded from the origin
  3. if another user using the same edge location ask for the same file, that user will receive the cache copy from the edge location. 
* Cloud Front support the following delivery technologies
  1. We distribution
  2. Real Time Multimedia protocol (RMTP)
* In AWS console Cloud Front is under networking. 
* Edge locations are not just Read only, you can put objects on to them.
* TTL time to live of cached file

## EC2 101

* Elastic Compute clous is just a virtual server/server in the cloud
* It reduces the time to obtain and boot new servers instances to minutes allowing you to quickly scale your capacity according to your requeriments.
* Pricing models:
  1. On demand: allows you to pay a fix rate by the time of use
     * Useful for low cost and flexibility without long term use
     * Application with hirt term, spiky or unpredictable work loads
     * Development
  2. Reserved: provides you a capacity reservation and offer a significant discount compared with On demand instances. Normally you have to sign a 1 year of 3 years contract.
     * Applications with steady setate or predictable use
     * applications that require reserved capacity
     * Upfront payment to reduce long term costs
     * Reserved price model:
       1. Standard:75% off more you pay up front and long term more discount.
       2. Convertible: 54% and allow you to change the attributes of the reserve instance. 
       3. Schedule reserve: Launch instances in a time window.
  3. Spot: Enable you to bid whatever price you want to pay for your computation capacity. it offer grater saving if your application have flexible start and stop times. 
     * Allow compute a low prices
  4. Dedicated hosts. Physical EC2 server dedicated for your use. It will help you to reduce cost by allowing you to use your existing server-bound software licenses.
     * Useful for regulatory requirements
     * great for licensing that not support multi tenancy
     * if a Spot instance is terminated by EC2 you will not pay for a partial hour of usage. However if you terminate the instance yourself you will be charged for any hour in which the instance ran.
* Amazon EBS allows you to create storage volumes and attach them to ECs instances. Once attached, you can create a file system on top these volumes, run database or use them in any other way you would use a block device. EBS volumes are places in a specific availability zone replicated.
* EBS types:
  1. SSD General purpose
  2. provisiones IOPS SSD
  3. Magnetic Throughput HHD (frequent access)
  4. Cold HHD
  5. Magnetic

## Let's use EC2

* EC2 is a region service you have your instances in one regions
* When you launch a new instane you have to select the AMI
* After this you have to select type of instance
* After EC2 configuration you have to add EBS
* The instance can have some tags 
* Finally you have to define your security group for that particular instance
* To allow accessfrom everywhere the security group should have 0.0.0.0/0 as source for each interest protocol ports
* The last part of the instance creation is the creation or selection of a key pair
* To connect using ssh you shoudl use `ssh ec2-user@instace.ip -i your_key.pem`

## Using The Command Line

* you have to download your private access key in csv format
* the command line can interact with AWS services
* The access to command line can be done by roles or by user

## Using Roles

* IAM inside console
* Select the service to be applied the role
* We need to add a policy to the role
* simple add name and tags
* Once the role is created you can attach the role to an EC2 instance for example.
* The good part of roles is that your credentials are not stored inside the instance.

##Let's build a Web server

* Create EC2 instance
* install apache with yum 
* start apache service
* put your content on /var/www/html

## Let's use a load balancer

* Application Load Balancer is good for applications
* Network load balancer is for high performance and static ip adresses
* Classic Load Balancer is for older services
* Select http port 80 and all availability zones
* use the security group webDMZ
* Select the target group and your ec2 application instances
* you can add your own script to run at ec2 boot using user data when you configure your instance

## Databases 101

* Relational database is AWS-RDS (OLTP)
  * SQL Server
  * Oracle
  * PostgreSQL
  * MySql server
  * Aurora
  * MariaDb
* Multiple Availability Zones for disaster
* Read Replicas to improve performance up to 5 copies
* Non relational database DynamoDb
* Data warehousing database: Redshift (OLAP)
* ElasticCache is a web service that maskes ir easy to deploy, operate and scale in-memory cache in the cloud. ElastiCache support two caching engines:
  * memcached
  * redis

## Let's provision an RDS instance

* Provision RDS
* Provision an Aplication LoadBalancer
* Create a target group
* create an EC2 instance
* Register the instance to the target group
* Open MySQL port to Web-DMZ
* Connect to DNS name to load balancer
* Install your app

## Autoscaling

* Create a launch configuration first to configure the ec2 instances created for the autoscaling group.
* Then simply create the autoscaling group attached to the automatic load balancer

## Let's register a domain name

* Route 53 is the place to management all the things related with DNSs

## Let's look at Elastic Beanstalk

* will provision all the infraestructure to run automatically an application just uploading your code and forgetting about the infraestructure under the curtains

## Let's look at Cloudformation

* Is a tool that allows you to design an aws architecture directly from code. 
* The templates are written in son or yams and they describe a complete stack for run your applications.
* From templates you only need to define the different parameters to run your application like instances types, database configuration etc...

## Architecting for the cloud

