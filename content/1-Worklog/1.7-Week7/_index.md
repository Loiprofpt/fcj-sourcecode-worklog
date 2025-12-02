---
title: "Week 7 Worklog"
date: "2025-09-10"
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---
{{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}}


### Week 7 Objectives:

* Acquire comprehensive knowledge of **AWS Lambda** and its role in serverless computing architectures.
* Develop proficiency in **AWS CLI** installation, configuration, and deployment of Java functions to Lambda.
* Understand the integration patterns between **API Gateway** and **AWS Lambda** for building scalable backend APIs.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ----------------------------------------- |
| Mon   | - Gain an overview of AWS Lambda: core concepts, architectural principles, benefits of the serverless model, and function execution flow | 20/10/2025 | 20/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Tue   | - Explore AWS CLI: functionality, installation procedures, IAM User configuration for AWS account access, and basic command syntax | 21/10/2025 | 21/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Wed   | - Execute AWS CLI installation on a local machine, configure credentials, and conduct testing with resource management commands (S3, EC2, Lambda) | 22/10/2025 | 22/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Thu   | - Study the Java function deployment workflow to AWS Lambda: Maven project preparation, .jar file packaging, and function creation/upload via AWS CLI | 23/10/2025 | 23/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Fri   | - Practice deploying a Java function to Lambda through AWS CLI, configure appropriate IAM roles, and execute function operational tests | 24/10/2025 | 24/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Sat   | - Examine API Gateway integration with AWS Lambda for backend API development; configure endpoints and perform API call validation | 25/10/2025 | 25/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| Sun   | - Synthesize knowledge on Lambda, API Gateway, and AWS CLI relationships; document deployment procedures and prepare the weekly report | 26/10/2025 | 26/10/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 7 Achievements:

#### 1. Comprehensive Understanding of AWS Lambda

* Successfully grasped the fundamental concepts and role of **AWS Lambda** within serverless computing paradigms.

* Thoroughly understood Lambda's operational mechanism encompassing trigger activation, function execution lifecycle, and result delivery.

* Clearly distinguished architectural and operational differences between **Lambda** and **EC2** across multiple dimensions:
  * Infrastructure management responsibilities
  * Cost models and billing structures
  * Scalability characteristics and operational flexibility

#### 2. Proficiency with AWS CLI

* Successfully installed and configured the **AWS CLI** on a personal machine using appropriate IAM User credentials.

* Demonstrated practical expertise with essential CLI commands:
  * Enumeration of S3 bucket resources
  * Creation and retrieval of Lambda function metadata
  * Management of AWS cloud resources
  
* Acquired comprehensive understanding of AWS CLI request mechanisms and authentication protocols utilizing Access Key/Secret Key pairs.

#### 3. Practical Deployment Experience: Java Functions to AWS Lambda via CLI

* Constructed a Java project using **Maven** framework, implemented handler classes, and generated executable .jar artifacts.

* Successfully executed Lambda function deployment using the `aws lambda create-function` command for function upload and publication.

* Configured and assigned appropriate **IAM Role** policies to facilitate Lambda function execution with necessary permissions.

* Validated function operational integrity through systematic testing procedures.
