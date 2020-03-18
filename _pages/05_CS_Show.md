---
layout: page
title: CS Show
permalink: /cs/
---

# Goals
- Gain competency in Microsoft Azure through Fundamentals certification and beyond
- Gain competency in Amazon Web Services through Associate certification and beyond
- Prove ability in React JS Front End development
- Prove knowledge in novice level C++ or C# development
- Prove awareness and/or knowledge in the realm of product ownership
- Prove ability in breadth of engineering knowledge surrounding software engineering

## Certifications

### Azure

#### Core Cloud Services - Azure Architecture and Service Guarentees
Region is a geographical area with at least one datacenter. When a resource is deployed on Azure, the user 
chooses the region where the resource is deployed. Exceptions are some services are only available in some 
regions, such as VM size or storage types. Some global Azure services do not need the user to select a region 
such as the Azure Active Directory, Traffic Manager, or DNS. Over 54 total regions.

Availability Zones

Each AZ is made up of one or more datacenters with independent systems. If one goes down the other can continue to work.
Availability zones are connected by fiber. Region pairs are identical resources running in two datacenters in the same
geography.

SLA: Service Level Agreement

SLA describe Microsoft's commitment to providing Azure customers with specific performance standards. There are SLAs for
individual products and services. SLAs specify what happens if a product fails to perform a governing SLA specification.

MONTHLY UPTIME PERCENTAGE and SERVICE CREDIT PERCENTAGE

< 99.9 10; < 99 25; < 95 100

#### Core Cloud Services - Manage services with the Azure portal
Tools for use day-to-day with Azure. The Portal (GUI), Powershell and Azure CLI, Cloud Shell, Azure mobile app.

Azure marketplace is where you create new resources.

#### Core Cloud Services - Azure Compute Options




## Amazon Web Services

### AWS Certi. Solution Architect

Most popular. Needed for speciality exams. Prereq for professional. To do well, 
familiar with core services and how best to use them to follow best practices.

Multiple choice. No penalty for guessing.

130 minutes to complete the exam. Mark for future consideration. 65 questions. 

#### Domain 1: Design Resilient Architecture
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

##### 1.1: Choose Reliable Resilient Storage

Even in disaster, you don't lose data or state. 

##### 1.2: Decoupling mechanisms using AWS Services

Made easy with AWS

##### 1.3: How to Design a Multi-Tier Architecture Solution

Naturally decoupled.

##### 1.4: How to Design High Availability and/or Fault Tolerant Solutions

Operating at scale, failure should be treated as a normal operation which is handled.




#### Domain 2: Define Performant Solutions
24% of exam

#### Domain 3: Specify Secure Applications and Architectures
26% of exam

#### Domain 4: Design Cost-Optimized Architectures
10% of exam

#### Domain 5: Define Operationally Excellent Architectures
6% of exam




## Skills 

## Languages

#### Python


#### C++


#### Ruby


#### HTML, CSS, JS
Using React

{% raw %}
{% if page.lang == 'en' %}
    {{ page.date | date: "%d/%m/%Y" }}
{% endif %}
{% endraw %}

