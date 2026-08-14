# AWS Examples

## Example 1

### User

Deploy a FastAPI application.

Recommended Architecture

Internet

↓

Route53

↓

Application Load Balancer

↓

ECS Fargate

↓

RDS PostgreSQL

↓

ElastiCache

↓

CloudWatch

---

## Example 2

### User

Build an image upload service.

Recommended Services

Frontend

↓

API Gateway

↓

Lambda

↓

S3

↓

EventBridge

↓

SNS

---

## Example 3

### User

Deploy a LangGraph application.

Recommended Architecture

React

↓

API Gateway

↓

FastAPI

↓

LangGraph

↓

LLM

↓

Vector Database

↓

RDS

↓

CloudWatch

↓

Secrets Manager

---

## Example 4

### User

Deploy a static website.

Use:

S3

↓

CloudFront

↓

Route53

↓

ACM Certificate

---

## Example 5

### User

Deploy Docker containers.

Use:

GitHub Actions

↓

Build Docker Image

↓

Push to ECR

↓

Deploy ECS

↓

CloudWatch

---

## Example 6

### User

Implement CI/CD.

Workflow

Developer

↓

GitHub

↓

CodePipeline

↓

CodeBuild

↓

CodeDeploy

↓

Production

---

## Example 7

### User

Design secure VPC.

Architecture

Internet

↓

Internet Gateway

↓

Public Subnet

↓

Application Load Balancer

↓

Private Subnet

↓

Application Servers

↓

Private Database Subnet

↓

RDS

---

## Example 8

### User

Serverless workflow.

Client

↓

API Gateway

↓

Lambda

↓

DynamoDB

↓

EventBridge

↓

SNS

---

## Example 9

### User

Multi-region architecture.

Region A

↓

Route53 Failover

↓

Region B

↓

Cross-region Backup

↓

CloudFront

---

## Example 10

### User

Production AI Application.

Frontend

↓

CloudFront

↓

ALB

↓

FastAPI

↓

LangGraph

↓

OpenAI / Bedrock

↓

Aurora PostgreSQL

↓

S3

↓

CloudWatch

↓

Secrets Manager

↓

IAM Roles

↓

VPC