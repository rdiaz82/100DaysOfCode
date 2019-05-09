## Six Advantages of Cloud Computing

* Trade capital expenses for variable expeneses
* Benefit from massive economies of scale
* Stop guessing capacity
* Increase speed and agility
* Stop spending money running and mainting data centers
* Global in minutes

## Types of Cloud Computing

* Infrastructure as a service
* Platform as a service
* Software as a service

## Types of Deployment models

* Cloud
* Hybrid
* On-premises

## Global infraestructure

Each Amazon Region is designed to be completely isolated from the other Amazon Regions. This achieves the greatest possible fault tolerance and stability. EachAvailability Zone is isolated, but the Availability Zones in a Region are connected through low-latency links. AWS provides you with the flexibility to place instances and
store data within multiple geographic regions as well as across multiple Availability Zones within each AWS Region. Each Availability Zone is designed as an independent failure zone. This means that Availability Zones are physically separated within a
typical metropolitan region and are located in lower risk flood plains (specific flood zone categorization varies by AWS Region). In addition to discrete uninterruptable power supply (UPS) and onsite backup generation facilities, they are each fed via different grids from independent utilities to further reduce single points of failure. Availability Zones are all redundantly connected to multiple tier-1 transit providers.

## Security

The AWS Cloud enables a shared responsibility model. While AWS manages security of the cloud, you are responsible for security in the cloud. This means that you retain control of the security you choose to implement to protect your own content, platform, applications, systems, and networks no differently than you would in an onsite data center.

The main benefits of AWS security model are the following:

* Keep your data safe
* Meet Compliance Requirements
* Save Money
* Scale Quickly

## AWS Cloud platform

Different type of access:

* AWS managmeent console
* AWS command Line Interface
* Software Development kits

### Analytics

**Athena**: interactive query service for S3 using SQL queries

**Amazon EMR** provides a managed Hadoop framework to process data using EC2 instances

**Amazon CloudSearch** managed service to set up and manage search solutions for applications. 

**Amazon ElasticSearch** makes it easy deploy, secure, operate and scale ElasticSearch to search, analyze and visualize data in real time. 

**Amazon Kinesis** allows to collect, process and analyze real time stream data.

**Amazon Kinesis Data Firehose** the easiest way to load data from streams into store and analytics tools.

**Amazon Kinesis Data Analytics** the easiest way to analyze a data stream using SQL queries. 

**Amazon Kinesis Data Streams (KDS)** massive and scalable realtime streaming service. It can capture gigabytes of data per second. 

**Amazon Kinesis Video Streams** makes easy video stream processing for analytics, machine learning or playback.

**Amazon RedShift** is a scalabel data warehouse that makes easy analize data across data warehouse and data lake

**Amazon QuickSight** Cloud-powered business intelligence servide.

**AWS Data pipeline** is a service that allows to process and move data between different AWS services

**AWS Glue** Its a fully managed extract, transform and load service that makes it easy for customer to prepare and load their data for analytics. 

**AWS lake formation** allows to set up a secure data lake in a centralized way. 

**AWS streaming for Kafka** fully managed services that makes easy build and run applications that uses apache kafka

## Application Integration

**AWS step functions** lets you coordinate mutiple aws services into a serverless workflow.

**Amazon MQ** is a managed message broker service for apache ActiveMQ.

**AmazonSQS** (simple Queue) service is a fully managed message queuing service that enables you to decouple and scale microservices. 

**Amazon SNS** (simple notification service) is a highly available, durable and secure fully managed pub/sub messaging service.

**Amazon SWF** (simple workflow) helps developers to build run and scale background jobs that have parallel or sequential steps. 

## AR and VR

**Amazon Sumerian** Let you create and run virtual, augmented and 3d applications quickly and easy without needed of 3d experts

## AWS Cost Management

**AWS Cost Explorer** easy interface to understand, visualize and manage your AWS costs over time

**AWS budgets** gives you the ability to set custom budgets that alert you when costs or usage exceed your budgeted amount. 

**AWS Cost & Usage Report** a single localization for accessing comprehensive information about your AWS costs and usage. 

**Reserve Instance Reporting** The same as AWS cost explorer focused on reserved instances. 

## Blockchain

**Amazon managed Blockchain** fully managed service that makes easy create and manage scalable blockchains networks.

## Business Applications

**Alexa for Business** enables organizations and employeed to use Alexa to get more work done. 

