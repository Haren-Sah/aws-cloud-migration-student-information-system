# Cost Analysis

## Cost Management Objectives

The architecture balances performance, availability, and security while maintaining cost efficiency.

The design leverages managed AWS services to reduce operational overhead and infrastructure maintenance costs.

---

# Primary Cost Components

## Compute

### Amazon EC2

Used for:

- Student portal application servers

Cost drivers:

- Instance size
- Runtime hours
- Auto Scaling activity

Optimization:

- Auto Scaling Groups
- Right-sized instances

---

## Database

### Amazon RDS MySQL

Used for:

- Student Information System database

Cost drivers:

- Instance type
- Storage allocation
- Multi-AZ deployment

Optimization:

- Reserved Instances
- Storage monitoring

---

## Storage

### Amazon S3

Used for:

- Student documents
- Historical archives
- CloudTrail logs

Optimization:

- Lifecycle policies
- Intelligent Tiering
- Glacier archival

---

## Serverless Processing

### AWS Lambda

Used for:

- Enrollment data processing

Benefits:

- Pay only for execution time
- No server management

---

## Monitoring & Governance

Services:

- CloudWatch
- CloudTrail
- AWS Backup

Benefits:

- Operational visibility
- Compliance support

---

# Business Benefits

## Improved Availability

- Multi-AZ deployment
- Automated failover

Result:

Reduced downtime risk.

---

## Reduced Infrastructure Management

AWS-managed services reduce:

- Hardware maintenance
- OS patching effort
- Backup administration

---

## Scalability

The environment automatically adapts to:

- Enrollment periods
- Increased user demand
- Seasonal workload spikes

---

## Security Improvements

Benefits include:

- Centralized access control
- Encryption
- Audit logging

---

# Cost Optimization Strategy

The project incorporates:

- Auto Scaling Groups
- S3 Lifecycle Policies
- Glacier Storage
- Serverless Processing
- Resource shutdown during development
- Infrastructure as Code for repeatable deployment

---

# Conclusion

Although cloud adoption introduces operational expenditure, the benefits gained through scalability, resilience, security, and reduced infrastructure maintenance outweigh the costs. The proposed architecture provides a cost-effective foundation for Horizon College's digital transformation initiative.
