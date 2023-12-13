# Class 13 Reading Assignment

## Active Directory ([article](https://www.cyberark.com/what-is/active-directory/))

1. **What exactly is “Active Directory” and are the key services it provides?**
    - Active Directory (AD) is Microsoft’s directory and identity management service used in Windows domain networks to manage users and resources. Key services include management of user data, digital security certificates, identity and access sharing across organizations, and information rights management.
2. **What are the differences between a domain, forest, and tree in Active Directory?**
    - In AD, a domain is a collection of objects with a shared database, a tree is one or more domains with a contiguous namespace, and a forest is a collection of trees that share common components but not a contiguous namespace.
3. **How can objects (e.g. users, devices) within a domain be grouped?**
    - Objects within a domain can be grouped into organizational units (OU) to simplify administration and policy management. Administrators can create arbitrary organizational units to mirror functional, geographical, or business structures, and then apply group policies to OUs to simplify administration. OUs also make it easier to delegate control over resources to various administrators.
4. **Explain the benefits of Active Directory, as you would to a family member.**
    - Think of Active Directory as the head chef in a bustling kitchen. It ensures that all ingredients (network resources) are securely stored and only accessible to the right kitchen staff (users). No matter how busy the service gets, the kitchen is always ready to deliver (high availability), ensuring that diners (business operations) are never let down.

## Additional Resources

- DHCP Overview ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/dhcp-overview-n10-008/))
- Configuring DHCP ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/configuring-dhcp-n10-008/))

## Things I Want to Know More About

How does Active Directory link into Azure?
