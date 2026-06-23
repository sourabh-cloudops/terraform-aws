# Terraform AWS Lab

## Overview

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision AWS resources.

The objective of this lab is to automate AWS infrastructure creation and eliminate manual provisioning activities.

## Architecture

Terraform
↓
AWS Provider
↓
EC2 Instance
↓
Infrastructure Ready

## Technologies Used

* Terraform
* AWS EC2
* AWS IAM
* AWS VPC
* Amazon Linux
* GitHub

## Project Structure

terraform-aws-lab/

├── provider.tf

├── variables.tf

├── main.tf

├── outputs.tf

├── terraform.tfvars

└── README.md

## Prerequisites

1. AWS Account
2. AWS CLI Installed
3. Terraform Installed
4. IAM User with EC2 permissions

## Configure AWS Credentials

**aws configure**

Provide:

* Access Key
* Secret Key
* Region
* Output Format

## Verify Configuration

aws sts get-caller-identity

## Initialize Terraform

**terraform init**

Purpose:

* Downloads AWS provider plugins
* Initializes Terraform working directory

## Validate Configuration

**terraform validate**

Purpose:

* Validates Terraform syntax
* Checks configuration correctness

## Review Execution Plan

**terraform plan**

Purpose:

* Displays resources that Terraform will create
* Helps prevent accidental changes

## Deploy Infrastructure

**terraform apply**

Type:

yes

Terraform creates:

* EC2 Instance

## Verify Resources

AWS Console

EC2 Dashboard

Verify:

* Instance Running
* Public IP Assigned

## View Outputs

terraform output

Example:

instance_id

public_ip

## Destroy Infrastructure

terraform destroy

Purpose:

* Removes all resources created by Terraform
* Avoids unnecessary AWS charges

## Key Benefits

### Infrastructure as Code

Infrastructure can be created using code instead of manual AWS console activities.

### Repeatability

Same infrastructure can be deployed multiple times with consistent configuration.

### Version Control

Terraform files can be stored in GitHub and tracked through Git commits.

### Automation

Reduces manual effort and provisioning time.

### Consistency

Eliminates configuration drift across environments.

### Scalability

Supports creation of multiple environments such as DEV, UAT, TEST, and PROD.

## Learning Outcomes

* Terraform Basics
* Providers
* Variables
* Outputs
* EC2 Provisioning
* Infrastructure Automation
* AWS Resource Management
* Infrastructure as Code (IaC)

## Author

Sourabh Bhosale

AWS Certified Solutions Architect Associate

DevOps Engineer
