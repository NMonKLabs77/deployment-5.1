m
# Deployment 5.1 Retail Banking Application 

## Overview

1. [Prerequisites](#prerequisites)
2. [Creating AWS Key Pair](#creating-aws-key-pair)
3. [Recreating VPC with Terraform](#recreating-vpc-with-terraform)
4. [Infrastructure Components](#infrastructure-components)
5. [Jenkins Configuration](#jenkins-configuration)
6. [Application Deployment](#application-deployment)
7. [Improvisation](#improvisation)
8. [Purpose of a Jenkins Agent](#purpose-of-a-jenkins-agent)
9. [Diagram](#diagram)

## Prerequisites

Before you start, ensure you have the following prerequisites in place:

1. AWS Account
2. AWS CLI Installed and Configured
3. Terraform Installed

## Creating AWS Key Pair

When you create new EC2 instances, follow these steps to create a new AWS Key Pair and save the .pem file on your local computer. Ensure that you attach the private key to all your instances.

## Recreating VPC with Terraform

To recreate the VPC and associated resources, follow these steps:

1. Clone this repository to your local machine.

2. Navigate to the project directory in your terminal.

3. Update the `variables.tf` file with your AWS credentials, region, and any other required variables.

4. Run the following commands to create the infrastructure:

   ```
   terraform init
   terraform apply
   ```

5. Confirm the changes when prompted by Terraform.

## Infrastructure Components

The infrastructure includes the following components:

- **1 VPC**

- **2 availability zones**
- **2 Public Subnets**
- **3 EC2s**
- **1 Route Table**
- **Security Group Ports: 8080, 8000, 22**

## Jenkins configuration
[Lik to jenkins setup](/requirements/jenkins.sh)

##Application Deployment


## Improvisation


## Purpose of a Jenkins Agent


## Diagram
