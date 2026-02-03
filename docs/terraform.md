# Terraform Fundamentals – Infrastructure as Code

## Introduction
Terraform is an open-source Infrastructure as Code (IaC) tool developed by HashiCorp. It allows infrastructure to be defined, managed, and version-controlled using code.

This document explains Terraform concepts from a beginner DevOps perspective.

---

## What is Infrastructure as Code (IaC)?
Infrastructure as Code is the practice of managing infrastructure using configuration files instead of manual processes.

Benefits:
- Automation
- Repeatability
- Version control
- Reduced human error

---

## Why Terraform?
Terraform is widely used because:
- It is cloud-agnostic
- Uses declarative syntax
- Supports multiple providers
- Is easy to learn and maintain

---

## Terraform Architecture
Terraform works with:
- **Providers**: Cloud platforms such as AWS
- **Resources**: Infrastructure components like EC2
- **State file**: Tracks current infrastructure

---

## Terraform Workflow
1. `terraform init` – Initializes the project and downloads providers
2. `terraform plan` – Shows execution plan without creating resources
3. `terraform apply` – Creates or updates infrastructure
4. `terraform destroy` – Deletes infrastructure to avoid cost

---

## Terraform Configuration Files
- `provider.tf`: Provider configuration
- `main.tf`: Resource definitions
- `variables.tf`: Input variables
- `outputs.tf`: Output values

---

## Dynamic AMI Selection
AMI IDs are region-specific. Terraform data sources can dynamically fetch the latest AMI, making configurations portable across regions.

This is a best practice in real-world DevOps projects.

---

## Best Practices Followed
- IAM user instead of root
- AWS Free Tier usage
- Dynamic AMI lookup
- Resource cleanup using destroy
- Clean folder structure

---

## Summary
Terraform enables DevOps engineers to manage cloud infrastructure efficiently and safely using automation. It plays a key role in modern DevOps workflows.
