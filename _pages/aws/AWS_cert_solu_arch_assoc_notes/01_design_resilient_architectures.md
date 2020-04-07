---
layout: page
title: AWS Design Resilient Architectures
permalink: /aws_dra
---

34% of exam

EC2 Instance Store. Ephemeral volumes. Only certain EC2 instances are stored. Fixed capacity. Application level durable.
- Used for storing temperary data, but not affected by ephemeral. 

Elastic Block Store. Encrpytion and snapshots. Provisionable capacity. Independent lifecycle. Can stop or preserve and 
connect to EC2. Durable, attachable storage for EC2.
- SSD and HDD
- SSD types: general purpose and provisional IOPs (scale up easy)
- HDD types: general purpose and cold

Third option for storage is Amazon EFS (elastic file system). 
- Multiple EC2 can reach the same EFS.
- Elastic
- NFS v4.0
- Compatible with Linux AMIs

EFS can only attach to one VPC at a time. The most common model is S3. It is implemented as a distributed model. 
The S3 is eventually consistent across redundancies. S3 standard is cheaper for upload/download, most for access. 

Access through IAM, bucket policy, or IALs. Virtually unlimited. Region scoped. Design for eleven 9's.

EFS: Elastic File service

S3: Distributed system, is it strongly consistent for new objects and eventually consistent 
for older objects. It is a scaled, distributed service. Offers the Standard and Standard-IA modes.

Loosely coupled services are most easily scaled and more fault tolerant.

An AWS load balancer can help build loosely coupled architectures.

CloudFormation: Declaritive programming language for deploying AWS Resources. Uses templates and stacks to provision 
resources. CRUD a whole stack. 

AWS Lambda: Fully managed compute service that runs stateless code in response to an event or on a time
based interval.

Allows you to run code without managing infrustructure like EC2 and auto scaling groups.

Test Axioms:
Expect single AZ will never by the answer. AWS managed service always preferred.
Fault tolerant and high availability are not the same things. Expect that everything will fail at some point.
