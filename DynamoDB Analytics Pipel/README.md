# 🚀 DynamoDB Data Flow



This project enables seamless visualization of **DynamoDB data** in **Amazon QuickSight** using **AWS Athena** and **AWS Lambda**. It integrates several AWS services into a powerful and cost-effective **data analytics pipeline**.

---

## 📌 Overview

This pipeline connects your operational data stored in **Amazon DynamoDB** with **Amazon QuickSight**, allowing for **real-time dashboards** and **interactive analytics**. Using **Athena** (via the DynamoDB connector) and **S3** as an intermediate store, the pipeline is efficient and affordable — costing around **$1.30** total to run.

<p align="center">
  <img src="https://github.com/user-attachments/assets/e19ff0c7-28c8-4878-b6c6-d0d7b501efdb" width="600">
</p>

---

## 🧰 Technologies Used

- 🔹 **Amazon DynamoDB** – NoSQL database
- 🧠 **AWS Lambda** – Serverless compute to connect Athena and DynamoDB
- 📊 **Amazon QuickSight** – Business intelligence dashboards
- 🔍 **AWS Athena** – SQL query engine
- 🧪 **AWS Glue** – Data catalog and schema detection
- ☁️ **Amazon S3** – Spillover storage for Athena results

---

## 🌟 Features

- ✅ **DynamoDB Table Setup** with partition & sort keys
- ✅ **Lambda-Athena Integration** using DynamoDB Connector
- ✅ **S3 Spill Location** for Athena query results
- ✅ **IAM Role Configuration** to enable QuickSight access
- ✅ **Data Import & Visualization** using:
  - 🔹 **SPICE**
  - 🔹 **Direct Query**
  
<p align="center">
  <img src="https://github.com/user-attachments/assets/683ae8b3-f6e9-492b-81c9-292ad3cf05be" width="600">
</p>

- ✅ **Custom Dashboards**:
  - Donut Charts
  - Bar Charts
  - Interactive Tables
  
<p align="center">
  <img src="https://github.com/user-attachments/assets/a8c4de0c-c85c-4f4b-ad2a-3f255b8cc01a" width="600">
</p>

- ✅ **Live Data Sync**: Reflects changes in DynamoDB in real time
- 💲 **Cost Efficient**: Full setup costs about **$1.30**

<p align="center">
  <img src="https://github.com/user-attachments/assets/4a9749d5-1b4f-484f-a1d3-fb99dfe776f0" width="600">
</p>

---

## 📦 Folder Structure (if needed)

```plaintext
DynamoDB Analytics Pipeline/
├── lambda/                  # Lambda function code for Athena connector
├── glue/                    # Glue crawlers or schema definitions
├── templates/               # CloudFormation or setup templates
├── dashboards/              # Screenshots or QuickSight exports
└── README.md
