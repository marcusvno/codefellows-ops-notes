# Class 12 Reading Assignment

## Domain Controller ([link](https://www.howtogeek.com/194069/what-is-a-windows-domain-and-how-does-it-affect-my-pc/))

1. **Explain the role of a Domain Controller?**
   - Windows Domains are typically used by large networks to manage a large number of PCs and control them from one place. Domain controllers are the servers that have control over the domain and the computers on it.
2. **What is the benefit of being able to login with the same username and password on any computer joined to the domain? What are the security risks?**
   - The benefit of have a single login for the domain is that you have AAA on any computer on the domain. This allows for diminished risk of users creating simply passwords to avoid having to memorize multiple passwords. Users also do not have to memorize specific passwords for specific devices/computers. The risk, of course, is that if the password is compromised, it could give access to all devices on the domain.
3. **Describe how group policies are used in domains?**
   - Group policies on domains are used to manage systems, software, and users. Any changes to a group policy means that all computers on the domain will get these settings and override and local settings users specify on their PCs. All settings are controlled from a single place and are "locked down".
4. **In what other ways can you think of that domains could be used beyond what was presented in the reading?**
   - Software deployment, monitoring user changes and activities, and implementing rapid security changes when breaches are detected.

## Additional Resources

- Overview of DNS ([videos](https://www.professormesser.com/network-plus/n10-008/n10-008-video/an-overview-of-dns-n10-008/))
- DNS Record Types([videos](https://www.professormesser.com/network-plus/n10-008/n10-008-video/dns-record-types-n10-008/))

## Things I Want to Know More About

Does Linux have similar domain controllers? Clearly Windows Server is the Domain Controller for Window networks with Window endpoints, is it the same with Linux or is this where Enterprise Linux distros come in like, Red Hat?
