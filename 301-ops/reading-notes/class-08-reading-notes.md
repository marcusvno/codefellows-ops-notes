# Class 08 Reading Assignment

## RADIUS Authentication

**Computer Network | AAA (Authentication, Authorization, Accounting)** ([article](https://www.geeksforgeeks.org/computer-network-aaa-authentication-authorization-and-accounting/))

1. **Explain each of the three A’s as you would to a non-technical family member. Use an analogy or a story.**
   - Assume you're a cook at a restaurant. Authentication is proving you work there, authorization is seeing what fridges you can unlock and what you are allowed to cook, and accounting is keeping track of what you've cooked and how much it costs.
2. **What should the administrator do if the ACS server fails to authenticate a user during AAA implementation?**
   - The administrator should mention using the local database of the device as a backup, in the method list, to implement AAA.
3. **What is the role of the NAS in the AAA implementation using an ACS server? Use a diagram.**
   - The client or Network Access Server (NAS) sends authentication requests to the ACS server and the server takes the decision to allow the user to access the network resource or not according to the credentials provided by the user.

![AAA network diagram](https://techhub.hpe.com/eginfolib/networking/docs/switches/5130ei/5200-3946_security_cg/content/images/image1.png)

(Image from HP Enterprise)

## RADIUS Concepts ([article](https://archive.is/27Y19#selection-2061.0-2077.160))

1. **What are the benefits of using RADIUS for authentication and authorization?**
   - RADIUS enables a company to maintain user profiles in a central database that all remote servers can share. Having a central database provides better security, enabling a company to set up a policy that can be applied at a single administered network point. A central database also makes it easier to track usage for billing for the network access or internet service provider and for keeping network statistics.
2. **What is RADIUS and what does it stand for?**
   - RADIUS (Remote Authentication Dial-In User Service) is a client-server protocol and software that enables remote access servers to communicate with a central server to authenticate dial-in users and authorize their access to the requested system or service.
3. **Research: What encryption algorithms does RADIUS use?**
   - **Password Authentication Protocol (PAP) -** The RADIUS client forwards the remote user's user ID and password to the RADIUS authentication server. If the credentials are correct, the server authenticates the user and the RADIUS client enables the remote user to connect to the network.
   - **Challenge Handshake Authentication Protocol (CHAP) -** Also known as a three-way handshake, CHAP authentication relies on the client and server using an encrypted shared secret. Compared to PAP, CHAP authentication is considered more secure because it encrypts authentication exchanges and it can be configured to do repeated mid-session authentications

![radius protocol architecture](https://archive.is/27Y19/65f5e54fc396b8bbab5b03c23a026a5ad255436e.png)

(Image from TechTarget)

## Additional Resources

- Authentication Methods ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/authentication-methods-n10-008/))
- Defense in Depth ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/defense-in-depth-n10-008/))
- RADIUS and TACACS ([video](https://www.professormesser.com/security-plus/sy0-401/radius-and-tacacs-2/))
- Kerberos ([video](https://www.professormesser.com/security-plus/sy0-401/kerberos-2/))

## Things I Want to Know More About

Is RADIUS a foundational protocol, like IP, and what else is built on it (aside from Microsoft Azure)
