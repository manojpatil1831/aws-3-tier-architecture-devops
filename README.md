# aws-3-tier-architecture-devops
Production-ready AWS 3-tier architecture with ALB, EC2, RDS, and VPC


# AWS 3-Tier Architecture – DevOps Project

## 📌 Project Overview
This project demonstrates a production-ready AWS 3-tier architecture using best practices for
security, scalability, and high availability.

## 🧱 Architecture
- VPC with public & private subnets
- External & Internal Application Load Balancers
- Web & App EC2 instances
- RDS (Multi-AZ) in private subnet
- NAT Gateway for outbound access

## 🔁 Traffic Flow
Internet → External ALB → Web Tier → Internal ALB → App Tier → RDS

## ⚙️ Execution Steps
1. VPC & subnet design
2. Security Groups & NACLs
3. EC2 deployment
4. ALB & Target Groups
5. RDS configuration
6. Auto Scaling
7. End-to-end testing

## 🐞 Issues Faced
- Target groups showing unhealthy
- Apache not responding due to NAT misconfiguration

## 🔧 Fixes Applied
- Corrected health check path
- Enabled outbound access via NAT Gateway
- Verified security group rules

## 📚 Key Learnings
- Importance of subnet design
- ALB health depends on networking & app readiness
- NAT is mandatory for private subnet instances
- Security must be validated

## 🔜 Future Improvements
- CI/CD pipeline
- Monitoring & alerts
- Infrastructure as Code (Terraform)

## 🙌 Author
Manoj Patil  
DevOps / Cloud Engineer (Fresher)
