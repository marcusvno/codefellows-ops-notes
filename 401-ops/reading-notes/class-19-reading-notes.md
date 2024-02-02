# Class 19 Reading Assignment

## Cloud Detective Controls
- What is Amazon GuardDuty? ([link](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html))

## Questions

1. **What are some of the IoCs that GuardDuty can detect?**
    - Some of the Indicators of Compromise that Guard Duty can detect are unusual API calls, irregular traffic, and other indicators of possibly compromised accounts.
2. **What are some of the data sources which GuardDuty can use?**
    - VPC Flow Logs
    - AWS CloudTrail event logs
    - DNS logs
    - Kubernetes audit logs
    - RDS login activity
    - S3 logs
    - EBS volumes
    - Runtime monitoring
    - Lambda network activity logs
3. **How does GuardDuty use access behavior to spot potential malicious activity?**
    - GuardDuty establishes baseline user access habits to notice when things are abnormal. If a personal is usually only on from 9-5pm, a sudden login of 2am is beyond that baseline and may indicate as possible account compromise.


## Additional Resources

AWS re:Inforce 2019: Threat Detection on AWS: An Introduction to Amazon GuardDuty (FND216) ([video](https://www.youtube.com/watch?v=czsuZXQvD8E))

