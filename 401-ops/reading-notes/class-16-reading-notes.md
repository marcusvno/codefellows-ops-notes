# Class 16 Reading Assignment

## Cloud Identity and Access Management (IAM) with AWS

- Lessons Learned from the Capital One Data Breach (PDF) - ([pdf](https://www.zscaler.com/resources/white-papers/capital-one-data-breach.pdf))

## Questions

1. **What were the three commands used for the attack?**
    - **Get Credentials -** First command when executed obtained security credentials known as \*\*\*\*-WAF-Role account (an IAM account) for an elevated role access AWS Web Application Firewall (WAF)
    - **List Buckets -** Second command, when executed, used the security credentials \*\*\*\*\*-WAF-Role account to list files and folders (aka S3 buckets)
    - **Download Files -** Third command, when executed used the \*\*\*\*\*-WAF-Role account to download files that were accessible by the credentials.

2. **What misconfiguration of AWS components allowed the attacker to access sensitive data?**
    - The attackers identified a misconfigured WAF that enabled accessing the corresponding AWS EC2 instanceECS task *metadata* using Server-side REquest Forgery (SSRF) and call the metadata service endpoint using an iam security-credentials command.
      - The endpoint must have returned a role that they could use.
    - From there, they used those roles to gain access to temporary credentials and used AWS CLI to access S3 buckets and sync.
    - In short, the misconfigured components were:
      - An AWS Web App Firewall
      - IAM role access to S3
      - EC2
      - S3 Bucket
3. **What are two of the AWS Governance practices that could have prevented such attack?**
    - Review all access paths and permissions from human identities or non-human identities (ec2 machine) to data storages (s3 buckets). Use CEIM solutiosn to automate detection of over-privileged identities and over-exposed data.
    - Clean up unused cloud resources (especially EC2 instances and S3 buckets) leftover from prior development or production debugging efforts.

## Things I Want to Know More About

Where can I find other white papers like this?
