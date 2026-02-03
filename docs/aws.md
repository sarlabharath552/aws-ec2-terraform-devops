# AWS Core Concepts – EC2 and Cloud Fundamentals
## Introduction
Amazon Web Services (AWS) is a cloud service provider that offers on-demand computing resources such as servers, storage, and networking. Cloud computing allows organizations to avoid managing physical infrastructure and instead use scalable resources over the internet.

This document explains the core AWS concepts required to understand EC2 and cloud infrastructure from a DevOps perspective.

---

## What is Cloud Computing?
Cloud computing is the delivery of computing services like servers, storage, databases, and networking over the internet. It provides flexibility, scalability, and cost efficiency through a pay-as-you-go model.

Key benefits:
- No physical hardware management
- High availability
- Scalability on demand
- Reduced operational cost

---

## AWS Regions and Availability Zones
- **Region**: A geographic location where AWS hosts its data centers (example: eu-north-1 – Stockholm).
- **Availability Zone (AZ)**: An isolated data center within a region designed for fault tolerance.

Using multiple AZs improves application reliability.

---

## Amazon EC2 (Elastic Compute Cloud)
Amazon EC2 provides virtual servers called instances. These instances allow users to run applications and workloads in the cloud.

Key features:
- Resizable compute capacity
- Full control over operating system
- Secure and scalable
- Pay only for usage

EC2 is commonly used for hosting backend services, APIs, and development environments.

---

## Amazon Machine Image (AMI)
An AMI is a template used to launch EC2 instances. It contains:
- Operating system
- Preinstalled software
- Configuration settings

Example AMIs:
- Amazon Linux 2
- Ubuntu

AMI IDs are region-specific.

---

## Instance Types
Instance types define CPU, memory, and networking capacity.

Example:
- `t3.micro`: Free Tier eligible, suitable for learning and testing.

---

## Key Pair
A key pair is used for secure authentication when connecting to EC2 instances via SSH.

It consists of:
- Public key (stored in AWS)
- Private key (.pem file stored by the user)

The private key must be kept secure.

---

## Security Groups
Security groups act as virtual firewalls for EC2 instances. They control inbound and outbound traffic.

Example rules:
- Allow SSH (port 22)
- Allow HTTP (port 80)

---

## Virtual Private Cloud (VPC)
A VPC is a logically isolated network in AWS where resources are launched. AWS provides a default VPC suitable for beginners.

---

## AWS Free Tier
AWS Free Tier allows limited usage of services such as EC2 (750 hours per month of t2/t3.micro).

Resources should be terminated after use to avoid billing.

---

## Summary
Understanding AWS core concepts is essential before automating infrastructure using tools like Terraform. These fundamentals form the backbone of cloud and DevOps engineering.
