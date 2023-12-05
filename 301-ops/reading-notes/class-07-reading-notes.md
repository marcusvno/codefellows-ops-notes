# Class 07X Reading Assignment

## Web Server Deployment

- What is NGINX ([article](https://www.nginx.com/resources/glossary/nginx/))

## Questions

1. **What are some common use cases for NGINX?**
   - Web serving, reverse proxying, caching, load balancing, media streaming and can also function as a proxy server for email services like IMAP, POP3, and SMTP.
2. **How does NGINX handle tasks that could slow down the web server?**
   - NGINX was originally made to tackle the "C10k" problem -- the difficulty for servers to handle large numbers (10k) of connections concurrently (c) -- and continues to handle slowdown by acting as a load balancer to manage incoming traffic and distribute it to slower upstream servers.
3. **Describe, as if to a non-technical friend how to actually pronounce “NGINX”, and why an org might chooose to use it.**
    - "NGINX" is pronounced "engine-x". An org might choose it as a multifaceted solution for their webserver when they value high speed (NGINX is one of the fastest web servers around), load balancing, and have a high volume of concurrent users.

## Additional Resources

- Network Architectures ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-architectures-n10-008/))
- Network Devices ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/networking-devices-n10-008/))
- Network Connectors ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-connectors-2/))
- Ethernet Standards ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/ethernet-standards-n10-008/))

## Things I Want to Know More About

Whats the difference between APACHE and NGINX? And if NGINX is open-source, why is there an pricing page? Do they offer additional support to for enterprise clients? Could a business decide to handle all NGINX fixes/etc internally and not pay NGINX?
