\# Secure S3 Storage

\## Project Report



\---



\# Cover Page



\# Secure S3 Storage



\### AWS Cloud Security Project



\*\*Project Name:\*\* Secure S3 Storage



\*\*Prepared By:\*\*  

\*\*Teja Srinivas\*\*



B.Tech – Computer Science Engineering (Cyber Security)



Sri Venkateswara College of Engineering (SVCE), Tirupati



Academic Year: 2026–2027



Project Type:



AWS Cloud Security Hands-on Project



\---



\# Declaration



I hereby declare that this project report entitled \*\*"Secure S3 Storage"\*\* is my own work completed as part of my AWS Cloud Security learning roadmap.



The project demonstrates practical implementation of Amazon S3 security features including Versioning, Bucket Policies, Server-Side Encryption, Lifecycle Management, Static Website Hosting, and secure EC2 integration using IAM Roles.



The work presented in this report is intended solely for educational and portfolio purposes.



\---



\# Acknowledgement



I sincerely thank everyone who contributed to my learning throughout this project.



Special thanks to AWS Documentation and practical cloud security resources that helped me understand Amazon S3 security concepts and best practices.



This project significantly improved my practical understanding of AWS Cloud Storage Security.



\---



\# Table of Contents



1\. Introduction

2\. Project Objectives

3\. Amazon S3 Overview

4\. AWS Services Used

5\. Project Architecture

6\. Security Features

7\. Implementation Steps

8\. Practical Labs

9\. Challenges Faced

10\. Learning Outcomes

11\. Best Practices

12\. Conclusion

13\. References



\---



\# 1. Introduction



Amazon Simple Storage Service (Amazon S3) is one of the most widely used cloud storage services provided by Amazon Web Services (AWS). It provides scalable, highly durable, secure, and highly available object storage for organizations of all sizes.



In modern cloud environments, protecting data stored in Amazon S3 is a critical responsibility. AWS provides several built-in security mechanisms including Bucket Policies, IAM, Versioning, Encryption, Lifecycle Management, and Public Access Controls.



The objective of this project is to build a secure Amazon S3 environment by implementing AWS security best practices while gaining practical hands-on experience.



\---



\# 2. Project Objectives



The primary objectives of this project are:



\- Create a secure Amazon S3 bucket

\- Upload and manage objects

\- Configure Bucket Policies

\- Enable Versioning

\- Enable Server-Side Encryption

\- Configure Lifecycle Rules

\- Demonstrate Static Website Hosting

\- Secure EC2 access using IAM Roles

\- Implement AWS security best practices

\- Document the complete implementation



\---



\# 3. Amazon S3 Overview



Amazon S3 is an object storage service designed for scalability, durability, availability, security, and performance.



Amazon S3 stores files as objects inside buckets.



Each object contains:



\- Data

\- Metadata

\- Object Key



Amazon S3 provides:



