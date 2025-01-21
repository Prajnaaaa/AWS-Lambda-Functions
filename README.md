# AWS-Lambda-Functions

This repository contains two AWS Lambda functions:
1. **AddTwoNumbers**: A function that adds two numbers and returns the result.
2. **StoreDocumentInS3**: A function that stores a document or PDF file in an S3 bucket.

Task 1: AddTwoNumbers
Description:
This function takes two numbers as input and returns their sum.

Sample Input:
```json
{
    "num1": 5,
    "num2": 10
}
Sample Output:

{
    "statusCode": 200,
    "body": {
        "num1": 5,
        "num2": 10,
        "sum": 15
    }
}

Task 2: StoreDocumentInS3
Description:
This function takes a Base64 encoded document and stores it in the specified S3 bucket.

Sample Input:

{
    "file_content": "VGhpcyBpcyBhIHRlc3QgZG9jdW1lbnQ=",
    "file_name": "test-document.txt"
}

Sample Output:

{
    "statusCode": 200,
    "body": "File test-document.txt uploaded successfully to my-document-storage!"
}

Technologies Used:
AWS Lambda
Python
S3

