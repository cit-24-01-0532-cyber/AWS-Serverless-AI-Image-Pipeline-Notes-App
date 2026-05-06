# AWS-Serverless-AI-Image-Pipeline-Notes-App
## Overview
This project is a serverless application built on AWS. It demonstrates two core cloud computing patterns:
1. **Event-Driven Image Processing:** Utilizing S3 triggers and AWS Lambda to automatically process/copy images between buckets.
2. **Serverless Web Hosting:** A secure note-taking frontend application hosted on Amazon S3.

## Technical Stack
- **AWS Lambda:** Serverless compute for image processing (Python/Boto3).
- **Amazon S3:** Used for static website hosting and object storage.
- **Infrastructure:** Managed via EC2 and Auto Scaling Groups (ASG) for scalable compute power.
- **Scheduling:** Amazon EventBridge (Cron) for automated tasks.

## Workflow
1. User uploads an image to `cloudmart-source-image`.
2. S3 triggers the `imageresizerfunction` (Lambda).
3. Image is processed and stored in `cloudmart-resized-image-isara`.
   
