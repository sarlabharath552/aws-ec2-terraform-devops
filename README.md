# AWS EC2 & Terraform – DevOps Internship Task

## Introduction
This repository documents my hands-on learning and implementation of AWS EC2 and Terraform as part of my DevOps internship. The goal of this task was to understand cloud infrastructure concepts theoretically and implement them practically using both manual and automated approaches.

The documentation is written in a beginner-friendly yet professional manner, following industry best practices and AWS Free Tier guidelines.

---

## Objectives
The main objectives of this task are:
- To understand AWS cloud core concepts
- To manually launch and manage an EC2 instance using the AWS Management Console
- To provision the same infrastructure using Terraform (Infrastructure as Code)
- To document the complete learning and implementation process
- To follow DevOps best practices such as automation, cost control, and version control

---

## Tools & Technologies Used
- Amazon Web Services (AWS Free Tier)
- Amazon EC2
- AWS CLI
- Terraform
- Git & GitHub
- Visual Studio Code
- Markdown documentation

---

## Repository Overview
This repository is organized as follows:

- `docs/aws.md` – Detailed theoretical explanation of AWS core concepts  
- `docs/terraform.md` – Terraform fundamentals and workflow explanation  
- `terraform_ec2/` – Terraform configuration files to provision EC2  
- `images/` – Screenshots of AWS Console and Terraform execution  

---

## AWS EC2 – Manual Implementation
The first part of this task involved launching an EC2 instance manually using the AWS Management Console. This helped in understanding the core components involved in EC2 provisioning, such as AMI selection, instance types, key pairs, security groups, and networking.

Screenshots of the manual EC2 launch process are available in the `images/` folder.

---

## EC2 Provisioning Using Terraform
The second part of the task focused on automating EC2 provisioning using Terraform. The same infrastructure was created using Infrastructure as Code principles, ensuring repeatability and consistency.

Terraform was configured to dynamically fetch the latest Amazon Linux AMI, avoiding region-specific AMI issues.

---

## Free Tier & Cost Management
All resources were created using AWS Free Tier eligible services. After verification, EC2 instances were terminated using `terraform destroy` to avoid unnecessary charges.

---

## Learning Outcome
Through this task, I gained a strong understanding of:
- AWS EC2 architecture
- IAM and AWS CLI configuration
- Infrastructure as Code using Terraform
- Automation vs manual provisioning
- DevOps best practices for cloud resource management

---

## Conclusion
This project provided practical exposure to real-world DevOps workflows. By combining theoretical knowledge with hands-on implementation, I developed confidence in managing and automating cloud infrastructure.

---
