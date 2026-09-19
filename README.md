# ☁️ AWS EC2 Monitoring, EBS Storage & CloudWatch Project

## 📌 Project Overview

This project demonstrates the practical implementation of AWS cloud infrastructure using **Amazon EC2, Amazon EBS, and Amazon CloudWatch**, along with **Linux, SSH, Git, and GitHub**.

The project was developed to gain hands-on experience in cloud infrastructure management, Linux system administration, storage management, performance monitoring, and basic DevOps practices.

In this project, an **Amazon EC2 Linux instance** was launched and configured as the main compute resource. An additional **Amazon EBS volume** was created and attached to the EC2 instance to provide persistent block storage. The EBS volume was identified, formatted, mounted, and used for storing and managing files.

**Amazon CloudWatch** was used to monitor the EC2 instance and observe its **CPU Utilization** metric. This provided practical experience in monitoring AWS resources and understanding server performance.

**Git and GitHub** were used for version control, project documentation, and maintaining the project repository.

Overall, this project combines **AWS Cloud, EC2, EBS, CloudWatch, Linux, SSH, Git, and GitHub** into one practical cloud infrastructure implementation.

---

## 🎯 Project Objectives

The main objectives of this project are:

- To understand AWS cloud infrastructure
- To launch and manage an Amazon EC2 Linux instance
- To connect to EC2 using SSH
- To perform Linux administration tasks
- To create and attach an EBS volume
- To format and mount EBS storage
- To create and manage files on mounted storage
- To monitor EC2 performance using CloudWatch
- To monitor CPU Utilization
- To understand basic cloud monitoring
- To use Git for version control
- To maintain the project using GitHub
- To gain practical exposure to basic DevOps practices

---

# 🏗️ AWS Architecture

```text
                         AWS CLOUD
                             │
                             ▼
                    ┌─────────────────┐
                    │   Amazon EC2    │
                    │   Linux Server  │
                    └────────┬────────┘
                             │
              ┌──────────────┴──────────────┐
              │                             │
              ▼                             ▼
     ┌─────────────────┐          ┌─────────────────────┐
     │    Amazon EBS   │          │   Amazon CloudWatch │
     │ Persistent      │          │     Monitoring      │
     │ Block Storage   │          └──────────┬──────────┘
     └────────┬────────┘                     │
              │                              ▼
              ▼                     ┌─────────────────────┐
     ┌─────────────────┐             │  CPU Utilization   │
     │ Format / Mount  │             │      Metrics       │
     │     /index      │             └─────────────────────┘
     └────────┬────────┘
              │
              ▼
     ┌─────────────────┐
     │ Files / Data    │
     │   test.txt      │
     └─────────────────┘


                  VERSION CONTROL
                         │
                         ▼
                    ┌─────────┐
                    │   Git   │
                    └────┬────┘
                         │
                         ▼
                    ┌─────────┐
                    │ GitHub  │
                    └─────────┘
                    START
                      │
                      ▼
             Launch EC2 Instance
                      │
                      ▼
              Connect using SSH
                      │
                      ▼
           Linux Administration
                      │
                      ▼
             Create EBS Volume
                      │
                      ▼
            Attach EBS to EC2
                      │
                      ▼
          Identify Storage Device
                      │
                      ▼
            Format EBS Volume
                      │
                      ▼
            Create Mount Point
                      │
                      ▼
             Mount EBS Volume
                      │
                      ▼
           Store / Manage Files
                      │
                      ▼
          Configure CloudWatch
                      │
                      ▼
        Monitor CPU Utilization
                      │
                      ▼
             Git Version Control
                      │
                      ▼
             Push to GitHub
                      │
                      ▼
                     END


#EBS Implementation

Create EBS Volume
       │
       ▼
Attach Volume to EC2
       │
       ▼
Identify Device
       │
       ▼
Format Volume
       │
       ▼
Create Mount Point
       │
       ▼
Mount Volume
       │
       ▼
Create / Store Files
       │
       ▼
Verify Storage