**Amazon WorkDocs** fully managed secure entreprise storage and sharing service. 

**Amazon WorkMail** is a secure managed business mail and calendar service with support for existing desktop and mobile email clients. 

**Amazon Chime** is a communications service that allows you to manage online meetings

## Compute

**Amazon EC2** is a web service that provides secure resizable compute camacity in the cloud. It is designed to make web-scale computing easier for developer.

Instance types:

* On-demand: you pay for compute capacity by the hour with no long-term commitments. 
* Reserved instances: provide you with a significant discount (up to 75%) compared to On-demand instances. 
* Spot: allow you to bid on space Amazon EC2 computing capacity

**Amazon autoscaling** heps you to maintain applications availability and allows you to automatically add or remove EC2 instances according to conditions you define. 

**Amazon Elastic Container Register** is a fully managed Docker container registry that makes it easy for developers to storage manage and deploy docker container images. 

**Amazon Elastic Container Service** is a highly scalable, high-performance container orchestration service that supports Docker containers and allows you to easyly run containerized applications on AWS.

**Amazon Elastic container service for Kubernetes** makes it easy yo deploy, manage and scale containerized applications using kubernetes on AWS. 

**Amazon LightSail** is designed to launch, manage a virtual private server on AWS.

**AWS Batch** Enable developers, scientists and engineer to easily run hundred of thousands of batch computing jobs on AWS. 

**AWS Elastic Beanstalk** easy-to-use service for deploying and scaling web applications and services using different languages like Java, .net, php, node, python, ruby, go.

**AWS Fargate** Allows to run containers without having to manage servers or clusters. 

**AWS lambda** lets you run code without provisioning or managing servers. You pay only for compute time you consume

**AWS serverless application repository** enables you to quickly deploy code samples, components ans complete applications for common uses cases such as web and mobile back-ends.

**AWS Outposts** brings native aws services, infraestructure and models to virtually and and data center, co-location space or on premises facility. 

**Vmware Cloud on AWS** is an integrated cloud offering jointly developed by AWS and VMware delivering VMware solutions on AWS.

## Customer Engagement

**Amazon Connect** self service cloud based contact center service that makes it easy for any business to deliver a better customer service at lower cost.

**Amazon SES** Simple email service is a cloud based email sending service designed to help digital marketers and applications debelopers send marketing notifications.

## Database

**Amazon Aurora** is a MySQL and PostgresSQL compatible relational database engine that combines the speed and availability of high-end commercial database with the simplicity and cost-effectiveness of open source

**Amazon RDS** makes it easy to set up, operate and scale a relational database in the cloud.

**Amazon RDS on VMware** lets you deploy managed database on premises VMware environments. 

**Amazon DynamoDB** is a key-value and document database. 

**Amazon ElasticCache** is a web service that makes it easy to deploy operate and scale an in-memory cache in the cloud. It has support for Redis  and Memcached. 

**Amazon Neptune** is a fully managed graph database service.

**Amazon Quantum Ledger Database** fully managed ledger database that provides a transparent immutable and cryptographically verifiable transaction log owned by a central trusted authority. 

**Amazon TimeStream** fully managed time series database services for IoT and operationsl applications that makes easy to store and analyse trillios of events per day at 1/10th the cost of a relational database. 

## Desktop and App Streaming

**Amazon workspaces** secure cloud desktop service that allows to provisioning either windoes or linux desktops. 

**Amazon AppStream 2.0** fully managed application streamin service. You centrally manage your desktop application en AppStream 2.0 an securely deliver them to any computer. 

## Developer Tools

**AWS CodeCommit** Aws github clone

**AWS CodeBuild** service that compiles source code, run tests and produce software package ready for production. 

**AWS CodeDeploy** Service that automated code deployments to any instance including ECS2 instance and instances running on premises. 

**AWS CodePipeline** continious delivery service to automate release pipeline.

**AWS CodeStar** is a unified user interface to configure your continious delivery system. 

**Amazon Corretto** AWS distribution of the JDK based on OpenJDK

**AWS Cloud9** cloud based IDE that lets you write run and debug your code just in a browser. 

**AWS X-Ray** helps developers to analyze and debug distributed applications in production or under development in a micro service architecture. 

## Game Tech

**Amazon GameLift** service for deploying, operating and scaling game servers for session-based multiplayer games. 

**Amazon Lumberyard** is a free, cost-platform, 3D game engine for you to create highest-quality games. 

## Internet of Things (IoT)

