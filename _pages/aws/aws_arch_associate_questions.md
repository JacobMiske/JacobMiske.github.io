---
layout: page
title: AWS Arch. Associate Questions
permalink: /aws_arch_associate_questions
---

# Domain 1: Design Resilient Architectures

### Question 1.2
Which of the two following AWS Services facilitates the implementation of loosely coupled architectures?

- A: AWS CloudFormation
- B: Amazon Simple Queue Service
- C: AWS CloudTrail
- D: Elastic Load Balancing
- E: Amazon Elastic MapReduce 

Solution: A and C. AWS CloudFormation stands up stacks of components, not A. AWS SQS is a logging service, not C. 
And Amazon Elastic MapReduce is a managed Hadoop service, not E.

### Question 1.3
Your web service has a performance SLA to respond to 99% of requests in <1 second. Under normal and heavy operations, 
distributing request over four instances meets performance requirements. 

What architectures ensures cost efficient, high availability of the service if an AZ becomes unavailable?

- A: Deploy on four servers in one AZ
- B: Deploy on six servers in one AZ
- C: Deploy on four servers across two AZ
- D: Deploy on eight servers across two AZ

Solution: C, need at least two AZ and eight is not cost effective.

### Question 1.4
Your web service has a performance SLA to respond to 99% of requests in <1 second. Under normal and heavy operations, 
distributing request over four instances meets performance requirements. 

What architectures ensures cost efficient, fault tolerant of the service if an AZ becomes unreachable?

- A: Deploy on four servers in one AZ
- B: Deploy on six servers in one AZ
- C: Deploy on four servers across two AZ
- D: Deploy on eight servers across two AZ

Solution: D, need at least two AZ and eight is necessary for fault tolerance.

### Question 1.5
You are planning to use CloudFormation to deploy a Linux EC2 instance in two different regions using the same base
Amazon Base Image.

How can you do this with CF?

- A: Use Two different tempaltes since CF templates are region specific
- B: Use mappings to specify the base AMI since AMI IDs are different in each region
- C: Use parameters to specify the base AMI since AMI IDs are different in each region
- D: AMI IDs are identical across regions

Solution: B, AMI ids are different across regions and a mapping is used for the same CF template

### Question 1.6
How can I access print statements from AWS Lambda?

- A: SSH into lambda and look at system logs
- B: Lambda writes all output to S3
- C: CloudWatch logs
- D: Print statements are ignored in Lambda

Solution: C

### Question 1.7
You are running an EC2 instance which uses EBS for storing its state. You take an EBS snapshot every day. 
When the system crashes, it takes you 10 minutes to reset. What are RTO and RPO?

RTO: Recovery time objective, measured by time to reset
RPO: Recovery Point Objective, measured by data lost in time down

- A: RTO is 1 day, RPO is 10 minutes
- B: RPO is 1 day, RTO is 10 minutes
- C: Both are 10 min
- D: Both are 1 day

Solution: B

# Question 2.1
In what ways does S3 object storage differ from block storage and file storage (3).

- A: S3 allows storing an unlimited number of objects
- B: Objects are immutable
- C: Object are replicated across AZ
- D: Objects are replicated across regions

Solution: A,B,C

# Question 2.2
Which of the following are features of Amazon EBS? (2)

- A: Data stored on EBS is auto backed up to an AZ
- B: EBS data is backed up on tape
- C: EBS volumes can be encrypted
- D: Data on EBS is lost when the attached instance is stopped

Solution: A,C

# Question 2.3
Which RDS database engines support read replica?

- A: Microsoft SQL Server and Oracle
- B: MySQL, MariaDB, PostgreSQL, and Aurora
- C: Aurora, Microsoft SQL Server, and Oracle
- D: MySQL and PostgreSQL

Solution: B
