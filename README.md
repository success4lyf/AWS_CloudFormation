# AWS_CloudFormation
A simple CloudFormation repository to show how to create and deploy s3 and lambda templates in stack.

## Deploying Templates To CloudFormation Stacks
A CloudFormation template is a declaration of AWS resources that make up a stack. The template is stored as either a JSON or YAML file, since they are just text files they can be edited using any text editor and managed in source control system with the rest of your code.

### Template1: S3 Bucket
This template is for a simple s3 bucket. The template will be uploaded to a s3 bucket befor deploying to stack. The code to upload the template to s3 bucket is:
```python
aws s3 cp templates/template1-s3-bucket.yaml s3://<bucket-name>/templates/template1-s3-bucket.yaml
```

Exercise 1: Extend this template by adding another S3 bucket. You will have to update the CloudFormation template, upload the revision to S3 and run the aws cloudformation update-stack command.


### Template2: Lambda Function

### Template3: Lambda Function with S3 Trigger

### Template4: Lambda Deployment Packages
