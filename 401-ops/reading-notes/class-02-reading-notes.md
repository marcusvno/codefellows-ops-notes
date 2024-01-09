# Class 02 Reading Assignment

## Cloud Security Principles and Frameworks

AWS Architecture Blog - Compute Abstractions on AWS: A Visual Story ([article](https://aws.amazon.com/blogs/architecture/compute-abstractions-on-aws-a-visual-story/))

## Question

1. **Explain the levels of abstraction in AWS to someone without a technical background.**
    - 
2. **What are the control plane and data plane responsible for in container abstraction?**
    - A containers data plane that is responsible for providing capacity (as in CPU/Memory/Network/Storage) so that those containers can actually run and connect to a network. From a practical perspective this is typically a Linux host or less often a Windows host where the containers get started and wired to the network.
    - A containers control plane that is responsible for exposing the API and interfaces to define, deploy, and lifecycle containers. This is also sometimes referred to as the container orchestration layer.
3. **Where does AWS Lambda fall in the layers of abstraction and what makes it so special?**
    - What makes Lambda so special is its event-driven model. Not only can you invoke Lambda directly (for example, via the Amazon API Gateway), but you can trigger a Lambda function upon an event in another AWS service (for example, an upload to Amazon S3 or a change in an Amazon DynamoDB table).

## Additional Resources

- 13 Compliance Frameworks for Cloud-based Orgs
- Cloud Security Alliance (CSA)
  - Cloud Controls Matrix (CCM)
  - CSA Security Guidance for Cloud Computing

## Things I Want to Know More About
