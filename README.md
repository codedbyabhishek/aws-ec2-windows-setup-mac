# AWS EC2 Windows Server Setup from MacBook Air (M1)

## Overview

This project documents the step-by-step process of launching and managing a Windows Server instance on AWS EC2 and accessing it from a MacBook Air M1 using Remote Desktop.

The goal was to gain hands-on experience with:

- EC2 instance provisioning
- Security group configuration
- Key pair authentication
- RDP connection from macOS
- Instance lifecycle management

---

## Architecture

MacBook Air (M1)
        ↓
Microsoft Remote Desktop (RDP)
        ↓
AWS EC2 Windows Server Instance

---

## 🚀 Setup Steps

### 1️⃣ Launch Windows EC2 Instance
- Selected Windows Server 2019 AMI
- Instance Type: t2.medium
- Configured storage (30GB+)

### 2️⃣ Configure Security Group
- Allowed RDP (TCP 3389) from my public IP
- Restricted unnecessary inbound traffic

### 3️⃣ Key Pair Authentication
- Generated .pem key pair
- Used AWS console to decrypt Administrator password

### 4️⃣ Connect from macOS
- Installed Microsoft Remote Desktop
- Connected using Public IPv4 address
- Logged in with Administrator credentials

### 5️⃣ Manage Instance Lifecycle
- Tested start, stop, and reboot functionality
- Monitored EC2 status checks

---

## Key Learnings

- Practical AWS EC2 provisioning
- Cloud networking fundamentals
- Secure remote server access
- Windows server management in cloud
- Infrastructure lifecycle control

---

## 📌 Future Improvements

- Automate setup using Terraform
- Add CloudFormation template
- Configure IAM roles
- Explore VPC customization

