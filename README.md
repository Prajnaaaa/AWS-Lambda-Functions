# AWS-Lambda-Functions
1. Add Two Numbers
Create a Lambda function in Python:
def lambda_handler(event, context):
    num1 = event.get('num1')
    num2 = event.get('num2')
    return {"sum": num1 + num2}
    
2. Store a Document in S3
import boto3
def lambda_handler(event, context):
    s3 = boto3.client('s3')
    bucket_name = "your-bucket-name"
    file_content = event['file_content']
    file_name = event['file_name']

    s3.put_object(Bucket=bucket_name, Key=file_name, Body=file_content)
    return {"message": "File uploaded successfully"}

