---
layout: page
title: Code; Things related to computer science
permalink: /cs/
---

# Table of Contents
<a href="/jsreading/">JS Readings</a>

<a href="/codecomplete/">Code Complete</a>


# Goals
- Gain competency in Microsoft Azure through Fundamentals certification and beyond
- Gain competency in Amazon Web Services through Associate certification and beyond
- Prove ability in React JS Front End development
- Prove knowledge in novice level C++ or C# development
- Prove awareness and/or knowledge in the realm of product ownership
- Prove ability in breadth of engineering knowledge surrounding software engineering

## Certifications

### Azure
<a href="/azure_notes/">Azure Notes</a>

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

