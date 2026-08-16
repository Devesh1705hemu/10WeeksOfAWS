# 🌍 AWS Global Infrastructure & Security Basics

## ❓ Questions

### 1. What is a Region?

An **AWS Region** is a geographic area where AWS has multiple isolated data centers called **Availability Zones**.

**Example:** `ap-south-1` is the Mumbai Region.

**Key Point:** Choose a Region based on latency, compliance, service availability, and cost.

---

### 2. What is an Availability Zone?

An **Availability Zone (AZ)** is an isolated data center location within an AWS Region.

A Region contains multiple Availability Zones, which are designed to be independent from failures in other AZs.

**Exam Pointer:**  
Use multiple Availability Zones to improve **high availability** and fault tolerance.

---

### 3. What is one thing AWS secures?

AWS secures the **infrastructure of the cloud**.

Examples:

- Physical data centers
- Physical hardware
- AWS networking infrastructure
- Underlying infrastructure used by AWS managed services

This is called **Security of the Cloud**.

---

### 4. What is one thing you must secure?

You are responsible for securing the resources and applications that **you deploy in AWS**.

Examples:

- IAM users, roles, and permissions
- Your data
- Applications
- Security Groups
- Network configuration
- EC2 guest operating system
- EC2 OS patching

This is called **Security in the Cloud**.

---
# AWS Global Infrastructure
## AWS infrastructure is built using:
Region: a geographic area where AWS has multiple data centers.
Availability Zone: an isolated data center location inside a Region.
Edge Location: a location used by services like CloudFront to serve users faster.
### Exam pointer:
-Use multiple Availability Zones for high availability.
-Use CloudFront and Edge Locations for low-latency content delivery.
# Shared Responsibility Model
-AWS security is shared between AWS and the customer.
-AWS is responsible for security of the cloud.
-You are responsible for security in the cloud.
#### Examples:
AWS manages data centers, hardware, networking, and managed service infrastructure.
You manage IAM, permissions, data, applications, network rules, and EC2 guest OS patching.
#### Simple line:
AWS secures the cloud. You secure what you build in the cloud.

# Root User
The root user owns the AWS account and has full access to everything.
## Best practices:
-Enable MFA on root user.
-Do not use root user for daily work.
-Create IAM users or roles for regular tasks.
-Monitor billing from the beginning.
Use the root user only for account-level setup like MFA and billing. After that, avoid using it for daily practice.
