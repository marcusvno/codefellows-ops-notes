# Class 12 Reading Assignment

## Introduction to pfSense: an Open Source Firewall and Router Platform ([link](https://turbofuture.com/computers/Introduction-to-pfSense-An-Open-Source-Firewall-and-Router-Platform))

1. **List some popular uses for pfSense.**
    - LAN/WAN router
    - Internet cafes
    - Wireless hotspot
    - VPN router
    - Firewall
    - DHCP/DNS server
    - Wireless access point
    - Transparent squid proxy server
    - Multi WAN router or load balancer
    - DNS blacklist
    - Port Forwarding / NAT (network address translation) 
2. **What are the hardware requirements for setting up a pfSense router?**
    - There are a number of embedded devices that are compatible with pfSense as well as repurposing an old PC for the job. However, with an old PC, you need at least two network cards installed.
3. **Where can you find support options for pfSense users?**
    - You can find support via the forums, mailing list, and IRC. BSD Perimeter, the company that founded pfSense also offers commercial support for users running pfSense in an enterprise environment. 
4. **How can you access the automatic configuration backup utility in pfSense?**
    - While the PC is ***not*** connected to any network cables, use the pfSense LiveCD to boot you into the pfSense console setup menu and select "install pfSense to the hard drive." Keep selecting the default options until complete. Once the installation is complete, remove the LiveMedia and reboot. When it boots pfSense for the first time, it'll ask if you want to configure VLANs, say no. Next it will prompt if you want to use the auto-detection configuration or to enter your LAN interface name. Follow the instructions to finish setup.
5. **Reflect on the importance of cultural awareness in the field of network security and administration. How might cultural differences influence decision-making and problem-solving when dealing with virtual routers and firewalls, like pfSense, in a global context?**
    - Time zone differences and language barriers may make configuring administrative points on a server network confusing. A unifying SOP and well defined policies will keep everyone on the same page.

## Additional Resources
[How to Install and Setup pfSense in VirtualBox](https://getlabsdone.com/how-to-install-pfsense-on-virtualbox/)

## Things I Want to Know More About
If we will ever be given an example for these multicultural questions because I'm starting to have difficulties on how to connect these with the material we're reading. Is there a case in which a multinational/crosscultural company had a security issue develope due to that culture clash? What did they do to fix address it?Is there a normalized SOP that companies use to deal with these problems? Some guidance would be welcome. 
