# Install-AwsCli-Script
## What is AWSCLI..?
### Ans: AWS CLI (Amazon Web Services Command Line Interface) is a powerful tool that lets you interact with AWS services using command-line commands instead of the AWS Management Console.
* It allows developers, sysadmins, and DevOps engineers to automate tasks, manage resources, and control AWS services directly from the terminal.

## ⚙️ Why use AWS CLI?
### ANS:-
* Automate AWS operations (EC2, S3, IAM, etc.)
* Easily integrate with shell scripts or CI/CD tools
* Manage multiple AWS accounts and regions
* Quick and repeatable infrastructure management

## 🔐 Configure AWS CLI
### ANS:-
### Before using, configure credentials:
* aws configure
### You’ll be asked for:
* AWS Access Key ID: <your-access-key>
* AWS Secret Access Key: <your-secret-key>
* Default region name: ap-south-1
* Default output format: json

## 📋 Basic AWS CLI Commands
### ANS- 
### 🖥️ 1. EC2 (Elastic Compute Cloud)
* aws ec2 describe-instances 👉 List all EC2 instances
* aws ec2 start-instances --instance-ids i-0abcd1234efgh5678 👉 Start Instance
* aws ec2 stop-instances --instance-ids i-0abcd1234efgh5678  👉 Stop Instance
* aws ec2 terminate-instances --instance-ids i-0abcd1234efgh5678 👉 Stop Instance
* aws ec2 describe-volumes  👉 List EBS volumes