**AWS IoT Core** managed cloud service that lets connected device easily and securely interact with cloud applications and other devices. 

**Amazon FreeRTOS** is a real time operative system for microcontrollers. 

**AWS IoT GreenGrass** allows to run AWS services locally on IoT devices for instance AWS lambda or machine learning models. 

**AWS IoT 1-Click** enables simple devices to trigger AWS lambda functions 

**AWS IoT Analytics** fully managed service that makes it easy to run and operationalize analytics on massive volume of IoT Data. 

**AWS IoT Button** programmable button based on the Amazon Dash Button.

**IoT Device Defender** is a service that helps you secure your fleet of IoT devices. 

**AWS IoT Device Management** allows you to organise, monitor and remotely manage IoT devices. 

**AWS IoT Events** services that makes easy to detect and respond to events from IoT sensors and applications. 

**AWS IoT SiteWise** service that makes it easy to collect and organize data from industrial equipment at scale. 

**AWS IoT Things Graph** is a service that makes it easy to visually connect different devices and web services to build IoT applications.

**AWS Partner Device Catalog** helps you find devices and hardware to help you explore, build and go to market with your IoT solution. 

## Machine Learning

**Amazon pagemaker** fully managed platform that enables developers and data scientist to quickly and easily build, train and deploy machine learning models at any scale. 

**Amazon SageMAker Ground Truth** helps you to build highly accurate training datasets for machine learning.

**Amazon Comprehend** is a natual language processing service that uses machine learning to find insights and relationships in texts.

**Amazon Lex** is a service for building conversational interfaces into any application using voice and text.

**Amazon Polly** is a service that turns test into lifelike speech.

**Amazon Rekognition** is a service that makes it easy to add image analysis to you applications

**Amazon Translate** is a neural machine translation service that delivers fast, high quality and affordable language translation.

**Amazon Transcribe** is an automatic speech recognition service that makes it easy for developers to add speech-to-text capability to their applications

**Amazon Elastic Inference** allows you to attach low-cost GPU powered acceleration to amazon EC2 and Amazon sagemaker. 

**Amazon Forecast** is a fully managed service that uses machine learning to deliver highly accurate forecasts. 

**Amazon textract** is a service that automatically extracts text and data from scanned documents. 

**Amazon personalize** is a machine learning service that makes it easy for developers to create individualised recommendations for customers using their applications. 

**Amazon Deep Learning AMIs** provides marching learning practitioners and researchers with the infraestructure and tools to accelerate deep learning in the cloud. 

**AWS DeepLeans** helps put deep learning in the hands of developers

**AWS DeepRacer** is a 1/18th scale race car which gives you an interesting and fun way to get started with reinforcement learning.

**Apache MXNet on AWS** is a fast and scalable training and inference framework with easy-to-use, concise api for machine learning.

**TensoFlow on AWS** enables developers to quickly and easily get started with deep learning in the cloud. 

**AWS Inferentia** is a machine learning inference chip designed to delver high performance at low cost. 

## Management and Governance

**Amazon CloudWatch** is a monitoring service that provide you data about your applications

**AWS Autoscaling** monitors your applications and automatically adjust capacity to maintain steady, predictable performance at the lower possible cost.

**AWS Control Tower** automates the set up of a baseline environment or landing zone that is a secure well-architected multi account AWS environment.

**AWS System Manager** gives you the visibility and control of your AWS infraestructure, containing the following tools:

* Resurce Groups: lets you create logical group of resources associated with a particular workload. 
* Insight Dashboard: Displays operational data that the AWS manager automatically aggregates for each resource group.
* Run Command: Simple way to automate administrative tasks in EC2 or servers on premise
* State Manager: Helps you define and maintain consistent OS configurations such us firewall settings and anti-malware definition to comply your policies. 
* Inventory: Helps you collect and query configurations about your instances and installed software on them. 
* Maintenance Window: lets you define a recurring window of time to run administrative an maintenance tasks accross your instances
* Patch Manager: Helps you select and deploy operating system and software patches automatically across a large group of instances.
* Automation: Simplifies common maintenance and deployment tasks such as updating Amazon Machine images (AMIs)
* Parameter store: provides encrypted location to store important administrative information such us passwords and database strings.
* Distributor: helps you securely distribute and install software packages such as software agents.
* Session Manager: provides a browser-based interactive shell and CLI for managing Windows and Linux EC2 instances without need to open inbound ports manage SSH keys or use bastion hosts.

