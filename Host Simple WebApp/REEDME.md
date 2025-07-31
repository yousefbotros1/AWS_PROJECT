# 🛠️ Simple Web Application Deployment on AWS

This project demonstrates the deployment of a **highly available**, **scalable**, and **secure web application** using native AWS services. The infrastructure is built for **resilience, monitoring, and automation** — ideal for production-grade applications.

---

## 🧱 Architecture Overview

The system uses **public and private subnets** inside a **Virtual Private Cloud (VPC)** to separate web servers and databases for security and control.

### 🔹 Public Subnet
- **Application Load Balancer (ALB)**: Distributes incoming traffic across EC2 instances in multiple Availability Zones.
- **Auto Scaling Group (ASG)**: Dynamically increases or decreases the number of EC2 instances based on demand.

### 🔹 Private Subnet
- **Amazon RDS (Multi-AZ)**: Highly available relational database (MySQL/PostgreSQL), automatically backed up and replicated across Availability Zones.

### 🔹 Security & Monitoring
- **Security Groups**: Fine-grained firewall rules to control traffic to EC2 and RDS.
- **Amazon CloudWatch**: Real-time monitoring of system performance and logs.
- **Amazon SNS**: Sends email alerts to developers based on triggered CloudWatch alarms.

---

### 📐 Architecture Diagram

<p align="center">
  <img src="https://github.com/user-attachments/assets/0e4ec2e0-05ec-47d0-9e37-f664896a8bb1" width="700">
</p>

---

## 🔁 High Availability & Scalability

- 🌐 **Multi-AZ Load Balancing** ensures traffic is distributed evenly across zones.
- 📈 **Auto Scaling** adjusts EC2 instance count based on traffic spikes or failures.
- 🧮 **Amazon RDS Multi-AZ** provides automatic failover support for the database layer.

---

## 👥 Users & Access Flow

1. **End Users** → access the website via the **Application Load Balancer**.
2. **Developers** → receive infrastructure alerts via **SNS emails** for real-time monitoring and debugging.

---

## ☁️ AWS Services Used

| AWS Service         | Role in Architecture |
|---------------------|----------------------|
| **Amazon EC2**      | Hosts the application code within auto-scaled instances |
| **Application Load Balancer (ALB)** | Routes incoming traffic to healthy EC2s |
| **Auto Scaling Group (ASG)** | Ensures compute scales based on demand |
| **Amazon RDS (Multi-AZ)** | Provides a fault-tolerant, managed database |
| **Amazon VPC**      | Isolated networking environment with subnets |
| **AWS IAM**         | Manages secure role-based access between services |
| **Amazon CloudWatch** | Monitors system health and performance |
| **Amazon SNS**      | Sends email notifications to developers |

---

## 🌐 Web Application Screenshot

The deployed web app is a **personal portfolio** site with the following sections:

- **WELCOME**
- **ABOUT**
- **SERVICES**
- **RESUME**
- **WORKS**
- **TESTIMONIALS**
- **CONTACT**

<p align="center">
  <img src="https://github.com/user-attachments/assets/7cdc4490-0039-42d6-8e60-6fc67258799e" width="700">
</p>

---

## 🧩 Folder Structure (optional)

```plaintext
Simple-WebApp-AWS/
├── cloudformation/         # Infrastructure-as-code templates
├── app/                    # Web application source code
├── screenshots/            # Screenshots for documentation
├── README.md
