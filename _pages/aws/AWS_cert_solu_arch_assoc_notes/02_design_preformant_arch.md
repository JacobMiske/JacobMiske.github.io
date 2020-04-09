---
layout: page
title: AWS Design Preformant Architectures
permalink: /aws_dpa
---

24% of exam

#### 2.1: Choose Performant Storage and DBs
EBS volume types: SSD and HDD

SSH has a higher IOPS performance. More costly.

High performing arch offloads static content to S3. Dramatically improves web server performance.

In S3, the name is specific to the region. They are globally unique however. The path after the bucket name is the key.

Pay for GBs per month, transfer out of region, and PUT/COPY/POST/etc.

There are two S3 storage classes. Standard and Infrequent-Access.

Lifecycle policies can automatically move S3 data from standard to IA to glacier... and eventually delete.

##### Databases
Amazon RDS:

Managed relational database. Complex transactions or complex queries. medium to high write rate. High durability.

Amazon no-sql on Dynamo DB:

Good for massive read/write and sharding. Scales horizontally fast. Read capacity is up to 4kB. Write cap is up to 1kB.
One strongly consistent read/s. Two eventually consistent reads per second. One write per second.

Data warehouse with redshift, sql interface. Getting aggregate numbers on tables.

#### 2.2: Apply caching to improve performance

#### 2.3: Design Solutions for Elasticity and Scalability
