# ☁️ AWS EC2 Monitoring, EBS Storage & CloudWatch Project

## 📌 Project Overview

This project demonstrates the practical implementation of AWS cloud infrastructure using Amazon EC2, Amazon EBS, and Amazon CloudWatch, along with Linux, SSH, Git, and GitHub.

The project was developed to gain hands-on experience in cloud infrastructure management, Linux system administration, storage management, performance monitoring, and basic DevOps practices.

In this project, an Amazon EC2 Linux instance was launched and configured as the main compute resource. An additional Amazon EBS volume was created and attached to the EC2 instance to provide persistent block storage.

The EBS volume was identified, formatted, mounted, and used for storing and managing files.

Amazon CloudWatch was used to monitor the EC2 instance and observe CPU Utilization metrics.

Git and GitHub were used for version control, project documentation, and maintaining the project repository.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Understand AWS cloud infrastructure
- Launch and manage an Amazon EC2 Linux instance
- Connect to EC2 using SSH
- Perform Linux administration tasks
- Create and attach an EBS volume
- Format and mount EBS storage
- Create and manage files on mounted storage
- Monitor EC2 performance using CloudWatch
- Monitor CPU Utilization
- Understand basic cloud monitoring
- Use Git for version control
- Maintain the project using GitHub
- Gain practical exposure to basic DevOps practices

---

## 🏗️ AWS Architecture

```text
                         AWS CLOUD
                             |
                             v
                    +-----------------+
                    |   Amazon EC2    |
                    |   Linux Server  |
                    +--------+--------+
                             |
                +------------+------------+
                |                         |
                v                         v
       +-----------------+       +---------------------+
       |    Amazon EBS   |       |   Amazon CloudWatch |
       | Persistent      |       |     Monitoring      |
       | Block Storage   |       +----------+----------+
       +--------+--------+                  |
                |                           v
                v                  +---------------------+
       +-----------------+         |  CPU Utilization   |
       | Format & Mount  |         |      Metrics       |
       |     /index      |         +---------------------+
       +--------+--------+
                |
                v
       +-----------------+
       | Files / Data    |
       |   test.txt      |
       +-----------------+

                    |
                    v
             +--------------+
             |     Git      |
             +------+-------+
                    |
                    v
             +--------------+
             |    GitHub    |
             +--------------+

## 🔄 Complete Project Workflow

```text
START
  |
  v
Launch EC2 Instance
  |
  v
Connect using SSH
  |
  v
Perform Linux Administration
  |
  v
Create EBS Volume
  |
  v
Attach EBS Volume to EC2
  |
  v
Identify Storage Device
  |
  v
Format EBS Volume
  |
  v
Create Mount Point
  |
  v
Mount EBS Volume
  |
  v
Create and Manage Files
  |
  v
Configure CloudWatch
  |
  v
Monitor CPU Utilization
  |
  v
Git Version Control
  |
  v
Push Project to GitHub
  |
  v
END
```

---

## 💾 Amazon EBS Implementation

Amazon Elastic Block Store (EBS) was implemented to provide persistent block-level storage for the EC2 instance.

### EBS Implementation Steps

### 1. Create EBS Volume

An additional EBS volume was created using the AWS Management Console.

### 2. Attach EBS Volume

The EBS volume was attached to the running EC2 instance.

### 3. Identify Storage Device

The attached storage device was identified using:

```bash
lsblk
```

### 4. Format EBS Volume

The EBS volume was formatted using the XFS filesystem:

```bash
sudo mkfs -t xfs /dev/nvme1n1
```

### 5. Create Mount Point

A mount directory was created:

```bash
sudo mkdir /index
```

### 6. Mount EBS Volume

The EBS volume was mounted to the `/index` directory:

```bash
sudo mount /dev/nvme1n1 /index
```

### 7. Create and Manage Files

A test file was created inside the mounted EBS storage:

```bash
touch /index/test.txt
```

The file was verified using:

```bash
ls -lh /index
```

### 8. Verify Storage

Disk usage was checked using:

```bash
df -h
```

The EBS volume was successfully formatted, mounted, and used for storing data.
---

## 💻 Amazon EC2 Implementation

Amazon EC2 was used as the main compute resource for this project.

### EC2 Tasks Performed

- Launched an Amazon Linux EC2 instance
- Connected to the instance using SSH
- Performed Linux command-line operations
- Checked system information
- Checked storage information
- Managed the EC2 environment
- Attached EBS storage
- Monitored the instance using CloudWatch

---

## 🔐 SSH Connection

The EC2 instance was accessed remotely using SSH.

Example:

```bash
ssh -i <key-file.pem> ec2-user@<public-ip>
SSH provided secure remote access to the Linux EC2 instance.