\- 99.999999999% (11 9's) durability

\- High availability

\- Unlimited storage capacity

\- Fine-grained access control

\- Encryption support

\- Lifecycle automation



\---



\# 4. AWS Services Used



The following AWS services were used during this project.



| Service | Purpose |

|----------|----------|

| Amazon S3 | Object Storage |

| Amazon EC2 | Compute Instance |

| AWS IAM | Identity Management |

| IAM Roles | Secure EC2 Access |

| Bucket Policy | Resource-based Permissions |

| Versioning | Object Recovery |

| SSE-S3 | Server-side Encryption |

| Lifecycle Rules | Automated Object Management |

| Static Website Hosting | Website Hosting |



\---



\# 5. Project Architecture



```

&#x20;                   Internet

&#x20;                        │

&#x20;                        ▼

&#x20;               Amazon S3 Bucket

&#x20;       ┌────────────────────────────┐

&#x20;       │                            │

&#x20;       │ Versioning                 │

&#x20;       │ Encryption                 │

&#x20;       │ Lifecycle Rule             │

&#x20;       │ Bucket Policy              │

&#x20;       │ Public Access Block        │

&#x20;       └─────────────┬──────────────┘

&#x20;                     │

&#x20;         Temporary Credentials

&#x20;                     │

&#x20;                IAM Role

&#x20;                     │

&#x20;                     ▼

&#x20;                Amazon EC2

```



\---



\# 6. Security Features Implemented



\## 6.1 Block Public Access



Enabled Block Public Access to prevent accidental public exposure of sensitive data.



Benefits



\- Prevents unauthorized access

\- Protects confidential information

\- Reduces security risks



\---



\## 6.2 Versioning



Enabled Versioning to maintain multiple versions of objects.



Benefits



\- Recover deleted files

\- Restore overwritten files

\- Protection against accidental deletion



\---



\## 6.3 Server-Side Encryption



Enabled default encryption using SSE-S3.



Benefits



\- Automatic encryption

\- No application changes required

\- Secure storage of data



\---



\## 6.4 Bucket Policy



Configured Bucket Policies following the Principle of Least Privilege.



Benefits



\- Fine-grained permissions

\- Secure resource access

\- Better compliance



\---



\## 6.5 Lifecycle Rules



Configured Lifecycle Rules to automatically transition and delete objects.



Benefits



\- Cost optimization

\- Automated storage management

\- Reduced manual administration



\---



\## 6.6 Static Website Hosting



Configured Amazon S3 to host a static website.



Features



\- HTML hosting

\- Public website endpoint

\- Lightweight hosting solution



\---



\## 6.7 IAM Role Integration



Configured EC2 to securely access Amazon S3 using IAM Roles.



Benefits



\- No Access Keys stored

\- Temporary credentials

\- AWS recommended security practice



\---



\# 7. Implementation Steps



The following implementation was performed.



\## Step 1



Created Amazon S3 Bucket



Screenshot



```

screenshots/bucket-created.png

```



\---



\## Step 2



Uploaded Objects



Screenshot



```

screenshots/uploaded-objects.png

```



\---



\## Step 3



Enabled Versioning



Screenshot



```

screenshots/versioning-enabled.png

```



\---



\## Step 4



Configured Bucket Policy



Screenshot



```

screenshots/bucket-policy.png

```



\---



\## Step 5



Enabled Default Encryption



Screenshot



```

screenshots/encryption-enabled.png

```



\---



\## Step 6



Created Lifecycle Rule



Screenshot



```

screenshots/lifecycle-rule-created.png

```



\---



\## Step 7



Enabled Static Website Hosting



Screenshot



```

screenshots/static-website-browser.png

```



\---



\## Step 8



Configured EC2 IAM Role Access



Screenshot



```

screenshots/ec2-iam-role.png

```



\---



\# 8. Practical Labs Completed



The following practical labs were completed successfully.



\## Lab 1



Create Amazon S3 Bucket



Completed



\---



\## Lab 2



Upload



Download



Delete Objects



Completed



\---



\## Lab 3



Enable Versioning



Modify Objects



Restore Previous Versions



Completed



\---



\## Lab 4



Bucket Policy



Permission Testing



Completed



\---



\## Lab 5



Server-side Encryption



Encrypted Object Upload



Completed



\---



\## Lab 6



Lifecycle Rules



Transition Objects



Automatic Object Deletion



Completed



\---



\## Lab 7



Static Website Hosting



Website Endpoint



Public Access Configuration



Completed



\---



\## Lab 8



IAM Role Access



Secure EC2 Integration



AWS CLI Verification



Completed



\---



\# 9. Challenges Faced



During the project, the following challenges were encountered.



\- Bucket Policy syntax validation

\- Static Website public access configuration

\- Understanding Block Public Access behavior

\- IAM Role permissions

\- Lifecycle Rule configuration

\- AWS CLI authentication

\- Secure EC2 access using IAM Roles



These challenges were resolved using AWS documentation and troubleshooting techniques.



\---



\# 10. Learning Outcomes



After completing this project, I gained practical experience in:



\- Amazon S3 Administration

\- AWS Identity and Access Management

\- Resource-based Policies

\- Object Versioning

\- Server-side Encryption

\- Lifecycle Management

\- Static Website Hosting

\- IAM Roles

\- AWS CLI

\- Cloud Storage Security

\- Principle of Least Privilege

\- AWS Security Best Practices



\---



\# 11. AWS Security Best Practices Followed



\- Enabled Versioning

\- Enabled Encryption

\- Used IAM Roles instead of Access Keys

\- Applied Principle of Least Privilege

\- Configured Lifecycle Rules

\- Used Bucket Policies

\- Re-enabled Block Public Access after demonstration

\- Avoided storing credentials on EC2



\---



\# 12. Future Improvements



The project can be further enhanced using:



\- Amazon CloudFront

\- AWS WAF

\- AWS KMS

\- Cross Region Replication

\- Event Notifications

\- AWS Lambda

\- Amazon Macie

\- AWS Config

\- AWS CloudTrail

\- Amazon GuardDuty



\---



\# 13. Conclusion



The Secure S3 Storage project successfully demonstrated the implementation of secure cloud storage using Amazon S3.



Throughout the project, multiple AWS security features were implemented including Versioning, Server-Side Encryption, Lifecycle Rules, Bucket Policies, IAM Role integration, and Static Website Hosting.



The project provided valuable hands-on experience in securing cloud storage resources while following AWS security best practices.



This project strengthened my practical understanding of Amazon S3 administration and cloud security and serves as a strong portfolio project for Cloud Security and AWS-related roles.



\---



\# References



1\. AWS Official Documentation

&#x20;  https://docs.aws.amazon.com/



2\. Amazon S3 Documentation

&#x20;  https://docs.aws.amazon.com/s3/



3\. AWS IAM Documentation

&#x20;  https://docs.aws.amazon.com/iam/



4\. AWS Well-Architected Framework



5\. AWS Security Best Practices



6\. AWS Cloud Practitioner Documentation



\---



\# End of Report

