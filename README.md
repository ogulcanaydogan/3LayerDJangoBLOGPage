# BlogDjango
BlogDjango

## Description

The Blog Page Application aims to deploy blog application as a web application written Django Framework on AWS Cloud Infrastructure. This infrastructure has Application Load Balancer with Auto Scaling Group of Elastic Compute Cloud (EC2) Instances and Relational Database Service (RDS) on defined VPC. Also, The Cloudfront and Route 53 services are located in front of the architecture and manage the traffic in secure. User is able to upload pictures and videos on own blog page and these are kept on S3 Bucket.


# Blog Project Tasks

## Infrastructure Setup

1. **Create VPC and all components**
   - Create VPC
   - Create Subnets
   - Create and attach an internet gateway
   - Create Route Tables
   - Create Endpoint

2. **Create Security Groups (ALB ---> EC2 ---> RDS)**
   - ALB Security Group
   - EC2 Security Groups
   - RDS Security Groups
   - NAT Instance Security Group

3. **Create RDS**
   - Create a subnet group for our custom VPC
   - Create Database
     - Database engine: `MySQL`
     - Version: `8.0.28`

4. **Create two S3 Buckets and set one of these as static website**
   - Failover Scenario
   - Web Site

## Application Deployment

5. **Copy files downloaded or cloned from Techproeducation repo on Github**
6. **Prepare your Github repository**
7. **Prepare a userdata to be utilized in Launch Template**
8. **Write RDS database endpoint and S3 Bucket name in settings file given by Developer and push your application into your own repo on Github**
9. **Create NAT Instance in Public Subnet**
10. **Create Launch Template and IAM role for it**
11. **Create certification for secure connection**
12. **Create ALB and Target Group**
13. **Create Autoscaling Group with Launch Template**
14. **Create Cloudfront in front of ALB**
15. **Create Route 53 with Failover settings**
16. **Create DynamoDB Table**
17. **Create Lambda function**
18. **Create S3 Event and set it as trigger for Lambda Function**

## Server Specifications

- **Operating System**: Ubuntu Server 20.04

## Project Skeleton 

```text
BlogDjango (folder)
|
|----Readme.md               # Given to the students (Definition of the project)
|----src (folder)            # Given to the students (Django Application's )
|----requirements.txt        # Given to the students (txt file)
|----lambda_function.py      # Given to the students (python file)
|----developer_notes.txt     # Given to the students (txt file)