---

## 📊 Amazon CloudWatch Implementation

Amazon CloudWatch was used to monitor the EC2 instance and observe its performance.

### Monitoring Performed

- CPU Utilization
- EC2 performance metrics
- Resource monitoring
- Performance activity over time

CloudWatch helped in understanding EC2 performance and resource utilization.

---

## 🔧 Git Version Control

Git was used for version control and project management.

### Git Tasks Performed

- Installed Git
- Initialized a Git repository
- Configured Git user
- Added project files
- Created commits
- Created and used the main branch
- Connected the local repository with GitHub
- Pushed project changes to GitHub

---

## 🐙 GitHub

GitHub was used to store the project and maintain project documentation.

The project repository contains the implementation details, AWS architecture, commands, and learning outcomes.

---

## 📁 Project Structure

```text
AWS-EC2-Monitoring-Project/
|
+-- README.md
---

## 🛠️ Tools and Technologies

| Technology | Purpose |
|---|---|
| Amazon EC2 | Compute Resource |
| Amazon EBS | Persistent Block Storage |
| Amazon CloudWatch | Monitoring and Metrics |
| Amazon Linux | Operating System |
| SSH | Secure Remote Access |
| Git | Version Control |
| GitHub | Repository and Project Management |

---

## 🎯 Skills Demonstrated

- AWS EC2 Instance Management
- Amazon EBS Storage Management
- Linux System Administration
- SSH Remote Access
- Disk Formatting and Mounting
- File and Storage Management
- Amazon CloudWatch Monitoring
- CPU Utilization Monitoring
- Git Version Control
- GitHub Repository Management
- Basic DevOps Practices

---

## 📚 Key Learning Outcomes

Through this project, I gained practical experience in:

- Launching and managing Amazon EC2 instances
- Connecting to Linux servers using SSH
- Creating and attaching EBS volumes
- Formatting and mounting EBS storage
- Managing files on mounted storage
- Monitoring EC2 performance using CloudWatch
- Understanding CPU Utilization metrics
- Using Linux command-line operations
- Using Git for version control
- Managing and documenting projects using GitHub
- Understanding fundamental AWS Cloud and DevOps concepts

---

## 🚀 Future Improvements

The project can be extended by implementing:

- CloudWatch Alarms
- Amazon SNS Notifications
- IAM Security Configuration
- Automated EBS Snapshots
- Infrastructure as Code using Terraform
- Docker Deployment
- CI/CD Pipeline
- Automated Monitoring and Alerting

---

## ⭐ Project Highlights

- Hands-on AWS EC2 implementation
- EBS storage configuration and management
- CloudWatch performance monitoring
- Linux server administration
- SSH-based remote access
- Git and GitHub integration
- Practical cloud infrastructure experience
- Basic DevOps workflow implementation

---

## 👩‍💻 Author

**Megha Gole**

AWS Cloud & DevOps Learner

---

## 📝 Conclusion

This project provided hands-on experience with AWS cloud infrastructure, EC2 compute resources, EBS persistent storage, CloudWatch monitoring, Linux administration, and Git/GitHub version control.

The project demonstrates the practical implementation of fundamental AWS Cloud and basic DevOps concepts in a real-world style infrastructure environment.
