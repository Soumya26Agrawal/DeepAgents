# AWS Development Instructions

## General Workflow

Whenever solving an AWS problem:

1. Understand business requirements.
2. Identify functional requirements.
3. Identify non-functional requirements.
4. Select appropriate AWS services.
5. Design secure networking.
6. Configure IAM.
7. Plan deployment.
8. Enable monitoring.
9. Optimize costs.
10. Explain architectural decisions.

---

# Service Selection

Always prefer managed services whenever possible.

Example:

Use Lambda before EC2 when appropriate.

Use Aurora instead of self-managed MySQL when managed databases are acceptable.

---

# Identity and Access Management

Follow least privilege.

Use:

- IAM Roles
- IAM Policies
- IAM Groups

Avoid:

- Root account usage
- Long-lived access keys
- AdministratorAccess unless necessary

---

# Networking

Design VPC carefully.

Separate:

- Public subnets
- Private subnets

Use:

- Security Groups
- Network ACLs
- Route Tables

Never expose internal services directly to the internet.

---

# Compute

Choose compute based on workload.

Use:

Lambda

for event-driven applications.

Use:

ECS/Fargate

for containerized workloads.

Use:

EC2

only when infrastructure control is required.

---

# Storage

Choose storage appropriately.

Object Storage

→ S3

Block Storage

→ EBS

Shared File System

→ EFS

Archive

→ Glacier

---

# Databases

Relational

→ Aurora / RDS

NoSQL

→ DynamoDB

Cache

→ ElastiCache

Search

→ OpenSearch

---

# Monitoring

Enable:

CloudWatch Metrics

CloudWatch Logs

CloudWatch Alarms

CloudTrail

X-Ray (when applicable)

---

# Infrastructure as Code

Prefer:

CloudFormation

or

AWS CDK

Avoid manual console configuration.

---

# CI/CD

Recommend:

CodePipeline

CodeBuild

CodeDeploy

GitHub Actions

depending on project requirements.

---

# Security

Use:

Secrets Manager

Parameter Store

KMS

Never hardcode credentials.

---

# High Availability

Deploy across multiple Availability Zones.

Use Auto Scaling whenever possible.

---

# Cost Optimization

Prefer:

Managed services

Auto Scaling

Spot Instances

Lifecycle policies

Storage tiering

Right-sized resources

---

# Documentation

Always explain:

Why each AWS service was selected.

Possible alternatives.

Trade-offs.

Estimated operational complexity.