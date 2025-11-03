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

###🗃️ 2. S3 (Simple Storage Service)
* aws s3 ls 👉 List all buckets
* aws s3 mb s3://my-bucket-name  👉 Make (create) a new bucket
* aws s3 cp file.txt s3://my-bucket-name/   👉 Upload file
* aws s3 cp s3://my-bucket-name/file.txt .  👉 Download file
* aws s3 rm s3://my-bucket-name/file.txt    👉 Delete file
* aws s3 rb s3://my-bucket-name --force     👉 Delete bucket

### 👤 3. IAM (Identity and Access Management)
* aws iam list-users 👉 List all users
* aws iam create-user --user-name newuser 👉 For Creating IAM User
* aws iam delete-user --user-name newuser 👉 For Deleting IAM User
* aws iam list-roles  👉 List all IAM roles

### 🧱 4. CloudFormation
* aws cloudformation create-stack --stack-name mystack --template-body file://template.yaml
* aws cloudformation describe-stacks
* aws cloudformation delete-stack --stack-name mystack

### 🗂️ 5. Lambda
* aws lambda list-functions
* aws lambda invoke --function-name myLambda output.txt

### 📦 6. ECR (Elastic Container Registry)
* aws ecr describe-repositories
* aws ecr create-repository --repository-name my-repo
* aws ecr delete-repository --repository-name my-repo --force

### 🌍 7. General Info
* aws --version         👉 Check AWS CLI version
* aws help              👉 Show help
* aws <service> help    👉 Show service-specific help (e.g., aws s3 help)
