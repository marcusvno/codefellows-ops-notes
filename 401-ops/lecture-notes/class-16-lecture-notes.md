# Class 16 - Cloud IAM with AWS

## IAM : A High Level View

- **User Authentication:** IAM verifies user identities through methods like passwords and biometrics.
- **Access Control:** IAM determines user access to resources based o nroles and permissions.
- **Least Privilege:** IAM follows the principle of least privilege to limit access to what's necessary.
- **Account management:** IAM covers account creation, modification, and removal; ensuring proper account lifecycle management.

## AWS IAM

- **Why should we practice AWS IAM controls?**
  - IAM users, roles, and policies determine what user accounts are allowed to do.
  - Administrator clearances are the primary targets of threat actors looking for privilege escalation.
- **Example: Capital One Data Breach**
  - Metadata service had a server side request forgery (SSRF) vulnerability
  - IAM admin role played a major part of this.

<img src="https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-16/slides/assets/16_02.png" width=500px/>

- **What does the AWS IAM service do?**
  - Enables centralized control over access to AWS resource.
  - Allows us to create and manage users, groups, and roles.
  - Provides detailed loggings and auditing of user activity.
  - Used for security and compliance best practices.
    - _If properly configured_

## AWS IAM Objects

- **IAM objects include:**
  - Users
  - Groups
  - Roles
  - Policies
    - ARN
    - Principal
    - Actions
    - Conditions

![iam objects](https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-16/slides/assets/16_04.png)

![AWS IAM](https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-16/slides/assets/16_05.png)

### AWS IAM Users

- **AWS root user**
  - The root user has complete and unrestricted access to all AWS resources
  - It is absolute **critical** to secure the root account with a _strong and unique password_ PLUS _multifactor authentication_
    - Root account access should be **_rare_** and reserved fro critical account or services changes.
      - Regular IAM users with _appropriate permissions_ should be used for most day to day activities.

![iam groups](https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-16/slides/assets/16_07.png)

### AWS IAM Groups

 A **IAM Group** is a collection of IAM users. Similar to how Linux does groups, users can belong to multiple user groups.

- Groups cannot be nested. (No groups inside groups)
- Groups cannot be identified as a **"Principle"**

![iam roles](https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-16/slides/assets/16_08.png)

### AWS IAM Roles

- **What _is_ an IAM Role?**
  - An IAM role is an entity that defines a set of permissions for making AWS service requests.
- **What do IAM roles _do?_**
  - Roles allow you to grant temporary permission to users, services, or applications without sharing long-term access keys.
- **Example:**
  - Role access between production and development environments.

![iam policies](https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-16/slides/assets/16_09.png)

### AWS IAM Policies

- **Inline Policies**
  - Not reusable or modular policies.
  - A policy that is _embedded_ in an IAM identity (a user, group, or role)
  - Policy is an _inherent_ part of the identity.
    - Specific to a single identity and can't be detached or reused.
- **AWS managed policy**
  - A standalone policy that is created and administrated by AWS.
  - Standalone policies have their own **Amazon resource Name (ARN)** that includes the policy name.
