# Infrastructure as Code (IaC) Repository

This repository contains Terraform configurations for provisioning various AWS resources. It includes definitions for IAM roles, policies, instance profiles, VPC settings, and more. The infrastructure is designed to support a secure and scalable cloud environment.

## Table of Contents

- [Overview](#overview)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
- [Resources Provisioned](#resources-provisioned)
- [Scripts](#scripts)
- [Contributing](#contributing)

## Overview

The IaC configurations in this repository aim to automate the creation and management of AWS resources such as IAM roles and policies, instance profiles, and VPC configurations. This approach ensures consistency, repeatability, and version control over the infrastructure.

## Requirements

- Terraform >= 0.12
- An AWS account with sufficient permissions to manage the required resources

## Getting Started

1. Clone the repository:

2. Initialize Terraform:

3. Review the configuration files (`*.tf`) to understand what resources will be provisioned.

4. Apply the Terraform configuration:


## Resources Provisioned

- **IAM Roles and Policies**: Defined in `iam-role.tf` and `iam-policy.tf`, these resources set up the necessary permissions for your AWS services.
- **Instance Profiles**: Configured in `iam-instance-profile.tf`, these profiles allow EC2 instances to assume the defined IAM roles.
- **VPC Configuration**: Managed in `vpc.tf`, this includes setting up the VPC, subnets, and other networking components.
- **Outputs**: Detailed in `outputs.tf`, this file defines outputs that can be accessed post-deployment, such as public IP addresses, DNS names, etc.

## Scripts

- **install-tools.sh**: A script to install necessary tools for managing the infrastructure. Run `./install-tools.sh` to execute the script.
