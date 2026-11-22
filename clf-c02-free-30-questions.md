# AWS Cloud Practitioner (CLF-C02) — 30 Free Practice Questions

30 original practice questions from [CloudCert Path](https://cloudcertpath.com). Try them interactively — with instant scoring and no sign-up — at https://cloudcertpath.com/demo

Answers are hidden under each question. Pick yours first, then check.

Want all 300? The [Cloud Practitioner Practice Exam Pack](https://cloudcertpath.com) is $19 (12 months' access, one-time payment). The [Complete Bundle](https://cloudcertpath.com) ($29) adds cram notes and Anki flashcards.

These are original practice questions written from the public CLF-C02 exam guide and official AWS documentation. They are not real exam questions. We are not affiliated with, endorsed by, or sponsored by Amazon Web Services, Inc.

---

## Q001 — Domain 1: Cloud Concepts

A company wants to stop buying servers up front and instead pay only for the computing resources it actually uses. Which cloud benefit describes this?

A. Trade capital expense for variable expense
B. Elasticity
C. High availability
D. Fault tolerance

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. Trade capital expense for variable expense**

Pay-as-you-go replaces large up-front capital expenditure with variable operating expense. Elasticity (B) is scaling capacity up/down with demand, not the spending model itself.

Source: AWS Cloud Practitioner Essentials / AWS pricing overview — pay-as-you-go model.

</details>


## Q002 — Domain 1: Cloud Concepts

An application automatically adds EC2 instances when traffic rises and removes them when traffic falls. Which cloud concept is this?

A. Agility
B. Elasticity
C. Economies of scale
D. Global reach

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. Elasticity**

Elasticity is the ability to acquire resources as needed and release them when no longer needed. Agility (A) is speed of deploying resources, not automatic scaling.

Source: AWS Cloud Concepts — elasticity and scalability.

</details>


## Q003 — Domain 1: Cloud Concepts

A company moves an on-premises application to EC2 without changing its architecture. Which migration strategy is this?

A. Replatforming
B. Repurchasing
C. Rehosting ("lift and shift")
D. Refactoring

<details>
<summary>Answer &amp; explanation</summary>

**Answer: C. Rehosting ("lift and shift")**

Rehosting moves an application as-is to the cloud. Replatforming (A) makes small optimisations; refactoring (D) re-architects it, e.g. for cloud-native services.

Source: AWS Prescriptive Guidance — 7 Rs migration strategies.

</details>


## Q004 — Domain 1: Cloud Concepts

Which pillar of the AWS Well-Architected Framework focuses on the ability of a workload to recover from infrastructure or service disruptions?

A. Cost Optimization
B. Performance Efficiency
C. Operational Excellence
D. Reliability

<details>
<summary>Answer &amp; explanation</summary>

**Answer: D. Reliability**

Reliability covers recovering from failure, scaling to meet demand, and managing change. Operational Excellence (C) covers running and monitoring systems.

Source: AWS Well-Architected Framework — six pillars.

</details>


## Q005 — Domain 1: Cloud Concepts

Under the AWS Shared Responsibility Model, which task is always the customer's responsibility?

A. Managing user access and permissions to AWS resources
B. Patching the physical host hardware
C. Securing the physical data centre
D. Maintaining the virtualization layer

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. Managing user access and permissions to AWS resources**

AWS is responsible for security of the cloud (physical hosts, virtualization, facilities); the customer is responsible for security in the cloud, including IAM users, permissions, and its own data.

Source: AWS Shared Responsibility Model documentation.

</details>


## Q006 — Domain 1: Cloud Concepts

A startup with unpredictable traffic wants to deploy its application in minutes, without buying hardware, and test new ideas quickly. Which benefit of the AWS Cloud best describes this?

A. Go global in minutes
B. Increase speed and agility
C. Benefit from massive economies of scale
D. Trade capital expense for variable expense

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. Increase speed and agility**

Speed and agility is the ability to provision and experiment quickly. Global reach (A) is about deploying in multiple Regions; economies of scale (C) is about lower unit costs from AWS's size.

Source: AWS Cloud Practitioner Essentials — six advantages of cloud computing.

</details>


## Q007 — Domain 1: Cloud Concepts

Which AWS Cloud Adoption Framework (CAF) perspective focuses on business value, outcomes, and the business case for cloud migration?

A. Platform perspective
B. Security perspective
C. Business perspective
D. Operations perspective

<details>
<summary>Answer &amp; explanation</summary>

**Answer: C. Business perspective**

The CAF Business perspective covers business capabilities, value realisation, and investment justification. Platform (A) covers infrastructure and applications; Operations (D) covers running workloads.

Source: AWS Cloud Adoption Framework. --- ## Domain 2 — Security and Compliance (Q8–Q16)

</details>


## Q008 — Domain 2: Security and Compliance

Which AWS service is used to create and manage users, groups, and permissions for accessing AWS resources?

A. AWS Organizations
B. AWS Key Management Service (AWS KMS)
C. Amazon Cognito
D. AWS Identity and Access Management (IAM)

<details>
<summary>Answer &amp; explanation</summary>

**Answer: D. AWS Identity and Access Management (IAM)**

IAM controls who can do what in an AWS account. KMS (B) manages encryption keys; Cognito (C) is for application user sign-in.

Source: AWS IAM User Guide.

</details>


## Q009 — Domain 2: Security and Compliance

What is the recommended first security step for the AWS account root user?

A. Enable multi-factor authentication (MFA) on the root user and use it only when necessary
B. Create an access key for the root user
C. Share the root user credentials with the whole team
D. Delete the root user

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. Enable multi-factor authentication (MFA) on the root user and use it only when necessary**

The root user cannot be deleted, but it should be locked down with MFA and used rarely; day-to-day work should use IAM users/roles with least privilege.

Source: AWS IAM best practices — securing the root user.

</details>


## Q010 — Domain 2: Security and Compliance

A security group allows inbound SSH (port 22) from a specific IP address. A network ACL (NACL) on the same subnet denies all inbound traffic. What happens to an SSH connection attempt from that IP?

A. It is allowed, because security groups take precedence
B. It is denied, because the NACL is evaluated and denies it
C. It is allowed, because NACLs are stateless and do not block return traffic
D. It is denied only if the security group is also stateful

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. It is denied, because the NACL is evaluated and denies it**

Both layers are evaluated. Security groups are stateful and NACLs are stateless, but a NACL deny blocks the traffic regardless of the security group allow.

Source: Amazon VPC documentation — security groups vs network ACLs.

</details>


## Q011 — Domain 2: Security and Compliance

Which AWS service continuously monitors an account for malicious activity and unauthorised behaviour, such as unusual API calls?

A. AWS CloudTrail
B. AWS Config
C. Amazon GuardDuty
D. AWS Trusted Advisor

<details>
<summary>Answer &amp; explanation</summary>

**Answer: C. Amazon GuardDuty**

GuardDuty is a threat-detection service. CloudTrail (A) records API activity (the data GuardDuty can analyse); Config (B) records configuration changes.

Source: Amazon GuardDuty documentation.

</details>


## Q012 — Domain 2: Security and Compliance

A company must prove to an auditor that its use of AWS meets a specific compliance standard. Which AWS resource provides on-demand access to AWS compliance reports and certifications?

A. AWS Config
B. AWS Security Hub
C. AWS Systems Manager
D. AWS Artifact

<details>
<summary>Answer &amp; explanation</summary>

**Answer: D. AWS Artifact**

AWS Artifact is the portal for AWS compliance reports (e.g. SOC, ISO). Config (A) records the configuration history of your own resources.

Source: AWS Artifact documentation.

</details>


## Q013 — Domain 2: Security and Compliance

Which service provides a central, encrypted audit log of API calls made in an AWS account?

A. AWS CloudTrail
B. Amazon CloudWatch
C. AWS Config
D. Amazon Inspector

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. AWS CloudTrail**

CloudTrail logs API activity (who did what, when). CloudWatch (B) collects metrics and logs from resources; Config (C) tracks resource configuration history.

Source: AWS CloudTrail documentation.

</details>


## Q014 — Domain 2: Security and Compliance

A company stores sensitive files in Amazon S3 and wants them encrypted at rest using keys it fully controls, including key rotation and usage policies. Which service should it use?

A. AWS Secrets Manager
B. AWS Key Management Service (AWS KMS)
C. AWS Certificate Manager (ACM)
D. AWS Shield

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. AWS Key Management Service (AWS KMS)**

KMS creates and controls encryption keys, including customer-managed keys with rotation. Secrets Manager (A) stores secrets such as passwords; ACM (C) manages TLS certificates.

Source: AWS KMS documentation; Amazon S3 server-side encryption.

</details>


## Q015 — Domain 2: Security and Compliance

Following the principle of least privilege, how should permissions normally be granted?

A. Give every user administrator access, then remove what they do not use
B. Use one shared IAM user for the whole team
C. Grant only the minimum permissions needed to perform a task
D. Attach the same managed policy to every role

<details>
<summary>Answer &amp; explanation</summary>

**Answer: C. Grant only the minimum permissions needed to perform a task**

Least privilege means granting only the permissions required for the job, typically via IAM roles and policies scoped to specific actions and resources.

Source: AWS IAM best practices.

</details>


## Q016 — Domain 2: Security and Compliance

Which AWS service protects web applications from common exploits such as SQL injection and cross-site scripting, by filtering HTTP requests?

A. AWS Shield
B. Amazon GuardDuty
C. AWS Firewall Manager
D. AWS WAF

<details>
<summary>Answer &amp; explanation</summary>

**Answer: D. AWS WAF**

AWS WAF is a web application firewall for HTTP(S) filtering. Shield (A) protects against DDoS attacks; Firewall Manager (C) centrally manages WAF/Shield rules.

Source: AWS WAF documentation. --- ## Domain 3 — Cloud Technology and Services (Q17–Q26)

</details>


## Q017 — Domain 3: Cloud Technology and Services

A developer wants to run code in response to an event without provisioning or managing any servers. Which AWS service is the best fit?

A. AWS Lambda
B. Amazon EC2
C. Amazon ECS on EC2
D. Amazon Lightsail

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. AWS Lambda**

Lambda is serverless — AWS runs the code on demand and manages the infrastructure. EC2 (B) requires managing virtual servers.

Source: AWS Lambda documentation.

</details>


## Q018 — Domain 3: Cloud Technology and Services

A company needs to store archived data that is rarely accessed and can tolerate a retrieval time of several hours, at the lowest possible storage cost. Which S3 storage class is the best fit?

A. S3 Standard
B. S3 Glacier Deep Archive
C. S3 Standard-Infrequent Access
D. S3 Intelligent-Tiering

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. S3 Glacier Deep Archive**

S3 Glacier Deep Archive is the lowest-cost class, designed for data accessed rarely with retrieval in hours (Standard retrieval within 12 hours, Bulk within 48 hours). Standard (A) is for frequent access.

Source: Amazon S3 storage classes documentation.

</details>


## Q019 — Domain 3: Cloud Technology and Services

Which AWS database service is a fully managed, serverless NoSQL key-value/document database that delivers single-digit millisecond performance at any scale?

A. Amazon RDS
B. Amazon Aurora
C. Amazon DynamoDB
D. Amazon Redshift

<details>
<summary>Answer &amp; explanation</summary>

**Answer: C. Amazon DynamoDB**

DynamoDB is NoSQL (key-value/document). RDS/Aurora (A/B) are relational; Redshift (D) is a data warehouse for analytics.

Source: Amazon DynamoDB documentation.

</details>


## Q020 — Domain 3: Cloud Technology and Services

A company deploys its application across two Availability Zones in the same Region so that it stays available if one zone fails. Which AWS concept is this using?

A. Edge locations
B. A single Region with a single VPC
C. AWS Direct Connect
D. High availability through multiple Availability Zones

<details>
<summary>Answer &amp; explanation</summary>

**Answer: D. High availability through multiple Availability Zones**

Availability Zones are isolated data centres within a Region; spreading across them protects against a single-zone failure. Edge locations (A) serve CloudFront cached content, not AZ redundancy.

Source: AWS Global Infrastructure documentation.

</details>


## Q021 — Domain 3: Cloud Technology and Services

Which AWS service distributes incoming application traffic across multiple EC2 instances in different Availability Zones?

A. Elastic Load Balancing (ELB)
B. Amazon Route 53
C. Amazon CloudFront
D. Amazon VPC

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. Elastic Load Balancing (ELB)**

ELB distributes traffic to healthy targets. Route 53 (B) is DNS; CloudFront (C) is a content delivery network.

Source: Elastic Load Balancing documentation.

</details>


## Q022 — Domain 3: Cloud Technology and Services

A company wants its static website content delivered to users worldwide with low latency from locations close to them. Which service should it use?

A. Amazon S3 Glacier
B. Amazon CloudFront
C. AWS Direct Connect
D. Amazon EFS

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. Amazon CloudFront**

CloudFront is a CDN that caches content at edge locations near users. Direct Connect (C) is a private network link to AWS, not content delivery.

Source: Amazon CloudFront documentation.

</details>


## Q023 — Domain 3: Cloud Technology and Services

A company runs a relational database and wants AWS to handle patching, backups, and failover, while it keeps control of the database engine and schema. Which service is the best fit?

A. Amazon DynamoDB
B. Amazon EC2 with a self-installed database
C. Amazon RDS
D. Amazon S3

<details>
<summary>Answer &amp; explanation</summary>

**Answer: C. Amazon RDS**

RDS is a managed relational database service (MySQL, PostgreSQL, etc.) that automates patching, backups, and Multi-AZ failover. Self-installing on EC2 (B) leaves that work to the customer.

Source: Amazon RDS documentation.

</details>


## Q024 — Domain 3: Cloud Technology and Services

An application needs to decouple its components so that a spike in orders does not overwhelm the processing service. Which AWS service provides a managed message queue for this?

A. Amazon SNS
B. Amazon EventBridge
C. AWS Step Functions
D. Amazon SQS

<details>
<summary>Answer &amp; explanation</summary>

**Answer: D. Amazon SQS**

SQS is a message queue — producers send messages, consumers process them at their own pace. SNS (A) is pub/sub notification (fan-out), not a queue.

Source: Amazon SQS documentation.

</details>


## Q025 — Domain 3: Cloud Technology and Services

Which AWS service collects metrics and logs from AWS resources and lets a user set alarms, for example when CPU utilisation exceeds 80%?

A. Amazon CloudWatch
B. AWS CloudTrail
C. AWS Config
D. AWS Trusted Advisor

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. Amazon CloudWatch**

CloudWatch monitors metrics/logs and alarms. CloudTrail (B) logs API calls; Config (C) tracks configuration changes.

Source: Amazon CloudWatch documentation.

</details>


## Q026 — Domain 3: Cloud Technology and Services

Which service provides DNS, domain registration, and health-check-based routing to AWS resources?

A. AWS Global Accelerator
B. Amazon Route 53
C. Amazon VPC
D. AWS Transit Gateway

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. Amazon Route 53**

Route 53 is AWS's DNS service (plus domain registration and health checks). Global Accelerator (A) improves performance for TCP/UDP traffic.

Source: Amazon Route 53 documentation. --- ## Domain 4 — Billing, Pricing and Support (Q27–Q30)

</details>


## Q027 — Domain 4: Billing, Pricing, and Support

A workload runs steadily 24 hours a day, 7 days a week, with predictable capacity needs for the next year. Which EC2 pricing option gives the largest discount for this pattern?

A. On-Demand Instances
B. Spot Instances
C. Reserved Instances (or a Savings Plan) with a 1- or 3-year commitment
D. Dedicated Hosts with no commitment

<details>
<summary>Answer &amp; explanation</summary>

**Answer: C. Reserved Instances (or a Savings Plan) with a 1- or 3-year commitment**

A long-term commitment (Reserved Instances / Savings Plans) gives the deepest discount for steady usage. Spot (B) can be cheaper per hour (up to ~90% off) but can be interrupted with two minutes' notice, so it does not fit a steady, must-not-stop workload.

Source: Amazon EC2 pricing documentation.

</details>


## Q028 — Domain 4: Billing, Pricing, and Support

A company wants to be alerted when its monthly AWS spending is forecast to exceed a set amount. Which service should it use?

A. AWS Cost Explorer
B. AWS Pricing Calculator
C. AWS Cost and Usage Report only
D. AWS Budgets

<details>
<summary>Answer &amp; explanation</summary>

**Answer: D. AWS Budgets**

AWS Budgets lets you set cost/use budgets and sends alerts when actual or forecast spend crosses a threshold. Cost Explorer (A) is for analysing past spend.

Source: AWS Budgets documentation.

</details>


## Q029 — Domain 4: Billing, Pricing, and Support

A company has several AWS accounts (development, testing, production) and wants one payer account with a single combined bill and volume discounts. Which feature provides this?

A. AWS Organizations with consolidated billing
B. AWS Cost Explorer
C. AWS IAM
D. AWS Control Tower only

<details>
<summary>Answer &amp; explanation</summary>

**Answer: A. AWS Organizations with consolidated billing**

AWS Organizations lets multiple accounts bill to one payer account (consolidated billing), pooling usage for volume discounts.

Source: AWS Organizations documentation — consolidated billing.

</details>


## Q030 — Domain 4: Billing, Pricing, and Support

Before launching a new project, a team wants to estimate its monthly AWS cost based on the services and usage it expects. Which tool is designed for this?

A. AWS Trusted Advisor
B. AWS Pricing Calculator
C. AWS Budgets
D. AWS Support Center

<details>
<summary>Answer &amp; explanation</summary>

**Answer: B. AWS Pricing Calculator**

The AWS Pricing Calculator estimates costs for a planned architecture. Trusted Advisor (A) checks an existing account for cost optimisation opportunities.

Source: AWS Pricing Calculator documentation. ---

</details>

---

Good luck. 🍀
