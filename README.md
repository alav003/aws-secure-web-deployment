# Secure AWS EC2 Deployment with Custom Networking & Monitoring

## Project Overview
This project demonstrates manual deployment of cloud infrastructure using AWS.  
A custom VPC, public subnet, EC2 instance, security group configuration, IAM role attachment, and CloudWatch monitoring were configured without automation tools.

## Architecture Components
- Custom VPC (10.0.0.0/16)
- Public Subnet (10.0.1.0/24)
- Internet Gateway and route table configuration
- EC2 instance (t3.micro, Amazon Linux 2)
- Security Group (SSH restricted to my IP, HTTP open to public)
- IAM role attached to EC2 instance
- CloudWatch CPU utilization alarm (>70%)

## Security Configuration
- SSH access restricted to personal IP only
- No public database or additional open ports
- IAM role used instead of embedded credentials

## Monitoring
- CloudWatch alarm configured to trigger when CPU utilization exceeds 70% for 5 minutes.

## Live Server
The deployed server hosts a basic Nginx page confirming successful infrastructure setup.

---

This project highlights foundational cloud networking, compute provisioning, access control, and monitoring practices.

