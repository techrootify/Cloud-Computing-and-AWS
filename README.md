# Cloud-Computing-and-AWS

Amazon Web Services (AWS) Guide

Introduction to Cloud Computing
Cloud computing is the practice of using internet-based resources like servers, storage, and applications instead of maintaining physical hardware. Businesses, from startups to large enterprises, benefit from its scalability and cost-effectiveness.

Cloud services are provided through data centers, which act as massive repositories of computing power and storage.

Cloud Computing Models
There are three main types of cloud computing models:

1. Infrastructure as a Service (IaaS): The cloud provider manages the entire infrastructure, including servers, networking, and storage.
2. Platform as a Service (PaaS): Clients can deploy applications on a managed platform without handling the underlying infrastructure.
3. Software as a Service (SaaS): Users access cloud-based applications provided by the cloud service provider.

Types of Cloud Computing

1. Public Cloud: Services are available to anyone (e.g., Google Drive, AWS, Azure).
2. Private Cloud: Exclusive to a single organization for security and customization.
3. Hybrid Cloud: A combination of public and private cloud services to optimize flexibility.

AWS Services Overview
AWS offers various services to meet diverse business needs. These services are accessible through the AWS Management Console.

1. Amazon EC2 (Elastic Compute Cloud)
EC2 provides virtual servers in the cloud, allowing businesses to deploy scalable computing power on demand.

Steps to Launch an EC2 Instance:
1. Navigate to AWS Console > EC2 > Launch Instance.
2. Provide a server name.
3. Select an operating system (e.g., RedHat 64-bit) within the free tier.
4. Choose machine specifications (e.g., 1 GB RAM, 1 vCPU).
5. Create a key pair and download it.
6. Configure security settings (enable SSH or RDP access).
7. Keep the default storage settings.
8. Click Launch Instance.

Connecting to an EC2 Instance:
- Via Windows Command Prompt:
  1. Open Command Prompt (Win + R > cmd).
  2. Navigate to the Downloads folder where the key pair is stored.
  3. Run the copied ssh -i command from the AWS Console.
  4. Type "yes" when prompted to establish the connection.

- Via PuTTY Software:
  1. Download and install PuTTY.
  2. Open PuTTYgen, load the .pem key, and save it as .ppk.
  3. Open PuTTY, navigate to Auth > Credentials, and browse for the .ppk file.
  4. Connect using the instance's IP or DNS name.
  5. Use ec2-user as the login username.

2. Amazon S3 (Simple Storage Service)
S3 provides scalable object storage with high availability, security, and performance.

Key Features of S3:
- Scalability, Availability, and Durability
- Cost-effective storage classes
- Robust security and access controls
- Data auditing and compliance
- On-demand data processing

Understanding S3 Objects and Buckets:
- Objects: Data stored in S3, along with metadata and versioning.
- Buckets: Containers that store objects and must be created before uploading files.

Example:
- Object: image.jpg
- Bucket Name: mybucket
- Storage Path: s3://mybucket/image.jpg
- Region: As per user selection

3. IAM (Identity and Access Management)
IAM is a security service that manages user access and permissions for AWS resources.

Key Features of IAM:
- Centralized user management and authentication
- Secure credential handling (access keys, passwords, MFA)
- Fine-grained permission control over AWS services

IAM enables organizations to create multiple user accounts under a single AWS account, restricting permissions based on roles and responsibilities.

Hosting a Static Website Using S3

Step 1: Configure Route 53 (AWS DNS Service)
1. Go to AWS Console > Route 53.
2. Create a hosted zone for managing DNS records.
3. Add an A record to link the domain to the S3 bucket.

Step 2: Create and Configure an S3 Bucket
1. Navigate to AWS Console > S3.
2. Create a bucket with your domain name (e.g., mywebsite.com).
3. Enable public access and versioning.
4. Upload index.html and error.html files.
5. Go to Properties > Static Website Hosting and enable it.

Step 3: Set Up Bucket Policy for Public Read Access
Ensure the S3 bucket allows public access for serving web content.

These notes provide a clear and professional breakdown of AWS fundamentals, making it easier to understand cloud computing concepts and AWS services.

--------------------------------------------

Be a part of the Tech Rootify community connect, support, and grow with us.

Website : https://www.techrootify.com/

YouTube : https://www.youtube.com/@techrootify

Instagram : https://www.instagram.com/techrootify/

GitHub : https://github.com/techrootify

LinkedIn : https://www.linkedin.com/company/techrootify/

Happy Tech Journey

