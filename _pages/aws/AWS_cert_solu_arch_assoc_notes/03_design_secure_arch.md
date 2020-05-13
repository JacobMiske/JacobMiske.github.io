---
layout: page
title: AWS Design Secure Architectures
permalink: /aws_dsa
---

24% of exam

Shared responsibility model: AWS is responsible for their security in the cloud. AWS is responsibly for the security
of the cloud itself.

Principle of least privilege: Persons can perform all activities for their specific jobs and no more.1

IAM: Centrally manage user permissions in AWS. Create users, groups, and policies.

IAM integrates with Microsoft Azure Directory and AWS Directory service using SAML identity federation.

### Domain 3.1: Determine how to secure application tiers

### Determine how to secure data


### Define the networking infrastructure for a VPC network
Virtual private cloud is organized by subnets, set of private IP addresses. Network isolation. Control NAT gateways.

Use subnets to define internet accessibility. Public subnets support inbound/outbound access to the public.

Security groups and Access Control Lists are used to limit access. SGs are stateful. ACLs are stateless.1

Use security groups to control traffic in and out of services.
