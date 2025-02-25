# ☁️ MultiCloud, DevOps & AI Challenge - Day 1
## Automating AWS Provisioning of S3 Bucket and DynamoDB using Terraform
![dynamodb-terraform-s3](https://github.com/user-attachments/assets/6c3a4e29-f4e5-4939-8249-365d8ae44d8e)

## 📌 Project Overview
In this project, we automate the provisioning of an **S3 bucket** and a **DynamoDB table** using **Terraform**. These resources serve as the foundation for a cloud-based **eCommerce application**, where:
- **S3** stores application assets.
- **DynamoDB** acts as a NoSQL database to manage **products, orders, and customer tickets**.

---

## 🛠 Environments and Technologies Used
- **Terraform** 🏗️ - Infrastructure as Code (IaC)
- **Amazon Web Services (AWS)** ☁️ - Cloud Provider
- **GitHub Codespaces** 🖥️ - Dev Environment
- **S3** 🗄️ - Cloud Storage
- **DynamoDB** 📊 - NoSQL Database

---

## 🚀 Features
- ✅ **Automated AWS provisioning** using Terraform  
- ✅ **S3 bucket creation** for storing application assets  
- ✅ **DynamoDB table setup** to store eCommerce product, order, and ticket data  
- ✅ **Secure AWS authentication** using IAM roles  
- ✅ **Efficient and scalable cloud deployment**  

---

## 📜 Step-by-Step Instructions

### **1️⃣ AWS CLI & Terraform Setup**
💡 _Make sure you're using a Linux environment (or follow AWS documentation for other OS)._  

### **Install AWS CLI**
```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install


# **Terraform Installation & Configuration**

## **1️⃣ Install Terraform**

To install Terraform on a **Linux** system, follow these steps:

### **Step 1: Add HashiCorp GPG Key**
```sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/AmazonLinux/hashicorp.repo
sudo yum -y install terraform


## **2️⃣ Terraform Configuration**

In this step, we will ensure that Terraform is set up properly.

### **Create a Terraform Project Directory**
First, create a new directory for the Terraform project and navigate into it:
```bash
mkdir terraform-project && cd terraform-project
