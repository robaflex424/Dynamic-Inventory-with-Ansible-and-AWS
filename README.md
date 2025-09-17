# Dynamic Inventory with Ansible and AWS

This small project demonstrates how **Ansible dynamic inventories** work using **AWS EC2** instances.  
Instead of manually maintaining a static `hosts` file, the inventory is automatically fetched from AWS using the **boto3** and **botocore** Python libraries.

---

## Requirements

Before starting, ensure you have:

1. An **AWS key pair** to access your EC2 instance(s).  
   - You can create or import one via the AWS Management Console or CLI.  
   - Keep the `.pem` file safe and secure.

2. **AWS credentials** configured on your system. You can set these up using the AWS CLI or environment variables.

---

## Setup Instructions

1. **Install Python 3** and create a virtual environment.  
2. **Activate the virtual environment**.  
3. **Install Python dependencies**:  
   - **boto3**  
   - **botocore**  
   - **ansible**

If you dont have python and all the dependencies installed, follow the commands in **python_configure.txt**.

---

## Usage

Once setup is complete, you can run **Ansible commands** with the dynamic inventory plugin to automatically fetch EC2 instance information.  

---

## Notes

- The `aws_ec2.yml` file defines how Ansible queries AWS for instance information.  
- **boto3** automatically picks up your AWS credentials from environment variables, AWS CLI config files, or IAM roles if running inside AWS.  

---

**Repo Description:**  
A sample **Ansible** project demonstrating **dynamic inventory** with **AWS EC2**, using **boto3** and **botocore**.  
