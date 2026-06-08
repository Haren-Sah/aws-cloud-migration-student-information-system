# Security Design

## Security Objectives

The architecture is designed according to AWS Well-Architected Framework security principles:

- Least privilege access
- Defense in depth
- Encryption by default
- Continuous monitoring
- Secure network segmentation

---

# Network Security

## VPC Segmentation

The environment is divided into three logical layers:

### Public Subnets

Contains:

- Application Load Balancer

Responsibilities:

- Accept HTTPS traffic
- Route requests to application servers

---

### Private Application Subnets

Contains:

- EC2 Auto Scaling Group
- AWS Lambda functions

Characteristics:

- No direct internet access
- Outbound access through NAT Gateway

---

### Private Database Subnets

Contains:

- Amazon RDS MySQL

Characteristics:

- No public access
- Access restricted to application layer

---

# Identity & Access Management

IAM controls access to AWS resources.

Key principles:

- Least privilege permissions
- Role-based access control
- No hardcoded credentials

Examples:

- EC2 Instance Roles
- Lambda Execution Roles
- Administrative IAM Groups

---

# Data Protection

## Encryption at Rest

Protected services:

- Amazon RDS
- Amazon S3
- AWS Backup

Encryption service:

- AWS Key Management Service (KMS)

---

## Encryption in Transit

Traffic is encrypted using:

- HTTPS (TLS)(Not Implemented in Project)
- Secure database connections

---

# Monitoring & Auditing

## Amazon CloudWatch

Used for:

- Performance monitoring
- Application logging
- Operational alerting

---

## AWS CloudTrail

Provides:

- API activity logging
- Compliance evidence
- Security investigations

CloudTrail logs are stored in a dedicated S3 bucket.

---

# Backup & Recovery

AWS Backup provides:

- Automated backup scheduling
- Retention management
- Recovery point objectives

Amazon RDS Multi-AZ supports:

- Automated failover
- High availability

---

# Risk Mitigation

| Threat                 | Mitigation                   |
| ---------------------- | ---------------------------- |
| Unauthorized access    | IAM least privilege          |
| Data breach            | Encryption using KMS         |
| Infrastructure failure | Multi-AZ deployment          |
| Data loss              | AWS Backup                   |
| Misconfiguration       | Security reviews and testing |

---

# Security Outcomes

The proposed design delivers:

- Strong network isolation
- Secure identity management
- End-to-end encryption(Not Implemented)
- Continuous monitoring
- High availability and resilience
