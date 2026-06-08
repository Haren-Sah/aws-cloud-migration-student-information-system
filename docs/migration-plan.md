# Migration Strategy

## Project Overview

Horizon College currently relies on disconnected enrolment systems, paper-based archives, and on-premises file servers. This project proposes a phased migration to AWS to improve accessibility, scalability, security, and operational efficiency.

The target architecture adopts a cloud-native design using Amazon EC2, Amazon RDS, Amazon S3, AWS Lambda, and supporting AWS security and governance services.

---

# Migration Objectives

The migration seeks to achieve the following outcomes:

- Centralize student, staff, and parent services.
- Improve availability and fault tolerance.
- Reduce dependence on on-premises infrastructure.
- Enable secure remote access.
- Improve data protection and disaster recovery.
- Establish a scalable foundation for future digital services.

---

# Migration Approach

A phased migration approach minimizes operational risk while allowing validation at each stage.

## Phase 1 – Assessment & Discovery

Activities:

- Review existing applications and workloads.
- Identify data sources and dependencies.
- Assess network requirements.
- Define security and compliance requirements.
- Establish migration success criteria.

Deliverables:

- Application inventory
- Dependency mapping
- Migration readiness assessment

---

## Phase 2 – AWS Foundation Setup

Activities:

- Create AWS account structure.
- Configure IAM roles and policies.
- Deploy VPC architecture.
- Create public and private subnets.
- Configure security groups and routing.

Deliverables:

- Secure AWS landing zone
- Network architecture deployment
- Governance baseline

---

## Phase 3 – Infrastructure Deployment

Activities:

- Deploy Application Load Balancer.
- Create EC2 Auto Scaling Groups.
- Deploy Amazon RDS Multi-AZ database.
- Configure S3 storage buckets.
- Configure monitoring and logging.

Deliverables:

- Operational cloud infrastructure
- High availability environment

---

## Phase 4 – Data Migration

Activities:

- Migrate student records.
- Transfer historical archives to Amazon S3.
- Configure lifecycle policies.
- Validate data integrity.

Deliverables:

- Cloud-hosted datasets
- Archive migration completion

---

## Phase 5 – Application Migration

Activities:

- Deploy student portal application.
- Configure database connectivity.
- Implement Lambda-based automation.
- Test application functionality.

Deliverables:

- Functional cloud-based SIS
- Integrated enrollment workflow

---

## Phase 6 – Validation & Go-Live

Activities:

- End-to-end testing.
- Security verification.
- Performance testing.
- User acceptance testing.

Deliverables:

- Production-ready environment
- Operational handover

---

# Success Criteria

The migration will be considered successful when:

- All critical systems operate in AWS.
- Data integrity is maintained.
- Availability targets are achieved.
- Security controls are validated.
- Staff and students can access services remotely.

---

# Future Enhancements

Potential future improvements include:

- Infrastructure as Code (Terraform/CloudFormation)
- CI/CD pipelines
- AWS WAF integration
- VPN or Direct Connect connectivity
- Advanced monitoring and anomaly detection
