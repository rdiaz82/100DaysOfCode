## Key Principles

There are three key aspects of pricing in AWS:

* compute
* storage
* outbound data transfer

In most cases inbound data transfer or data transfer between services in the same region is not charged. 

## Start early with cost optimization

Adopting a clud serbive is not just adopt the technical solution. It alsoe requires changes to organizations operate. It's never too early to start with cost optimization in AWS.

## Maximize the power of flexibility

AWS serbices prices are intenpendent and transparent., so you can choose and pay for exactly what you need and no more. No minimum commtments or long term contracts are required unless you choose to save money through a reservation model. 

## Use Right pricing model for the job:

**On Demand** means you pay for the compute of database capacity with no long termi commitments or upfront payments. 

**Dedicated instances** run in a private cloud (VPC) on hardware that's dedicated to a single customer. 

**Spot Instances** are an Amazon EC2 pricing mechanism that lets you purchase spcare computing capacity with no upfront commitment ad discounted hourly rates.

**Reservation** provides you with the ability receive a greater discount, up to 75% by paying for capacity ahead of time.

## Get started with the AWS Free Tier

The AWS free tier enables you to gain free access ti AWS platform, and services. The AWS free Tier includes offer that expire 12 month after sign-in, other offers inside free Tier doesn't expire. 

* Offer that expires: EC2, S3, RDS and cloudfront
* Offers that not expires: DynamoDb,  Amazon Glacier, AWS lambda.

## EC2 pricing

**On demand instances:** You pay for compute capacity per hour  or per second. depending on which instances you run. No long-term commitments or upfront payment is needed.

**Spot instances**: aallow you to request space Amazon EC2 computing capacity for up to 90 percent off the OnDemand price. Spot instances are suitable for:

* Applications that have flexible star and end times
* Applications that aew only feasibles at very low compute price
* User with urgent computing needs for a lot of additional capacity.

**Reserved instances** provide you with a significant discount compared with On demand instances pricing. In addition, when reserved instances are assigned to specific Availability zone  they provide a capacity reservation, giving you additional confidence in your availability to launch instances when you needed them. This instances are perfects for predictable patterns of use. 

**Dedicated Hosts** is a physical EC2 server dedicated for your use. Dedicated hosts can help you reduce costs by allowing you to use your existing server-bound sotware licenses including windows server.

**Per-second billing** Since 2017 you have per-second billing for usage of Linux instances across On-Demand ,reserved, and Spot instances. 

## Estimate EC2 Cost

When you begin to estimate the cost of a EC2 instance you need to consider the following:

* Clock hours of serve time
* Instance type
* Pricing Model
* Number of Instances
* Load Balancing
* Detailed monitoring
* AutoScaling
* Elastic IP address 
* Operating System and software packages

## AWS Lambda

Aws lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume. There is no charge when your code is not running. With AWS lambda you can run code for virtually any type of application or backend service with zero administration.

**AWS Lambda pricing:** You only pay for what you use. You are charged based on the number of requests for your functions and the time it takes for your code to execute. 

## Amazon RDS

The cost of RDS comes from the following factors:

* Clock hours of server time
* Database characteristics
* Database purchase associated instances (On demand vs reserved)
* Number of database instances
* Provisioned storage
* Additional storage
* Requests
* Deployment type: single availability zone vs multiple availability zones
* Data transfer out

## Dynamo DB

Dynamo Db asks you about your prevision in terms of use and then automatically all resources are provisioned. The key aspects are:

* Provisioned throughput (write)
* Provisioned throughput (read)
* Indexed Data storage

## Cloud Front

Amazon CloudFront charges are based on the data transfers  and requests used to deliver content to your customers. There are no upfront payments or fixed platform fees. The cost will be estimated based on the following aspects:

* Traffic distribution: the price varies in different regions and pricing is based on the edge location through the content is served
* The number of requests
* Data transfer out

