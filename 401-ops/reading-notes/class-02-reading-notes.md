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
    - The key point about Lambda is that you don’t have to manage the infrastructure underneath the function you are running. No need to track the status of the physical hosts, no need to track the capacity of the fleet, no need to patch the OS where the function will be running. In a nutshell, no need to spend time and money on the undifferentiated heavy lifting.

## Additional Resources

- 13 Compliance Frameworks for Cloud-based Orgs
- Cloud Security Alliance (CSA)
  - Cloud Controls Matrix (CCM)
  - CSA Security Guidance for Cloud Computing

## Things I Want to Know More About