**AWS CloudFormation** gives developers and system administrators an easy way to create and manage a collection of related AWS resources provisioning and updating them in an orderly and predictable fashion. 

**Cloud Trail** is a web service that records AWS API calls for your account and delivers log files to you. 

**AWS Config** is a fully managed service that provides you an AWS resource inventory, configuration history and configuration change notification to enable security and governance. 

**AWS OpsWork** is a configuration manager service that provides managed instances of Chef and Puppet.

**AWS Service Catalog** allows organizations to create and manage catalog of IT services that are approved for use on AWS.

**AWS Trusted Advisor** is an online resource to help you reduce cost, increase performance and improve security by optimizing your AWS environment.

**AWS Personal Health Dashboard** provides alerts and remediation guidance when AWS is experiencing  events that might affect you.

**AWS Managed Services** provides ongoing management of your AWS infraestructure so you can focus on your application.

**AWS Console Mobile Application** lets customer view and amange a select set of resources to support incident response while on the go. 

**AWS License Manager** makes it easy to manage licenses in AWS and on-premises server from software vendors like Microsoft, SAP, oracle or IBM.

**AWS Well-architected Tool** helps you review the state of your workloads and compares them to the latest AWS architectural best practices. 

## Media Services

**AWS Elastic Transcoder** is a media transcoding in the cloud.

**AWS Elemental MediaConnect** is a high-quality transport service for live video.

**AWS Elemental MediaConvert** is a file base video transcoding service with bradcast-grade feature. 

**AWS Elemental MediaLive** is a broadcast-grade live video processing service. 

**AWS Elemental Media Package** realiably prepares and protects your videos for delivery over the internet. 

**AWS Elemental MediaStore** is an AWS store service optimized for media.

**AWS Elemental Media Tailor** lets video providers insert individually tarfeted advertising into their video streams without sacrificing broadcast-level quality of service. 

## Migration and Transfer

**AWS Migration Hub** provides a single location to track the progress of applications migration across multiple AWS and partner solutions

**AWS Application Discovery Service** helps enterprise curstomers plan migration projects by gathering information about their on-premise data centers.

**AWS Database Migration Service** helps you migrate database to AWS easily and securely. 

**AWS Server Migration Service** is an agentless service which makes it easier and faster for you to migrate thousand of on-premise workloads to AWS.

**AWS Snowball** is a petabyte-scale data transport solution that uses secure appliances to transfer large amounts of data into and out of AWS.

**AWS Snowball Edge** is a data migration and edge computing device.

**AWS Snowmobile** is an exabyte-scale data transfer service used to move extremely large amounts of data to AWS. You can transfer up to 100PB per snowMobile, a 45-foot long shipping container. 

**AWS DataSync** is a data transfer service that makes it easy for you to automate moving data between on-premises storage and Amazon S3 or Amazon Elastic File System. 

**AWS Transfer to SFTP** is a fully managed service that enables the transfer of files directly into S3 using SFTP.

## Mobile

**AWS Amplify** makes it easy to create, configure and implement scalable mobile applications powered by AWS. Amplify manages your mobile backend and provides a simple framework for your front, iOS, android, web and react native. 

**Amazon Cognito** lets you add user sign-up, sign-in and access control to your web and mobile apps quickly and easily.

**Amazon PinPoint** makes it easy to send targeted messages to your customers through multiple engagement channels

**AWS Device Farm** in as n app testing service that lets you test and interact with your Andoid, iOS and web app on many devices at once. 

**AWS AppSync** is a serverless back-end for mobile, web and entrerprise applications.

## Networking and Content Delivery

**Amazon VPC** lets you provision a logically isolated sections of the AWS cloud where you can launch AWS resources in a virtual network that you define. 

**Amazon CloudFront** is a fast content delivery network (CDN) service that securely delivers data, videos, applications an APIs to customers globally with low latency high speed transfer.

**Amazon Route 53** is a highly available and scalable cloud domain name system (DNS) web service. 

**AWS PrivateLink** simplifies the security of data shared with cloud-based applications from VPC or on-premises applications by eliminating the exposure of data to the public internet. 

**AWS Direct Connect** makes easy to establish a dedicated network connection from your on-premises data center to AWS. 

**AWS Global Accelerator** is a network service that improves de availability and performance of the applications that you offer to your global users.

**Amazon API Gateway** is a fully managed service that makes it easy for developers to create, publish, maintain, monitor and secure APIs at any scale. 

