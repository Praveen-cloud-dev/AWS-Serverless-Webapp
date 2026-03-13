# AWS Serverless Web Application

## Project Overview

This project demonstrates a simple **serverless web application on AWS**.
It uses AWS services such as **Lambda, DynamoDB, and API Gateway** to create a scalable backend without managing servers.

The application tracks the number of visitors to the website using **AWS Lambda** and stores the count in **DynamoDB**.

---

## Architecture

The application works with the following components:

1. **Frontend**

   * HTML
   * CSS
   * JavaScript
     These files create the web interface.

2. **API Gateway**

   * Provides an HTTP endpoint for the frontend to communicate with AWS Lambda.

3. **AWS Lambda**

   * Executes Python code when the API is triggered.
   * Retrieves and updates visitor count in DynamoDB.

4. **DynamoDB**

   * Stores the visitor count in a table.

---

## Project Structure

```
AWS-Serverless-Webapp/
│
├── index.html        # Frontend HTML page
├── style.css         # Styling for the webpage
├── script.js         # JavaScript to call the API
└── lambda-function.py # Lambda function to update visitor count
```

---

## Lambda Function

The Lambda function performs the following actions:

1. Connects to DynamoDB using boto3.
2. Retrieves the current visitor count.
3. Increments the count.
4. Updates the DynamoDB table with the new value.
5. Returns the updated visitor count.

---

## AWS Services Used

* AWS Lambda
* Amazon DynamoDB
* Amazon API Gateway
* Amazon S3 (optional for static website hosting)

---

## How to Deploy

1. Create a DynamoDB table.
2. Deploy the Lambda function with the provided Python code.
3. Create an API Gateway endpoint and connect it to the Lambda function.
4. Upload frontend files to an S3 bucket (for static website hosting).
5. Update the API URL in `script.js`.

---

## Use Case

This project demonstrates how to build a **serverless visitor counter application** using AWS.

---

## Author

DevOps / Cloud Project
