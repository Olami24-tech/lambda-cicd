# AWS CI/CD Pipeline with GitHub Actions & CloudFormation

## Overview

This project demonstrates how to automate AWS infrastructure deployment using GitHub Actions and AWS CloudFormation.

It validates CloudFormation templates during Pull Requests and deploys infrastructure automatically after code changes are merged.

---

## Architecture

![Architecture] <img width="856" height="155" alt="Github Workflow Architectural Diagram" src="https://github.com/user-attachments/assets/cf380e25-9323-475d-97a6-45044053cc70" />

---
## Screenshots

### Successful Pull Request Validation

<img width="1882" height="802" alt="Screenshot merge" src="https://github.com/user-attachments/assets/f79c5f6c-c30e-4161-832c-16aa21f8c880" />


### Successful GitHub Actions Deployment

(Insert screenshot)

### CloudFormation Stack

<img width="1890" height="317" alt="Screenshot cloudformation" src="https://github.com/user-attachments/assets/732d63ce-2c75-453a-b100-10659e7a7aa1" />


### Amazon S3 Bucket

<img width="1012" height="397" alt="Screenshot workflow" src="https://github.com/user-attachments/assets/44c0b4f0-c48e-431b-be91-f35604d1d492" />


lambda-cicd/

├── .github/
│   └── workflows/
│       ├── lambda-deploy.yml
│       └── cfn-validate-pr.yml
│
├── cloudformation/
│   └── s3-bucket.yml
│
├── lambda/
│   ├── lambda_function.py
│   └── requirements.txt
│
└── README.md

## Features
- Automated AWS Lambda deployment
- CloudFormation template validation
- Pull Request automation
- AWS credential management using GitHub Secrets
- Infrastructure as Code (IaC)
- CI/CD using GitHub Actions

---

## Technologies Used

- AWS CloudFormation
- Amazon S3
- GitHub Actions
- Git
- YAML
- AWS CLI

---
## Skills Demonstrated

- Git
- GitHub
- GitHub Actions
- AWS CloudFormation
- AWS Lambda
- Amazon S3
- Infrastructure as Code
- YAML
- AWS CLI
- CI/CD Pipelines

## Workflow

1. Developer creates a feature branch.
2. Opens a Pull Request.
3. GitHub Actions validates the CloudFormation template.
4. CloudFormation deploys a test stack.
5. After merge, infrastructure is deployed automatically.

---

## Lessons Learned

- Building GitHub Actions workflows
- CloudFormation validation
- Infrastructure as Code
- YAML troubleshooting
- AWS deployment automation
- CI/CD best practices

---
## Challenges Faced

During development I encountered several issues including:

- GitHub Actions YAML syntax errors
- CloudFormation template validation failures
- AWS credential configuration
- Git workflow and repository structure issues
- CloudFormation resource property errors

Resolving these issues helped me gain a much better understanding of GitHub Actions, Infrastructure as Code and AWS deployment workflows.

## Future Improvements

- Add automated stack cleanup
- Multi-environment deployments
- Manual approvals
- Security scanning
