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

## Repository Structure

aws-ec2-terraform-devops/
├── README.md
├── docs/
│ ├── aws.md
│ └── terraform.md
├── terraform_ec2/
│ ├── provider.tf
│ ├── main.tf
│ ├── variables.tf
│ └── outputs.tf
├── images/
└── .gitignore



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

## Manual EC2 Launch Using AWS Console

### Steps Followed
1. Logged into AWS Management Console
2. Navigated to EC2 Dashboard
3. Selected Amazon Linux 2 AMI
4. Chose `t3.micro` instance type (Free Tier eligible)
5. Created and selected an EC2 Key Pair
6. Configured security group
7. Launched the instance

### EC2 Running State
After launch, the EC2 instance entered the running state.
---

### EC2 Termination
After verification, the instance was terminated to avoid unnecessary billing.

## EC2 Provisioning Using Terraform (Infrastructure as Code)

Terraform was used to automate EC2 provisioning. This approach ensures repeatability, consistency, and reduced human error.

### Terraform Files Used
- `provider.tf` – AWS provider configuration
- `variables.tf` – Input variables
- `main.tf` – EC2 resource definition
- `outputs.tf` – Output values

---

### Terraform Initialization
Terraform was initialized to download required providers.

### Terraform Apply
The EC2 instance was created using Terraform with dynamic AMI selection.

### Terraform Destroy
After validation, the infrastructure was destroyed to ensure cost control.

## Key Learnings
- Manual provisioning helps understand AWS fundamentals
- Terraform enables automation and repeatability
- AMI IDs are region-specific and should be dynamically fetched
- Infrastructure as Code is essential for modern DevOps workflows
- Resource cleanup is critical when using AWS Free Tier

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
