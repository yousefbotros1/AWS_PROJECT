🛠️ Simple Web Application Deployment on AWS

This project showcases a highly available and scalable web application architecture deployed on AWS. The infrastructure is designed for resilience, scalability, and security using native AWS services.
🧱 Architecture Components

    VPC: Isolated network environment with public and private subnets.

    Public Subnet:

        Application Load Balancer (ALB): Distributes incoming traffic across multiple EC2 instances in different Availability Zones.

        Auto Scaling Group: Automatically adjusts the number of EC2 instances based on traffic load, providing high availability and fault tolerance.

    Private Subnet:

        Amazon RDS (Multi-AZ): Managed relational database service with high availability, deployed across multiple Availability Zones.

    Security Groups: Control traffic to EC2 instances and RDS databases.

    Monitoring and Notifications:

        CloudWatch Alarms: Triggered by performance metrics.

        SNS (Simple Notification Service): Sends notifications (e.g., email alerts) to developers on infrastructure events.

🔁 High Availability & Scalability

    Utilizes Auto Scaling Groups across three Availability Zones for load distribution and fault tolerance.

    Amazon RDS Multi-AZ ensures database availability even during zone failures.

👥 Users & Access

    End users access the app via the Application Load Balancer.

    Developers receive monitoring alerts via SNS and Email for proactive troubleshooting.

![Simple APP Deployment  drawio](https://github.com/user-attachments/assets/0e4ec2e0-05ec-47d0-9e37-f664896a8bb1)


☁️ Key AWS Services Used

    Amazon EC2
    Hosts the web application with compute instances launched in an Auto Scaling Group.

    Application Load Balancer (ALB)
    Automatically distributes incoming application traffic across multiple EC2 instances in different Availability Zones.

    Auto Scaling Group (ASG)
    Maintains application availability by dynamically scaling the number of EC2 instances based on demand and health checks.

    Amazon RDS (Optional)
    Managed relational database service (MySQL/PostgreSQL) deployed in Multi-AZ mode for high availability and failover support.

    AWS IAM (Identity and Access Management)
    Enforces role-based access control for secure interactions between services (e.g., EC2 access to CloudWatch).

    Amazon CloudWatch & SNS
    Monitors application metrics and system logs, and sends notifications or alerts through SNS for proactive incident response.


he screenshot displays a personal portfolio website for Shreyas Shripad Kulkarni, a pre-final year BTech student in Information Technology.
🔹 Key Sections:

    WELCOME

    ABOUT

    SERVICES

    RESUME

    WORKS

    TESTIMONIALS

    CONTACT


![Screenshot from 2025-05-17 20-41-22](https://github.com/user-attachments/assets/7cdc4490-0039-42d6-8e60-6fc67258799e)

    
