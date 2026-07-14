\# Secure S3 Storage



\## Project Overview



Secure S3 Storage is an AWS cloud security project that demonstrates how to build a secure Amazon S3 environment by implementing AWS security best practices. The project covers secure object storage, version control, encryption, lifecycle management, IAM integration, and static website hosting.



This project was completed as part of an AWS Cloud Security learning roadmap.



\---



\## Objectives



\- Create a secure Amazon S3 bucket

\- Enable object versioning

\- Configure server-side encryption

\- Implement lifecycle management

\- Apply Bucket Policies

\- Integrate EC2 with S3 using IAM Roles

\- Demonstrate Static Website Hosting

\- Follow AWS security best practices



\---



\## AWS Services Used



\- Amazon S3

\- Amazon EC2

\- AWS IAM

\- IAM Roles

\- S3 Bucket Policies

\- Amazon S3 Versioning

\- Amazon S3 Lifecycle Rules

\- Amazon S3 Static Website Hosting



\---



\## Project Architecture



!\[Architecture](architecture/s3-architecture.png)



\---



\## Security Features Implemented



\### Block Public Access



Configured Block Public Access to protect sensitive data stored in the bucket.



\---



\### Versioning



Enabled Versioning to protect against accidental deletion and object overwrites.



\---



\### Server-Side Encryption



Enabled default encryption using Amazon S3 Managed Keys (SSE-S3 / AES-256).



\---



\### Bucket Policy



Configured Bucket Policies following the Principle of Least Privilege.



\---



\### Lifecycle Rule



Configured Lifecycle Rules to automatically transition objects and manage storage efficiently.



\---



\### IAM Role Integration



Attached an IAM Role to an EC2 instance to securely access Amazon S3 without storing AWS Access Keys.



\---



\## Practical Labs Completed



\- Create S3 Bucket

\- Upload and Download Objects

\- Delete Objects

\- Enable Versioning

\- Restore Previous Object Versions

\- Configure Bucket Policy

\- Enable Default Encryption

\- Create Lifecycle Rules

\- Static Website Hosting

\- EC2 Access to S3 using IAM Role



\---



\## Repository Structure



```

Secure-S3-Storage/

│

├── README.md

├── LICENSE

├── architecture/

├── diagrams/

├── docs/

└── screenshots/

```



\---



\## Screenshots



\### Bucket Created



!\[Bucket](screenshots/bucket-created.png)



\---



\### Versioning Enabled



!\[Versioning](screenshots/versioning-enabled.png)



\---



\### Encryption Enabled



!\[Encryption](screenshots/encryption-enabled.png)



\---



\### Lifecycle Rule



!\[Lifecycle](screenshots/lifecycle-rule-created.png)



\---



\### Bucket Policy



!\[Policy](screenshots/bucket-policy.png)



\---



\### Static Website



!\[Website](screenshots/static-website-browser.png)



\---



\### EC2 Access using IAM Role



!\[EC2](screenshots/ec2-upload-success.png)



\---



\## Learning Outcomes



After completing this project, I gained practical experience in:



\- Amazon S3 administration

\- AWS Identity and Access Management (IAM)

\- Secure object storage

\- Data encryption

\- Lifecycle automation

\- Resource-based access control

\- Static website hosting

\- AWS security best practices



\---



\## Future Improvements



\- Amazon CloudFront integration

\- SSE-KMS encryption

\- Cross-Region Replication

\- Event Notifications

\- AWS Lambda integration

\- Amazon Macie

\- Amazon GuardDuty

\- AWS Config Rules



\---



\## Author



\*\*Teja Srinivas\*\*



B.Tech – Computer Science Engineering (Cyber Security)



Cloud Security Engineer Aspirant



\---



\## License



This project is licensed under the MIT License.

