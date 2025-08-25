# EC2 Image Builder Components

A collection of reusable AWS EC2 Image Builder components for automating software installation and configuration on EC2 instances.

## Overview

AWS EC2 Image Builder is a fully managed AWS service that makes it easier to automate the creation, management, and deployment of customized, secure, and up-to-date server images. This repository contains custom components that extend Image Builder's capabilities for specific software installations and configurations.

## Components

### 1. Visual Studio Code (`install-vscode.yml`)

Installs Visual Studio Code on Windows instances for development environments.

**Features:**

- Silent installation with pre-configured options
- Adds VS Code to PATH
- Context menu integration
- File association setup
- Post-installation validation

## Prerequisites

- AWS Account with EC2 Image Builder access
- IAM permissions for:
  - EC2 Image Builder operations
  - S3 access (for components using S3)
  - EC2 instance management
- Target EC2 instances must have:
  - SSM Agent installed and running
  - Appropriate IAM instance profile
  - Internet connectivity or VPC endpoints for AWS services
