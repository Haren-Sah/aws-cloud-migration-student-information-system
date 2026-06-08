# AWS Cloud Migration – Student Information System Architecture

## Overview

This project presents a scalable, secure, and highly available AWS-based cloud migration architecture for a Student Information System (SIS) for a K–12 educational institution.

The existing system suffers from:

- Disconnected enrolment and academic systems
- Paper-based archival processes
- On-premise file storage limitations
- Lack of centralized access control for staff, students, and parents

This solution modernizes the infrastructure using AWS cloud-native services, focusing on scalability, security, and operational efficiency.

---

## Architecture Summary

The system is designed as a **multi-tier cloud-native architecture** deployed inside a secure Amazon VPC:

- Public Web Tier (Application Load Balancer)
- Private Application Tier (EC2 Auto Scaling Group)
- Private Data Tier (Amazon RDS Multi-AZ)
- Serverless Processing Layer (AWS Lambda + S3 events)
- Object Storage Layer (Amazon S3 with lifecycle policies)

---

## High-Level Architecture
