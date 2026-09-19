# AWS EC2 Monitoring Project

## 📌 Project Overview

This project demonstrates the practical implementation of AWS cloud infrastructure using Amazon EC2, Amazon EBS, and Amazon CloudWatch.

The project focuses on launching and managing an EC2 instance, attaching and configuring EBS storage, monitoring instance performance using CloudWatch, and managing the project using Git and GitHub.

---

## 🏗️ AWS Architecture

EC2 Instance
      |
      └── EBS Volume
      |
      └── CloudWatch
            |
            └── CPU Utilization Monitoring

Git → GitHub

---

## ☁️ AWS Services Used

| Service | Purpose |
|---|---|
| Amazon EC2 | Compute server / virtual machine |
| Amazon EBS | Persistent block storage |
| Amazon CloudWatch | Monitoring and performance metrics |
| Git | Version control |
| GitHub | Source code and project documentation |

---

## 💻 Amazon EC2

An Amazon EC2 Linux instance was launched and configured as the main compute resource.

### Tasks Performed

- Launched an EC2 instance
- Connected to the instance using SSH
- Performed Linux command-line operations
- Checked system and storage information
- Managed the EC2 environment

---

## 💾 Amazon EBS

An additional EBS volume was attached to the EC2 instance for persistent storage.

### Tasks Performed

- Created an EBS volume
- Attached the volume to EC2
- Formatted the volume
- Created a mount point
- Mounted the EBS volume
- Created and managed files on the mounted storage
- Verified disk usage using Linux commands

Example:

```bash
df -h
