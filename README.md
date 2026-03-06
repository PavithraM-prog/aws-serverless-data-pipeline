# aws-serverless-data-pipeline
## Overview
This project demonstrates a **serverless data processing pipeline** using AWS services. When a CSV file is uploaded to Amazon S3, an **AWS Lambda** function automatically processes the data and stores results in **Amazon DynamoDB**. Logs are recorded in **CloudWatch**.

## Architecture
User->AmazonS3(upload csv)->Trigger AWS Lambda-> Amazon DynamoDB->CloudWatch Logs 

## AWS Services Used
- Amazon S3 – to store CSV files  
- AWS Lambda – to process data automatically  
- Amazon DynamoDB – to store processed results  
- Amazon CloudWatch – to monitor logs  
- AWS IAM – to manage permissions  

## Workflow
1. Upload CSV dataset to S3 bucket  
2. S3 triggers the Lambda function  
3. Lambda reads the CSV, calculates total_price per row  
4. Processed data stored in DynamoDB  
5. Logs recorded in CloudWatch  

## Dataset
Sample sales dataset (`sales_data.csv`) used for demonstration:

## Key Learning Outcomes
* Building event-driven serverless architectures
* AWS Lambda function development
* Working with S3, DynamoDB, and CloudWatch
* Managing AWS IAM roles and permissions
* Understanding basic cloud automation pipelines