**AWS Transit Gateway** is a service that enables customers to connect their Amazon Virtual Private Clouds and their on-premise networks to a single gateway.

**AWS App Mesh** Makes it easy to monitor and control microservices running in AWS. 

**AWS Cloud Map** is a cloud resource discovery service 

**Elastic Load Balancer** automatically distribute incoming application traffic across multiple targets such as Amazon EC2 instances. It comes in three flavours:

* Application Load Balancer: is the best for load balancing HTTP and HTTPS traffic and provide advanced request routing. It operates at request level (Layer 7).
* Network Load Balancer: is best suited for load balancing of TCP traffic where extreme performance is needed. It operates at connection level (Layer 4)
* Classic Load Balancer: provides basic load balancing across multiple Amazon EC2 instances and operates at both levels request level and connection level. This Load blaancer is intended for applications that were built within the EC2-Classic Network.

## Robotics

**AWS Robomaker** is a service that makes it easy develop, test and deplot intelligent robotic applications at scale. 

## Satellite

**AWS Ground Station** is a fully managed service that lets you control satellite communications.

## Security, Identity and Compliance

**AWS Security Hub** gives you a comprehensive view of your high priority security alerts and compliance status accross AWS accounts. 

**Amazon Cloud Directory** enables you to build flexible, cloud-native directory for organizing hierarchies of data along multiple dimensions. 

**AWS Identity and Access Management (IAM)** enables you to securely control access to AWS services and resources for users. IAM allows to do the following:

* Manage IAM users and their access
* Manage IAM Roles and their permissions
* Manage federated users and their permissions: you can enable identity federation to allow existing identities in your enterprise to access the AWS management Console, call AWS APIs and access resources  without the need to create an IAM user for each identity. 

**Amazon GuardDuty** is a threat detection service that continuously monitors for malicious unauthorised behaviours to help you protect your AWS account and workloads.

**Amazon Inspector** is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS.

**Amazon Maice** is a security service that uses machine learning to automatically discover, classify and protect sensitive data in AWS.

**AWS artefact** is your go-to central resource for compliance-related information that matters to you. 

**AWS Certificate Manager** is a service that lets you provision, manage and deploy secure socket layer / transport layer security SSL/TLS certificates ofr use with AWS services and your internal connected resources. 

**AWS CloudHSM** is a cloud-based hardware security module that enables you to generate and use your own encryption keys on AWS cloud.

**AWS Directory Service** for microsoft Active directory, enables your directory-aware wokload and AWS resources to use managed active directory in the AWS cloud. 

**AWS Firewall Manager** is a security management service that makes easy to centrally configure and manage AWS WAF rules across your accounts and applications. 

**AWS Key Management Service** makes it easy for you to create and manage keys and control the use of encryption across a wide range of AWS services.

**AWS Organisations** offer policy-based management for multiple AWS accounts. With organizations you can create groups of accounts, automate account creation, apply and manage policies for those groups. 

**AWS Secret Manager** helps you protect secrets needed to access your applications services and IT resources. 

**AWS Shield** is a managed distributed Denial of Service (DDoS) protection. The standard shield provides protection at infraestructure level (Layer 3 and 4). Shield Advanced provides near real time visilibity for DDoS attacks and gives you 24x7 access to the AWS DDoS resposne team and protection against spikes in your charges.

**AWS Single Sign-On** is a cloud SSO service that makes it easy to centrally manage SSO access to multiple AWS accounts and business applications. 

**AWS WAF** is a web application firewall that helps protect your web applications from common web exploits that could affect application availability.

## Storage

**Amazon S3** is an object storage service that offers industry-leading scalability, data visibility, security and performance.

**Amazon Elastic Block Store** provides persisten block storage volumes for use with Amazon EC2 instances in the AWS cloud.

**Amazon Elastic File System** provides a simple scalable, elastic file system for linux based workloads for use with AWS cloud services and on-premises resources.

**Amazon FSx Lustre** is a fully managed file system that is optimized for compute intensive workloads such as high performance computing, machine learning and media data processing workflows.

**Amazon FSx for Windows File Server** provides a fully managed native microsoft windows file system so you can easily move your windows-base applications that requires file storage to AWS. 

**Amazon Glacier** is a secure durable and extremly low cost storage service for data archiving and long-term backups. 

**AWS Storage Gateway** is a hybrid storage service that enables your on-premises application to seamlessly use AWS cloud storage. 

