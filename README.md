# AWS Certified Cloud Practitioner (ACCP) Exam Note

[![Twitter Follow](https://img.shields.io/twitter/follow/045_hamid?label=045_hamid&style=plastic&logo=twitter&color=blue)](https://twitter.com/045_hamid)
[![GitHub Follow](https://img.shields.io/github/followers/hamidgholami?label=hamidgholami&style=plastic&logo=github&color=green)](https://github.com/hamidgholami)
[![Linkedin Badge](https://img.shields.io/badge/hamid--gholami-LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/hamid-gholami/)
<!--
[![Youtube Badge](https://img.shields.io/badge/-geekestan-red?style=plastic&&logo=youtube&message=geekestan&logoColor=white)](https://www.youtube.com/channel/UCBlOVqLEwcvFNG03KDAVTlw)
-->

This is my notes regarding ACCP exam which is completed gradually when I was studing the exam objectives.

> Who should take this exam?<br>
>
>[The AWS Certified Cloud Practitioner](https://aws.amazon.com/certification/certified-cloud-practitioner/) (*CLF-C01*) exam is intended for individuals<br>who can effectively demonstrate an overall knowledge of the AWS Cloud<br>independent of a specific job role.

You can find every updated information in this [link](https://aws.amazon.com/certification/certified-cloud-practitioner/) which is the official and reputable information.


The following table lists the main content domains and their weightings.<br>
Also you can download [the official exam guide](https://d1.awsstatic.com/training-and-certification/docs-cloud-practitioner/AWS-Certified-Cloud-Practitioner_Exam-Guide.pdf).

<div align="center">

| Domain                            | % of Exam |
|:-----------------------------------|:-----------:|
| Domain 1: Cloud Concepts          | 26%       |
| Domain 2: Security and Compliance | 25%       |
| Domain 3: Technology              | 33%       |
| Domain 4: Billing and Pricing     | 16%       |
| **Total**                             | **100%**      |

</div>

* * *
### Table of contents
 - [Amazon S3](#amazon-s3)
 - [Six advantages of Amazon Cloud (Benefits)](#six-advantages-of-amazon-cloud-benefits)
 - [AWS Compute Optimizer](#aws-compute-optimizer)
 - [Amazon EBS volumes types](#amazon-ebs-volumes-types)
 - [Amazon load balancers](#amazon-load-balancers)
 - [AWS Network ACL](#aws-network-acl)
 - [AWS Security Groups](#aws-security-groups)
 - [AWS Internet Gateway](#aws-internet-gateway)
 - [AWS Scalability](#aws-scalability)
 - [Amazon Simple Notification Service (SNS)](#amazon-simple-notification-service-sns)
 - [Amazon Simple Queue Service (SQS)](#amazon-simple-queue-service-sqs)
 - [AWS Inspector](#aws-inspector)
 - [AWS Trusted Advisor](#aws-trusted-advisor)
 - [AWS Personal Health Dashboard](#aws-personal-health-dashboard)
 - [AWS TCO Calculator](#aws-tco-calculator)
 - [AWS EBS](#aws-ebs)
 - [Amazon SageMaker](#amazon-sagemaker)
 - [Amazon Kinesis](#amazon-kinesis)
 - [Cloud Computing](#cloud-computing)
 - [AWS CloudFormation](#aws-cloudformation)
 - [AWS Elastic Beanstalk](#aws-elastic-beanstalk)
 - [AWS Lambda](#aws-lambda)
 - [AWS Well-Architected Framework](#aws-well-architected-framework)
 - [AWS WAF](#aws-waf)
 - [AWS AD Connector](#aws-ad-connector)
 - [AWS Simple AD](#aws-simple-ad)
 - [Amazon Elastic Container Service for Kubernetes (EKS)](#amazon-elastic-container-service-for-kubernetes-eks)
 - [Amazon Elastic Container Service (ECS)](#amazon-elastic-container-service-ecs)
 - [Virtual Private Gateway](#virtual-private-gateway)
 - [VPC peering connection](#vpc-peering-connection)
 - [AWS support plans](#aws-support-plans)
 - [Amazon IAM](#amazon-iam)
 - [Amazon Cognito](#amazon-cognito)
 - [Popular HTTTP code](#popular-htttp-code)
 - [AWS CloudTrail](#aws-cloudtrail)
 - [Amazon DynamoDB](#amazon-dynamodb)
 - [AWS Database SQL type](#aws-database-sql-type)
 - [AWS Device Farm](#aws-device-farm)
 - [AWS Config](#aws-config)
 - [AWS Shared Responsibility Model](#aws-shared-responsibility-model)
 - [Amazon RDS](#amazon-rds)
 - [AWS Auto Scaling Group](#aws-auto-scaling-group)
 - [AWS CloudHSM](#aws-cloudhsm)
 - [AWS Auto Scaling](#aws-auto-scaling)
 - [AWS Glacier](#aws-glacier)
 - [AWS Storage Gateway Volume Gateway](#aws-storage-gateway-volume-gateway)
 - [AWS Step Functions](#aws-step-functions)
 - [Amazon Simple Workflow Service (SWF)](#amazon-simple-workflow-service-swf)
 - [Amazon Security Token Service (STS)](#amazon-security-token-service-sts)
 - [AWS Server Migration Service (SMS)](#aws-server-migration-service-sms)
 - [Amazon DevPay](#amazon-devpay)
 - [Amazon Elasticsearch Service](#amazon-elasticsearch-service)
 - [Amazon Athena](#amazon-athena)
 - [Amazon QuickSight](#amazon-quicksight)
 - [Amazon CodeStar](#amazon-codestar)
 - [Amazon Cloud9](#amazon-cloud9)
 - [Amazon CodeDeploy](#amazon-codedeploy)
 - [Amazon Route 53](#amazon-route-53)
 - [Amazon CloudFront](#amazon-cloudfront)
 - [Amazon Lightsail](#amazon-lightsail)
 - [Amazon EC2](#amazon-ec2)
 - [AWS pricing policies](#aws-pricing-policies)
 - [AWS Cost Explorer](#aws-cost-explorer)
 - [AWS Cost Anomaly Detection](#aws-cost-anomaly-detection)
 - [Amazon Elastic Transcoder](#amazon-elastic-transcoder)
 - [AWS Organization](#aws-organization)
 - [AWS Glue](#aws-glue)
 - [AWS Artifact](#aws-artifact)
 - [AWS WAF](#aws-waf)
 - [AWS Service Catalog](#aws-service-catalog)
 - [AWS Managed Services](#aws-managed-services)
 - [Amazon Machine Image (AMI)](#amazon-machine-image-ami)
 - [Five design principles for performance efficiency in the cloud](#five-design-principles-for-performance-efficiency-in-the-cloud)
 - [Five design principles for cost optimization in the cloud](#five-design-principles-for-cost-optimization-in-the-cloud)
 - [Five design principles for reliability in the cloud](#five-design-principles-for-reliability-in-the-cloud)
 - [Six design principles for security in the cloud](#six-design-principles-for-security-in-the-cloud)
 - [Five pillars of the AWS Well-Architected Framework](#five-pillars-of-the-aws-well-architected-framework)
 - [Amazon S3 Transfer Acceleration](#amazon-s3-transfer-acceleration)
 - [Amazon Neptune](#amazon-neptune)
 - [Amazon Elasicsearch](#amazon-elasicsearch)
 - [AWS Direct Connect](#aws-direct-connect)
 - [AWS Snowball](#aws-snowball)
 - [Amazon Comprehend](#amazon-comprehend)
 - [Amazon Resource Names (ARNs)](#amazon-resource-names-arns)
 - [Amazon ELB](#amazon-elb)
 - [AWS IoT Core](#aws-iot-core)
 - [AWS Fargate](#aws-fargate)
 - [Amazon Detective](#amazon-detective)
 - [Amazon Global Accelerator](#amazon-global-accelerator)
 - [AWS Data Sync](#aws-data-sync)
 - [AWS CodePipeline ](#aws-codepipeline)
 - [Amazon GuardDuty](#amazon-guardduty)
 - [Amazon Macie](#amazon-macie)
 - [AWS X-Ray](#aws-x-ray)
 - [AWS OpsWorks](#aws-opsworks)
 - [Geographical Services](#geographical-services)
 - [Notes](#notes)

***
### Amazon S3
- **CRR** (Cross-region replication): enables automatic, asynchronous
copying of objects across buckets in different AWS Regions.
- You cannot reserve capacity.
- Bucket names rules:
	- Names must be unique across all of AWS
	- Names must be 3 to 63 characters in length
	- Names can only contain lowercase letters, numbers and hyphens.
	- Names cannot be formatted as an IP address.
- IAM policies can be written to grant access to Amazon S3 buckets.
- Amazon S3 storage tier:
	- **S3 Standard** -> 99.99% SLA -> for data that is accessed less frequently, butrequires rapid access when needed
	- **S3 Standard-IA** -> 99.9% SLA -> offers the high durability, high throughput, and low latency of S3 Standard
	- **S3 One Zone-IA** -> 99% SLA ->  *the most cost-effective* Amazon S3 storage tier for data that is not often accessed but requires high durability. It stores data in a **single** AZ
	- **Glacier** -> No SLA
- **Multipart upload** can be used to speed up uploads to S3
- **S3 Copy** -> up to 5GB in size in a single atomic operation
- **S3 Intelligent-Tiering** is an appropriate Amazon S3 storage class for "data with unknown/changing access pattern" 
- **Data consistency** models available are:
	- Read after write consistency for PUTS of new objects
	- Eventual consistency for overwrite PUTS and DELETES (takes time to propagate)
- "**MFA delete**" adds a layer of additional security to prevent accidental deletion.
- Amazon S3 **objects** consist of:
	- Key
	- Value
	- Version ID
	- Metadata
- **Object lifecycle management** can be used with objects so that they are stored cost effectively throughout their lifecycle. Objects can be transitioned to another storage class or expired. It enables you to **set rules** to **automatically transfer** objects between different storage classes at defined time intervals.
- **Standard-IA** and **One Zone-IA** both have a minimum storage duration charge of **30** days
	
### Six advantages of Amazon Cloud (Benefits)
- Trade capital expense for variable expense.
- Benefit from massive economies of scale.
- Stop guessing about capacity.
- Increase speed and agility.
- Stop spending money running and maintaining data centres.
- Go global in minutes.

### AWS Compute Optimizer
It helps avoid overprovisioning and underprovisioning, based on your utilization data, four types of AWS resources:
- Amazon Elastic Compute Cloud (EC2) instance types.
- Amazon Elastic Block Store (EBS) volumes.
- Amazon Elastic Container Service (ECS) services on AWS Fargate.
- AWS Lambda functions.

### Amazon EBS volumes types
- **General purpose(gp2)**(SSD): provides a good balance of price to performance, is suitable for most workloads and can be used as a system boot volume.
- **Provisioned IOPS(io1)**(SSD): is a high-performance volume type that is more expensive and should be used for apps that require the higher performance.
- **Cold HDD(sc1)**: cannot be used as a boot volume and is good for throughput oriented storage for infrequently accessed data.
- **Throughput Optimized(st1)**: It is ideal for streaming workloads with fast throughput such as big data and data warehouses.

### Amazon load balancers
- NLBs process traffic at the TCP level (layer 4)
- ALBs process traffic at the HTTP, HTTPS level (layer 7)
- CLBs process traffic at the TCP, SSL, HTTP and HTTPS levels (layer 4 & 7).
- *Load balancing with session affinity* can be used for **horizontal scaling** of **stateful** components.

### AWS Network ACL
- Stateless
- By default: all in - all out
- It operates on VPC subnet level
- Not used in S3

### AWS Security Groups
- Stateful firewalls
- By default: none in - all out
- Only `allow` rules, it is not possible to have `deny` rules
- It allows access through specific port
- It is possible to have **inbound** and **outbound** rules in a security group
- It operates on instance level, not on VPC subnet level
- Not used in S3

### AWS Internet Gateway
- Do not have `allow` or `deny` rules
- It operates on VPC level

### AWS Scalability
AWS Scaling **vertically**: increasing the instance size/CPU/RAM/DISK,...
AWS Scaling **horizontally**: adding more EC2 instances, AWS Lambda adding concurrently executing functions, Adding read replicas to an Amazon RDS database

### Amazon Simple Notification Service (SNS)
- **Topics**: how you label and group different endpoints that you send messages to
- **Subscriptions**: the endpoints that a topic sends messages to
- **Publisher**: the person/alarm/event that gives SNS the message that needs to be sent

- It is a web service that makes it easy to **set up**, **operate**, and **send notifications** <ins>from the cloud</ins>.
- SNS supports notifications over multiple transports including *HTTP/HTTPS*, *Email/Email-JSON*, *SQS* and *SMS*.
- It is used for building and *integrating* **loosely-coupled**, *distributed applications*.

### Amazon Simple Queue Service (SQS)
- It is a fully managed message queuing service that enables you to *decouple* and *scale microservices*, *distributed systems*, and *serverless applications*.
- **Use case**: *Decoupling application* components to ensure that there is no dependency on the availability of a single component.
- It can be used to ensure the **persistence** of **in-flight** *transactions independently* of any single application component.
- It is a message queue used for **decoupling** application components

### AWS Inspector
- Inspector is an *automated security assessment* service that helps improve the security and compliance of applications deployed on AWS.
- It uses an **agent** installed in EC2 instances and assesses applications for *vulnerabilities* and *deviations* from best practices.
- Organization can assess applications for vulnerabilities and **deviations** *from best practice*.

### AWS Trusted Advisor
- An **online resource** that helps to *reduce cost*, *increase performance* and *improve security* by **optimizing** your AWS environment.
- Five *categories* of Trusted Advisor:
	- Cost optimization
	- Security
	- Performance
	- Service limits
	- Fault tolerance
- It can be used to **display current usage and limits**.It offers a Service Limits check (in the *Performance* category) that displays your usage and limits for some aspects of some services
- It can be used to provide **real time guidance** on provisioning resources following *AWS best practices*.
- It can be used to **check service limits** for resources launched within AWS Infrastructure.

### AWS Personal Health Dashboard
- It provides **alerts** and **remediation** *guidance* when AWS is experiencing events that may *impact* you.

### AWS TCO Calculator
- It can be used to **compare** the *cost of running* your applications in an *on-premises* or colocation environment to *AWS*.
- "**Compute Hardware**" and "**Data Center Security**" should be included in a TCO analysis comparing on-premise to AWS Cloud.

### AWS EBS
- EBS Volume type
	- **Provisioned IOPS SSD**: supports **up to 50 IOPS** *per GiB* with **up to 32,000 IOPS** *per volume*.
	- **General Purpose SSD**: supports 3 IOPS per GiB and can burst up to 3000 IOPS (volumes > 334GB), and a maximum of **10,000** *per volume*.
	- Throughput Optimized HDD:
	- Cold HDD:
- The **easiest** way to store a backup of an EBS volume on Amazon S3: Create a **snapshot** of the volume.
- Amazon EBS snapshots are stored on *S3*.
- EBS volumes must be **in the same AZ** as the instances they are attached to.
- You can use *Amazon Data Lifecycle Manager* (**Amazon DLM**) to automate the creation, retention, and deletion of snapshots taken to back up your Amazon EBS volumes.
- The Fundamental *charges* for EBS volumes are:
	- the amount of data **provisioned** (**not** *consumed*) *per* <ins>month</ins>.
	- amount you provision in **IOPS**
- The **root** EBS volumes are **deleted** on termination by <ins>default</ins>.
- Extra **non-root** volumes are **not deleted** on termination by <ins>default</ins>.
- Both non-root and root if launched from an **encrypted** AMI.

### Amazon SageMaker
- That enables developers and data scientists to quickly and easily **build**, **train**, and **deploy** <ins>machine learning models</ins> at any scale. 

### Amazon Kinesis
- There are four **types** of Kinesis services:
	- Kinesis Video Streams
	- Kinesis Data Streams
	- Kinesis Data Firehose
	- Kinesis Data Analytics
- It enables you to build custom applications that process or analyze **streaming data** for specialized needs.
- **Producers** continually push data to Kinesis data Streams and **Consumers** process the data in *real time*.
- Consumers can <ins>store their results</ins> using an AWS service such as:
	- Amazon DynamoDB
	- Amazon Redshift
	- Amazon S3

### Cloud Computing
- Cloud computing is the **on-demand** delivery of compute power.
- With cloud computing you get to <ins>benefit from massive economies of scale</ins>.
- With cloud computing you can <ins>increase your speed and agility</ins>.

### AWS CloudFormation
- It provides a **common language** for you to <ins>describe</ins> and <ins>provision</ins> all the infrastructure resources in your cloud environment.
- It's free of charge.
- **Change sets** allow you to preview how proposed changes to a stack might impact your running resources.

### AWS Elastic Beanstalk
-  The **fastest** and **simplest** way to get web applications up and running on AWS.
-  It is more of a **PaaS** service and is focused on <ins>web applications</ins> not infrastructure.

### AWS Lambda
- Lambda functions can be invoked in response to **events**.
	- Invoke a function in response to resource lifecycle events, such as with Amazon **S3**. (*Lambda & S3*)
	- Respond to incoming **HTTP requests**. (*Lambda & API Gateway*)
	- Consume events *from* a **queue**. (*Lambda & SQS*)
	- Run a function on a **schedule**. (*Lambda & CloudWatch*)

### AWS Well-Architected Framework
- Operation excellence
- Security
- Reliability
- Performance efficiency
- Cost optimization

### AWS WAF
- create custom rules that block <ins>common attack patterns</ins>, such as:
	- SQL injection.
	- Cross-site scripting.
	- Rules that are designed for your specific application

### AWS AD Connector
- A directory gateway for **redirecting** <ins>directory requests</ins> to your on-premise Active Directory.
- Connects your **existing** *on-premise AD* to AWS.

### AWS Simple AD
- An inexpensive **Active Directory**-compatible service with common directory features.
- It is a **standalone**.
- It does **not** connect your on-premise AD to AWS

### Amazon Elastic Container Service for Kubernetes (EKS)
- It's a managed Kubernetes service that makes it easy for you to run Kubernetes on AWS without needing to install, operate, and maintain your own Kubernetes **control plane**.

### Amazon Elastic Container Service (ECS)
- It is used for running Docker containers on <ins>EC2 instances</ins>.

### Virtual Private Gateway
- It's the VPN concentrator on the **Amazon side** of the <ins>VPN connection</ins>.
-  You create a virtual private gateway and *attach* it to the **VPC** from which you want to create the VPN connection.
-  <ins>NAT devices and firewalls</ins> are **not** required for an *AWS managed VPN*.
-  A **customer gateway** is a physical device or software application on **your side** of the VPN connection.

### VPC peering connection
- if you have **more than one AWS account**, you can **peer** the VPCs across those accounts to create a <ins>file sharing network</ins>.
- You **cannot** peer *subnets*.
- It is a way of <ins>allowing routing between VPCs</ins> in *different AWS accounts*.
- It enables you to route traffic via **private IP addresses** between *two* peered VPCs.

### AWS support plans
- **Basic**: Does not provide any <ins>*technical support*</ins>.
- **Developer**: Provides **business hours** access via **email**.
- **Business**: Provides < 1-hour response times for a <ins>production system failure</ins>.
- **Enterprise**: Provides < 1-hour response times for a <ins>production system failure</ins> but is a **more expensive**.
- All support plans provide "**24/7**":
	- access to customer service
	- documentation
	- whitepapers
	- support forums
- Only the **Enterprise** plan provides a **response time of < 15 minutes** for the failure of a *business-critical system*.
- Both **Business** and **Enterprise** offer < 1-hour response time for the failure of a production system.
- Only **business** and **enterprise** plans provide *support via* **email**, **chat** and **phone**.
- **Enterprise** plan comes with a *Technical Account manager*(**TAM**)
- **Developer** plan provides **email support** by **cloud support associates** team whereas **business** and **enterprise** provide **email support** by the **cloud support engineers** team.
- With the **Developer** plan you can open **unlimited** cases.

### Amazon IAM
- You **cannot** use IAM to create **local user accounts** on any system.
- You are also not charged for what you use, <ins>IAM is free to use</ins>.
- You can share access to your AWS account.
- Identity federation.
- PCI DSS complince.
- AWS recommended **best practices**:
	- Create individual IAM users
	- Least privilege principle: granting only the permissions that are needed to perform specific tasks
 	- Culture strong passwords
  	- Multi-factor authentication
- IAM **supported authentication** methods include:
	- Console passwords
	- Access keys
	- Server certificates
- Best practice to ensure the security of AWS account
	- **Don’t generate** an access key for the **root account** user
	- Use **Temporary Security Credentials** (IAM Roles) Instead of Long-Term Access Keys
	- Manage IAM User Access Keys Properly
- You can enable single sign-on (**SSO**) to your AWS accounts by using **federation** and AWS Identity and Access Management (IAM).
- All you can do with an **access key** once it has been generated is to:
	- Make active
	- Make inactive
	- Delete
- IAM Policy Simulator evaluates the policies that you choose and determines the effective permissions for each of the actions that you specify.

### Amazon Cognito
- Amazon Cognito Identity Pool provides temporary AWS credentials for users who are guests (unauthenticated) and for users who have been authenticated and received a token. An identity pool is a store of user identity data specific to your account.
- Amazon Cognito User Pool is a user directory in Amazon Cognito. It doesn't enable access to unauthenticated identities. You have to use an Identity Pool instead.

### Popular HTTTP code
- A HTTP 200 codes: successful
- A HTTP 300 codes: redirection
- A HTTP 400 codes: client error
- A HTTP 500 codes: server error

### AWS CloudTrail
- It is a web service that **records activity** made on your account and delivers <ins>log files</ins> to an **Amazon S3 bucket**.
- Logging and saves a history of API calls for your AWS account.
- It is for **auditing**.
- It records account activity and service events from most AWS services and logs the following records:
	- The identity of the API caller.
	- The time of the API call.
	- The source IP address of the API caller.
	- The request parameters.
	- The response elements returned by the AWS service.

### Amazon DynamoDB
- It's a fully managed **NoSQL** database service. (schema-less)
- You can scale the DB at any time **without incurring downtime**.
- DaynamoDB pricing models:
	- **On-demand capacity mode**: charges you for the data reads and writes your application
	- **Provisioned capacity mode**: you specify the number of reads and writes per second that you expect
- Availability model:
	- **Data is synchronously** replicated across **3** facilities in a region
- Best practices for storing **large items** and attributes in DynamoDB:
	- <ins>Compress</ins> large attribute values
	- Store large attributes as objects in <ins>Amazon S3</ins>.

### AWS Database SQL type
- Amazon RDS
- Amazon Aurora
- Amazon RedShift

### AWS Device Farm
- It is an **app testing service** that lets you **test** and **interact** with your **Android**, **iOS**, and **web apps** on <ins>many devices</ins> at once, or reproduce issues on a device in real time

### AWS Config
-  It allows you to **automate the evaluation of recorded** configurations against desired configuration.
-  It enables you to **assess**, **audit**, and **evaluate** the <ins>**configurations of your AWS resources**</ins>.
-  It continuously **monitors** and **records** your <ins>AWS resource configurations</ins> and allows you to automate the evaluation of recorded configurations against desired configurations.
-  It can be used to **keep track** of configuration changes on AWS resources, *keeping multiple date-stamped* versions in a reviewable history.
-  It can be used to **retrieve configuration** changes made to AWS resources causing *operational issues*.

### AWS Shared Responsibility Model
- Customers are responsible for *networking traffic protection*.
- AWS are responsible for networking **infrastructure**.
- AWS are responsible for **compute infrastructure**.
- Customers are responsible for *network and firewall configuration*.
- **AWS** are responsible for **edge locations**.
- **Shared Controls**: Apply to both the *infrastructure layer* and *customer layers*
	- Patch Management: AWS -> Infra patches | Customer -> OS/Applications patches
	- Configuration Management: AWS -> Configuration of its infra devices | Customer -> Configuration their OS, Apps, DBs.

### Amazon RDS
- Read replicas are used for **offloading read traffic** from the primary RDS database.
	- You can configure **read replicas** to be:
		- within as AZ
		- across AZs
		- across regions
- It provides "**Multi-AZ**" and "**Read Replicas**" to deliver *scalability*, *availibility* and *durability*.
- You can **restore** a DB instance to a specific **point in time** with a granularity of **5 minutes**
- **Multi-AZ**: <ins>synchronously</ins>
- **Read Replicas**: <ins>asynchronously</ins>
- RDS supports the following **engines**:
	- SQL Server
	- Oracle
	- MySQL Server
	- PostgreSQL
	- Aurora
	- MariaDB
- **Read replicas** are available for:
	- MySQL
	- PostgreSQL
	- MariaDB
	- Aurora
- RDS **automated** *backups* allow point in time recovery to any point within the retention period down to a second.
- RDS supports **automated backups** as a **default** configuration
- With RDS you are **charged for**:
	- the type and size of DB
	- document type (e.g multi AZ)
	- data transfer outbound
	- requests
	- the uptime
	- any additional storage of backup

### AWS Auto Scaling Group
- **Scaling Policy** determine when, if, and how the ASG scales and shrinks:
	- **on-demand**(dynamic scaling)
	- **cyclic**(scheduled scaling)
- **Scaling Plan** define the triggers and when instances should be provisioned/de-provisioned

### AWS CloudHSM
- Is a **cloud-based hardware security module**(HSM) that allows you to easily <ins>add secure key storage</ins> and <ins>high performance crypto operations</ins> to your AWS applications.
- CloudHSM has **no upfront costs** and provides the ability to *start* and *stop* HSMs **on-demand**, allowing you to provision cpacity when and where it is needed quickly and cost-effectively.
- CloudHSM is a managed service that **automates** <ins>time-consuming administrative tasks</ins>, such as hardware provisioning, **software patching**, **high availability**, and **backups**.
- It uses a highly secure *hardware storage device* to **store encryption keys**

### AWS Auto Scaling
- The **scaling policies** include:
	- simple
	- scheduled
	- dynamic
	- step scaling
- vertical scaling -> scaling-up
- horizontal scaling -> scaling-out

### AWS Glacier
- Data access option **retrieves** data:
	- **Standard**: takes 3-5 hours
	- **Expedited**: within 1-5 minutes
- That is accessed though  S3
- You *pay* for <ins>storage on a per GB/month</ins> basis, <ins>retrival requests</ins> and <ins>quantity</ins> (based on expedited, standard or bulk)
- For **interacting** with AWS **Glacier** require that you use the **AWS CLI** or write code(Using **REST API**)
- Only Amazon Glacier has **a minimum storage** duration charge of **90** days

### AWS Storage Gateway Volume Gateway
- The volume gateway represents the family of gateways that *support* **block-based volumes**, previously referred to as gateway-cached and gateway-stored modes. it allows you to <ins>use block-based volumes on-premise</ins> that are then **asynchronously** backed up to Amazon **S3**.
	- **Stored Volumes mode**:  the *entire dataset is stored on-site* and is **asynchronously** backed up to S3 (EBS point-in-time snapshots). Snapshots are incremental and compressed
	- **Cached Volume mode**: the *entire dataset is stored on S3* and a cache of the *most frequently accessed* data is cached on-site.

### AWS Step Functions
- It lets you **coordinate** *multiple AWS services* into **serverless** workflows so you can build and update apps quickly.
- It lets you build **visual** *workflows*.

### Amazon Simple Workflow Service (SWF)
- helps developers build, run, and scale background jobs that have parallel or sequential steps.
- SWF is **not** a <ins>*visual*</ins> workflow tool.
- It can assist with **coordinating tasks** across *distributed application* components.

### Amazon Security Token Service (STS)
- It's used for requesting **temporary** credentials.

### AWS Server Migration Service (SMS)
- It's an **agentless** service which makes it easier and faster for you migrate on-premises workloads to AWS.
- You can migrarte Virtual Machines from **VMware vSphere** and **Windows Hyper-V** to AWS with this sevice.

### Amazon DevPay
- That makes it easy for budinesses to **sell applications** that are built in, or run on top of, *Amazon Web Services*.

### Amazon Elasticsearch Service
- For **operational analytics** such as:
	- application monitoring
	- log analytics
	- clickstream analytics
- It allows you to search, explore, filter, aggrigate and visualize your data in near real-time.

### Amazon Athena
- For interactive analysis
- analyze data directly in **S3** and **Glacier** using <ins>standard SQL queries</ins>

### Amazon QuickSight
- For dashboards and visualizations

### Amazon CodeStar
- It enables you to **quickly develop**, **build**, and **deploy** applications on AWS. AWS CodeStar provides a **unified user interface**, enabling you to easily manage your software development activities <ins>in one place</ins>.

### Amazon Cloud9
- It's a cloud-based integrated development environment (**IDE**) that lets you write, run, and debug your code with just a **browser**.

### Amazon CodeDeploy
- It is a deployment service that **automates application deployments** to <ins>Amazon EC2 instances</ins>, <ins>on-premises instances</ins>, or <ins>serverless Lambda functions</ins>.

### Amazon Route 53
- It has a **global scope**.
- Both **CNAME** records and **Alias** records can be used to <ins>map a domain name to a target domain name</ins>. However, only a **CNAME** record can be used to map to a target domain **external** to AWS.
- You can transfer domains to Route 53 only if the Top Level Domain (**TLD**) is supported
- Amazon **Route 53 health checks** monitor the health and performance of your web applications, web servers, and other resources
- It offers the following *functions*:
	- Domain Name registry
	- DNS resolution
	- Health checking of resources
- **Routing policies** include:
	- simple
	- Weighted
	- Latency-based
	- Failover
	- Geo-Location

### Amazon CloudFront
- It has a **global scope**.
- It is a content delivery network (**CDN**) that allows you to store (cache) your content at “**edge locations**” located around the world.
- This allows customers to access content **more quickly** and provides security against **DDoS attacks**.
- It can be used for **data**, **videos**, **applications**, and **APIs**.
- Routing policies:
	- simple
	- weighted
	- latency based
	- failover
	- geo-location
	- geo-proximity
	- multi-value
	- traffic flow
- It supports below **origins**:
	- S3 Bucket
	- EC2 instance
	- Elastic Load Balancer
	- Route 53

### Amazon Lightsail
- It provides developers compute, storage, and networking capacity and capabilities to deploy and manage websites, web applications, and databases in the cloud. Also it provides **preconfigured VPS** that inclouds **everything required to deploy** or create a **DB**.
- The **product set** includes:
	- **VPS** (Virtual Private Servers)
	- Managed **MySQL** databases
	- **HA** storage
	- **Load balancing**

### Amazon EC2
- Types:
	- **General Purpose**: instances provide a balance of compute, memory and networking resources, and can be used for diverse workloads; these are ideal for applications that use resources in equal proportions such as web servers and code repositories.
	- **Compute Optimized**: instances are ideal for compute bound applications that benefit from high performance processors; these are well suited for batch processing workloads, media transcoding, high performance web servers, high performance computing (HPC), scientific modeling, dedicated gaming servers and ad server engines, machine learning inference and other compute intensive applications.
	- **Memory Optimized**: instances are designed to deliver fast performance for workloads that process large data sets in memory.
	- **Accelerated Computing**: instances use hardware accelerators, or co-processors, to perform functions, such as floating point number calculations, graphics processing, or data pattern matching, more efficiently than is possible in software running on CPUs.
	- **Storage Optimized**: instances are designed for workloads that require high, sequential read and write access to very large data sets on local storage; these are optimized to deliver tens of thousands of low-latency, random I/O operations per second (IOPS) to applications.
	- **High Performance Computing**: instances are built to offer the best price performance for running HPC workloads at scale on AWS; these are ideal for applications that benefit from high-performance processors such as large, complex simulations and deep learning workloads.
- EC2 pricing model:
	- **On-Demand**: It is the **most economical** option that will ensure **no interruptions**.
	- **Spot**: They are good for **short term requirements** as they can be very economical. However, you may find that the instance is terminated if the spot market price moves.
	- **Dedicated Instance**: They are EC2 instances that run on hardware dedicated to a single customer.
	- **Reserved**: They are good for **long-term**, static requirements as you must lock-in for **1 or 3 years** in return for a decent discount.
- It offers SLAs of **95%** for *each region*.
- EC2 **benefits** over using non-cloud servers:
	- Elastic Web-Scale computing
	- Inexpensive
- Types of Reserved Instance(RI):
	- **Standard RIs**: These provide the **most significant discount** (up to 75% off On-Demand) and are best suited for **steady-state** usage.
	- **Convertible RIs**: These provide a discount (up to 54% off On-Demand) and the <ins>capability to change</ins> the attributes of the RI as long as the exchange results in the creation of Reserved Instances of equal or greater value. Like Standard RIs, Convertible RIs are best suited for steady-state usage.
	- **Scheduled RIs**: These are available to launch within the time windows you reserve. This option allows you to match your capacity reservation to a predictable recurring schedule that only requires a **fraction of a day, a week, or a month**.
	- Payment options for reserverd instances include All Upfront, Partial Upfront, and NoUpfront.
- With EC2 you are billed either by the **second**, for some Linux instances or by **hour**.
- with "**Inter-Region VPC Peering**" a company can connect their EC2 instances in <ins>*one region*</ins> with EC2 instances in <ins>*another region*</ins> using **private IP** addresses.

### AWS pricing policies
- pay-as-you-go
- save when you reserve
- pay less by using more

### AWS Cost Explorer
-  It is a free tool that allows you to **view charts** of your costs. You can view cost data for the **past 13 months** and **forecast** how much you are likely to spend over the **next three months**. Cost Explorer can be used to **discover patterns** in how much you spend on AWS resources over time and to **identify cost problem** area.

### AWS Cost Anomaly Detection
- Reduce cost surprises and enhance control without slowing innovation.
- Send alerts when anomalous spending is detected.

### Amazon Elastic Transcoder
- It **converts video and audio files** from their source format into versions that will **playback** on devices like smartphones, tablets and PC.

### AWS Organization
- **One bill provided** per AWS organization
- Best practices:
	-  Always enable **multi-factor** authentication (MFA) on the root account
	-  Always use a **strong and complex password** on the root account
	-  The **Paying account** should be used for **billing purposes only**. Do not deploy resources into the Paying account
-  With below options organizations can **reduce their cost**:
	-  "Create an AWS Organization configuration linking the accounts"
	-  "Setup consolidated billing between the accounts"
- Volume pricing discounts applied **across multiple accounts**.

### AWS Glue
- Is a fully managed **extract**, **transform**, and **load** (**ETL**) service that makes it easy for customers to prepare and load their <ins>data for analytics</ins>.

### AWS Artifact
- It is a self-service audit artifact retrieval **portal** that provides our customers with on-demand access to AWS’ compliance **documentation** and AWS **agreements**.
- You can use **AWS Artifact Reports** to download AWS security and compliance documents, such as <ins>AWS ISO certifications</ins>, <ins>Payment Card Industry (PCI)</ins>, and <ins>System and Organization Control (SOC) reports</ins>.
- It is **online**, self-service portal that AWS provides to enable customers to *view reports* and, such as *PCI reports*, and *accept agreements*.
- It is your **go-to**, central resource for compliance-related information that matters to you.

### AWS WAF
-  Is a **web application firewall** that protects against **common exploits** that could compromise application availability, compromise security or consume excessive resources.

### AWS Service Catalog
- It can be used to <ins>create and manage a selection of AWS services</ins> that are approved for use on AWS.
- These IT services **can include everything** from virtual machine images, servers, software, and databases to complete multi-tier application architectures.

### AWS Managed Services
- It manages the **daily operations** of your AWS infrastructure in alignment with **ITIL** processes and provides a **baseline integration** with IT Service Management (**ITSM**) tools such as the ServiceNow platform.

### Amazon Machine Image (AMI)
- It contains three catagories:
	- Community AMIs
	- AWS Marketplace AMIs
	- My AMIs
- It stores the **information** that defines an **EC2 instance** such as the template for the *root volume*, *launch permissions* and *block device mappings*.

### Five design principles for performance efficiency in the cloud
1. Democratize advanced technologies
2. Go global in minutes
3. Use serverless architectures
4. Experiment more often
5. Mechanical sympathy

### Five design principles for cost optimization in the cloud
1. Adopt a consumption model
2. Measure overall efficiency
3. Stop spending money on data center operations
4. Analyze and attribute expenditure
5. Use managed services to reduce cost of ownership

### Five design principles for reliability in the cloud
1. Test recovery procedures
2. Automatically recover from failure
3. Scale horizontally to increase aggregate system availability
4. Stop guessing capacity
5. Manage change in automation

### Six design principles for security in the cloud
1. Implement a strong identity foundation
2. Enable traceability
3. Apply security at all layers
4. Automate security best practices
5. Protect data in transit and at rest
6. Prepare for security events

### Five pillars of the AWS Well-Architected Framework
1. Operational excellence
2. security
3. reliability
4. performance efficiency
5. cost optimization

### Amazon S3 Transfer Acceleration
- It enables fast, easy, and secure **transfers** of files **over long distances** between your client and your Amazon S3 bucket.

### Amazon Neptune
- Amazon Neptune is a fast, reliable, fully-managed **graph database** service that makes it easy to build and run applications that work with highly connected datasets.

### Amazon Elasicsearch
- It is a fully managed Amazon search service b**ased on open source** software.

### AWS Direct Connect
- Benefits:
	- Reduce cost when using large volumes of traffic
	- Increase reliability (predictable performance)
	- Increase bandwidth (predictable bandwidth)
	- Decrease latency
- It uses <ins>private network connections</ins> (It's **NOT** based on internet connection)
- It is available in **1Gbps** and **10Gbps** speeds.
- When connecting to AWS over Direct Connect:
	- You can connect to all AZs **within the VPC** of the **local region**.
	- You can connect to public services in **remote regions**.
- You can use **AWS Direct Connect Gateway** for connecting a company from their on-premises network to VPCs in **multiple regions** using **private connections**

### AWS Snowball
- It is a **petabyte-scale** <ins>data transport</ins> solution that uses devices designed to be secure to transfer large amounts of data **into and out of** the AWS Cloud.

### Amazon Comprehend
- Amazon Comprehend is a natural language processing (**NLP**) service that uses **machine learning** to find insights and relationships in **text**.

### Amazon Resource Names (ARNs)
- It is used to **uniquely identify AWS resources**.

### Amazon ELB
- A **listener** is a process that checks for connection requests, using the protocol and port that you configure.
- Each listener has a default **rule**.
- Each rule **action** has a type.
- There are two types of **rule condition**:
	- host
	- path
- The primary **benefits** of using AWS ELB:
	- High availability
	- Elasticity

### AWS IoT Core
- It lets **connected devices** *easily* and *securely* interact with cloud applications and other devices.

### AWS Fargate
- Fargate <ins>removes the need to provision and manage servers</ins>.
- Amazon ECS is a container orchestration service used to provision and manage container clusters.
- It's **Serverless** offering (**no** EC2 instances)

### Amazon Detective
- It uses **machine learning** and **graph theory** capability collected log data to help you conduct faster and efficient security invedtigations.

### Amazon Global Accelerator
- You are asked to **improve the performance** of the application for <ins>local and global users</ins>. As part of this initiative, you must **monitor** the **application endpoint health** and **route traffic** to the most appropriate endpoint. For aiming this we should use amazon global accelerator.

### AWS Data Sync
- It is a simple and fast way to **move huge amounts** of data (hundreds of terabytes) between **on-premise** storage to **S3**, **EFS**, **FSx**.

### AWS CodePipeline
- AWS CodePipeline is a **continuous delivery service** you can use to **model**, **visualize**, and **automate the steps** required to release your software. You can quickly model and configure the different stages of a software release process. CodePipeline automates the steps required to release your software changes continuously.
- To orchestrate and **automate** the **various phases** involved in the release of application updates in-line with a predefined release model.

### Amazon GuardDuty
- Amazon GuardDuty is a **threat detection** service that **continuously monitors** your **AWS accounts** and **workloads** for malicious activity and delivers detailed security findings for visibility and remediation.
- For implementing a threat detection service that continuously monitors malicious activities and **unauthorized behaviors** protect AWS account, workloads and data stored in Amazon S3 we use this service.

### Amazon Macie
- It can be used to **detect users' personal credit card numbers** from data stored in Amazon **S3**.

### AWS X-Ray
- It is a service that helps developers **analyze** and **debug** distributed applications.

### AWS OpsWorks
- It is a service that allows you to host your own Puppet Enterprise infrastructure.

### Geographical Services
- Global level
	- AWS Route 53
	- AWS Cloud Front
	- AWS Direct Connect Gateway
	- AWS Global Accelerator
	- S3 (but data Regional)
	- IAM
	- WAF
	- AWS SNS
- Regional level
	- VPC
	- Security Groups
	- Resource Identifiers
 	- EFS	
	- ECS
	- ECR
	- Amazon GuardDuty
	- Amazon Detective
	- Amazon Inspector
	- Amazon Macie
	- AWS Security Hub
	- AWS Migration Hub
	- AWS Config
- Availability Zone level
	- Subnet
	- Elastic Load Balancer
	- EC2 Instances
	- EBS Volumes
	- Cluster Placement Groups

***
### Notes
- **Loose Coupling**: A desirable attribute of an IT system is that it can be broken into smaller, loosly coupled components.
- Amazon VPC is a **free of charge** service.
- Network ACLs operate at the **subnet** level NOT AZ level. It provides a firewall/security layer at the subnet level
- Network ACLs are **stateless** so you must create rules in both directions to allow traffic through.
- **Bootstrapping** and **Infrastructure as code** are two echniques for using automated, repeatable processes that are fast and avoid human error.
- **Golden Image Instances**: A golden image is a snapshot of a particular state for that resource. (e.g. EC2 instances, RDS instances, EBS volumes)
- "**Direct Connect**" and "**VPN CloudHub**" are two ways of connecting to an *Amazon VPC* from an *on-premise* data center.
- If you have **multiple VPN connections**, you can provide secure communication **between sites** using the **AWS VPN CloudHub**.
- Health Insurance Portability and Accountability Act of 1996 (**HIPAA**) is used for **secure AWS environment** to process, maintain and store protected health information.
- "**File Gateway**" and "**Gateway Virtual Tape Library**" are types of <ins>AWS storage gateway</ins>.
- "**virtual gateway**" on the <ins>VPC side</ins> and a **customer gateway** on <ins>the on-premise network side</ins> are need to connect VPC with a VPN connection (Those are <ins>parts of Amazon Managed VPN connection</ins>).
- *AWS Managed VPN* uses **internet connection**
- **Resource groups** make it easy to group resources using the tags that are assigned to them. You can group resources that share one or more tags
- "**PCI DSS**" is an **information security standard** applies to entities that store, process or transmit credit **cardholder data**.
- With the public cloud the consumer organization typically incurs **OPEX costs for usage**
- You **cannot detach** a primary network interface (**eth0**) from an instance. You can create and attach **additional** network interfaces.[elastic network interface(**ENI**)]
- **NAT instances** are managed by **you** and they must be **scaled manually** and <ins>do not privide HA</ins>. They can be used as **bastion** hosts and can be *assigned to security groups*.
- **NAT Gateway** are managed for you by **AWS**. They can **scale automatically** and they are **not** *associated with any security groups*. They are highly available in **each AZ**.
- You can use **DynamoDB** and **SWF** for create a "stateless" application
- These are valid use cases for using AWS services to implement **real-time auditing**:
	- Use Amazon Inspector to monitor for compliance
	- Use AWS Lambda to scan log files
- The options available in the **VPC Wizard** are:
	- VPC with a Single Public Subnet
	- VPC with Public and Private Subnets
	- VPC with Public and Private Subnets and Hardware VPN Access
	- VPC with a Private Subnet Only and Hardware VPN Access
- Only the **Memcached** and **Redis** database engines can be used with **ElastiCache**
- **AWS Migration Hub** provides a **single location** to <ins>track the progress of application migrations</ins> across multiple AWS and partner solutions.
- Amazon **CloudWatch**:
	- **Basic** monitoring: collects metrics **every 5 minutes**
	- **Detailed** monitoring: collects metrics **every 1 minute**
- Your payment model in cloud is operational (**OPEX**)
- "**AWS Concierge**" is available to support customers on an **Enterprise** support plan.
- You use a **key pair** to decrypt the Administrator password through the console or using the CLI (For Amazon EC2 **Windows** instance)
- An **RTMP** distribution (It is a type of Amazon CloudFront distribution) is used to distribute streaming media files using **Adobe Flash** Media Server’s RTMP protocol.
- The **public cloud** is offered under a purely **pay as you go** model, and allows companies to completely **avoid** *CAPEX costs*.
- **SQL** stands for *Structured Query Language*.
- AWS **Lambda** and Amazon **API Gateway** are both **app-facing** components of the AWS Serverless infrastructure.
- Amazon **DynamoDB** and **EFS** are *database and storage* services of the serverless infrastructure
- The *EC2 container registry* (**ECR**) is a managed AWS Docker registry service for storing, managing and deploying Docker images.
- **Amazon Aurora Multi-Master** can scale out **write** performance for their Amazon Aurora database across *multiple* availability zones.
- **Placement groups** are a logical grouping of instances in one of the following configurations:
	- A **Cluster**: It's a logical grouping on intances **within a single AZ**. Cluster placement groups are recommended for **applications** that benefit from **low network latency**, **high network throughput**, or both, and if the majority of the network traffic is between the instances in the group
	- A **spread**:  that are each placed on **distinct** underlying hardware. Spread placement groups are recommended for **applications** that have **a small number of critical instances** that should be kept separate from each other
- With "**EC2**, **Auto Scaling** and **E**lastic **L**oad **B**alancing" combination of AWS services could be used to deploy a **stateless** web application that can automatically and elastically scale.
- With the AWS cloud you get **fine-grained** billing and can **turn off resources** you are not using easily and not have to pay for them.
- To install a **PCI-compliant** workload on AWS:
	-  Use an AWS service that is in scope for PCI compliance and apply PCI controls at the application layer.
-  In IAM user access and secrert keys:
	-  The customer is responsible for **rotating** keys.
-  Which compute hosting model should be accounted for in the Total Cost of Ownership (TCO) when undertaking a cost analysis that allows physical isolation of a customer workload? **Dedicated Hosts**.
