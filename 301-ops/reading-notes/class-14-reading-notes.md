# Class 14 Reading Assignment

## Group Policy ([article](https://www.lepide.com/blog/what-is-group-policy-gpo-and-what-role-does-it-play-in-data-security/))

1. **What role does Group Policy play in Windows Active Directory?** - Group Policy is a feature of Windows that facilitates a wide variety of advanced settings that network administrators can use to control the working environment of users and computer accounts in Active Directory. It essentially provides a centralized place for administrators to manage and configure operating systems, applications, and users’ settings.
2. **Name and describe different ways GPOs can benefit security.** - GPOs can help implement a policy of least privilege where users only have the permissions they require to do their job, disable outdated protocols, prevent users from making certain changes, and can be used to deploy software updates and system patches to ensure your environment is healthy and up to date against the latest security threats.
3. **How can the acronym “LSDOU” help you figure out which policies are in effect?** - The order in which GPOs are processed affects what settings are applied to the computer and user. The order that GPOs are processed is known as LSDOU, which stands for local, site, domain, and organizational unit. The local computer policy is the first to be processed, followed by the site level to domain AD policies, then finally into organization units. If there happen to be conflicting policies in LSDOU, the last applied policies win out.

![diagram](https://www.lepide.com/blog/wp-content/uploads/2019/05/gpo-ad.png)

## Additional Resources

- Wireless Standards([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/wireless-standards-n10-008/))
- Wireless Technologies([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/wireless-technologies-n10-008/))
- Wireless Encryption([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/wireless-encryption-n10-008/))
