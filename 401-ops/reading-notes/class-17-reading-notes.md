# Class 17 Reading Assignment

## Cloud Network Security

- IBM Cloud Learn Hub - What is a _Virtual Private Cloud_ ([article](https://www.ibm.com/cloud/learn/vpc))

## Questions

1. **What are some of the key features of the VPC model?**

- VPCs are a hybrid "best of both worlds" approach to cloud computing, giving customers the advantages of private clouds while leveraging public cloud resources and savings. Some features include:
  - **Agility:** Control the size of the virtual network and deploy cloud resources whenever business needs them. Scale resources dynamically and in real time.
  - **Availability:** Redundant resources and highly fault-tolerant availability zone architectures mean your applications and workloads are highly available.
  - **Security:** VPCs are logically isolated networks, meaning data and applications won't share space or mix with those of the cloud provider's other customers. Customer has full control over how resources and workloads are accessed and by whom.

2. **What are the three tiers that comprise the three-tier architecture model?**

- A three tier application architecture on a VPC is made by assigning each tier its own _subnet_, which will give it its own IP address. Each layer is then automatically assigned its own unique ACL. The three tiers are as follows:
  - **Web or presentation tier -** takes requests from web browsers and presents infomration created by, or stored within, the other layers to end users.
  - **Application tier -** houses the business logic and where most of the processing takes.
  - **Database tier -** comprises the database servers that store the data processed in the application tier.

3. **Describe the differences between a VPC and a VPN to someone you know from your previous job.**
    - A VPN is like a private tunnel that connects your PC to the internet; no one can peek on the data traveling from the exit to your home. A VPC is like a private neighborhood, allowing for multiple layers of security, subsectors, and multiple devices.
