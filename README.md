# Terraform AWS S3 Bucket Provisioning

This project demonstrates provisioning AWS infrastructure using **Terraform**.  
The goal is to manage cloud resources through **Infrastructure as Code (IaC)** rather than manual configuration in the AWS console.

Terraform is used to define the desired infrastructure state and automate the creation and configuration of an Amazon S3 bucket.

---
<img width="2538" height="576" alt="image" src="https://github.com/user-attachments/assets/a99b1e03-abeb-4442-a2b3-b3988c950f8f" />

## Technologies

- Terraform
- AWS S3
- AWS CLI
- Infrastructure as Code (IaC)

---

## Project Overview

The Terraform configuration provisions:

- An **Amazon S3 bucket**
- **Public access restrictions** for security
- An **S3 object upload** (image)

All resources are defined in the Terraform configuration file `main.tf`.

---

## Terraform Workflow

The infrastructure is deployed using the standard Terraform lifecycle:

` bash
terraform init
terraform plan
terraform apply

init – initializes Terraform and installs provider plugins

plan – reviews the infrastructure changes Terraform will make

apply – provisions the infrastructure in AWS

Security

Public access to the S3 bucket is restricted using Terraform configuration.

Terraform-generated files such as state files and provider directories are excluded from version control using .gitignore.

Key Concepts Demonstrated

Infrastructure as Code

Terraform AWS provider configuration

Automated cloud resource provisioning

Secure S3 configuration

Terraform workflow and state management

Future Improvements

Potential enhancements include:

Terraform modules

Remote state storage (S3 + DynamoDB)

CI/CD automation with GitHub Actions

Expanded infrastructure provisioning

Author

Micah Okemeje
