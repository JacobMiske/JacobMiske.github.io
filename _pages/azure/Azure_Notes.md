---
layout: page
title: Azure Notes
permalink: /azure_notes
---

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
Only procure what you will use. 

##### Essential Azure compute concepts
Azure compute: a on-demand computing service. Four main techniques; VM, containers, 
azure app service, and serverless computing.
##### Explore Azure VMs
Options: total control over OS, ability to run custom software, custom hosting config.
Use: During test and dev, cloud apps, extend datacenter, disaster recovery.
Easy to shift operations to the cloud first as opposed to other options.

You can run single VM for testing. Availability set: logical grouping of two or more VM 
that keep an app running during maintenance.

Azure batch: enables large-scale job scheduling and compute management with scale ability
 to tens, hundreds, or thousands of VMs. Uses: Start a pool of compute VMs. Install apps and stage
 data. Run jobs with many tasks. ID failures. Requeues work. Scales down as work completes.
 
##### Explore Containers in Azure
Azure supports Docker containers in Azure Container Instances (ACI) and Azure Kubernetes
Service (AKS).

#### Explore Azure App Service
Enables to build and host web apps, background jobs, mobile backends, REST APIs.
Auto scaling and high availability. Is a PAAS.

Uses: Web apps, API Apps, WebJobs, Mobile Apps.

##### Explore Serverless Computing in Azure
1. Abstractions of servers

2. Event-driven scale

3. Micro-billing

Two implementations of serverless compute. Azure functions and Azure logic apps.

Azure functions can execute code in almost any language. Azure logic apps designed in a
web-based designer and can execute logic triggered by Azure services without any code.

Function vs Logic App

State: Normally stateless, durable functions provide state. VS Stateful

Development: Code-first (imperative) VS designer-first (declaritive)

Connectivity: Dozen built-in binding types, write code for customs VS large collection of connectors, 

## Azure Data Storage Options
How Azure can meet business storage needs:

### Azure SQL Database: 
A relational DAAS based on the latest stable version of the Microsoft SQL Server database engine. 

You can migrate existing SQL Server databases with minimal downtime using the Azure Database Migration service.

The service uses the Microsoft Data Migration Assistant, it generates assessment reports that provide recommendations to
help guide the user through any required changes prior to a migration. Once you assess and perform any 
remediation required, you're ready to begin the mibration process. The Azure Database Migration Service performs all of
the migration process. 

### Azure Cosmos DB: 
A globally distributed database service. It supports schema-less data that lets you build highly 
responsive and Always On applications to support constantly changing data. You can use this feature to store data that 
is updated and maintained by users around the world.

### Azure Blob Storage: 
An unstructured storage. Meaning there are no restrictions on the kinds of data it can hold. Blobs 
are highly scalable and apps work with blobs in much the same way as they would work with files on a disk, such as
reading and writing data. Blob Storage can manage thousands of simultaneous uploads, massive amount of video data,
constantly growing log files, and can be reached from anywhere with an internet connection.

### Azure Data Lake Storage:

The Data Lake feature allows you to perform analytics on your data usage and prepare reports. Data Lake is a large
repository that stores both structured and unstructued data.

Azure Data Lake Storage combines the scalability and cost benefits of object storage with the reliability and 
performance of the Big Data file system capabilities. The following illustration shows how Azure Data Lake stores all 
your business data and makes it available for analysis.

Azure Files: Azure Files gives fully managed file shares in the cloud accessible via the industry standard Server 
Message Block (SMB) protocal. Azure file shares can be mounted by cloud or on-premises deployments of Windows, Linux,
and macOS.

### Azure Queue:

Azure Queue storage is a service for storing large numbers of messages that can be accessed from anywhere in
the world. Queue storage can be used to help build flexible applications and separate functions for better
durability across large workloads. 

- Create a backlog of work and to pass messages between different Azure web servers.
- Distribute load among different web servers/infrastructure and to manage bursts of traffic.
- Build resislience against component failure when multiple users access your data at the same time.

### Disk Storage
Provides disks for VM, apps, and other services to access and use as they need. Variety of SSH and HDDs options
to choose from.

Storage Tiers:

Hot storage tier, Cold storage tier, and Archive storage tier.

Encryption and Replication:

Azure Storage Service Encryption (SSE) and Client-side encryption.

## Azure Networking Options
- How an Azure VPM provides secure network comms among resources such as VMs and other networks.
- What high availability and resiliency mean and how Azure Load Balancer can increase resiliency within a single 
geographic region.
- What latency is and how Traffic Manager helps reduce network latency and provides resiliency across geo regions.

There are several strategies employed by software architects and designers to make these complex systems easier to 
build, manage, and maintain. Let's look at a few of them, starting with loosely coupled architectures.

An N-tier arch. is loosely architected. The web tier provides the web interface to users on the browser.

The app tier runs business logic (user#1023 clicked here and there, CRUD).

The data tier includes DB and other storage that hold product info and customer orders.

### Scale with Azure Load Balancer
If the traffic is a HTTP, a potentially better option is to use Azure Application Gateway. This tool is
a load balancer designed for web applications. It uses Azure Load Balancer at the transport level (TCP) 
and applies sophisticated URL based routing rules to support advanced scenarios.

## Security, Responsibility, and Trust in Azure
Every system needs to be built with security in mind. Azure Event Hubs allow you to receive and process millions of 
events in real-time data each second via dynamic data pipelines. Event hubs also integrates seamlessly with other Azure
services.

There is a security advantage in using the cloud; assuming the cloud is well secured internally.

A good place to check for Azure solutions is the Azure Security Center.

#### Identity and Access
Two fundamental concepts need to be differentiated when talking about identity and access control. 

- Authentication: is the process of establishing the identity of a person or service looking to access a resource. It
involves the act of challenging a party for legitimate credentials, and provides the basis for creating a security 
principle for IAM use. It establishes if they are who they say they are. (AuthN)

- Authorization: is the process of establishing what level of access an authenticated person or service has. It specifies
what data they're allowed to access and what they can do with it. (AuthZ)

#### Encryption

Encryption is the process of making data unreadable and unusable to unauthorized users. To use or read the encrypted 
data, it must be decrypted, which requires use of a key. There are two top-level types of encryption. Symmetric and 
asymmetric.

- Symmetric encryption: Uses the same key to encrypt and decrypt the data. 

- Asymmetric encryption: Uses a public key and a private key. Useds for things like Transport Layer Security (TLS)
which is used online (HTTPS) and data signing.

#### Protect Your Network

Internet protection: use a firewall, a service that grants access based on the IP address of the requests. 

