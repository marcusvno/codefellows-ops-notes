# Class 13 Reading Assignment

## Reconstructing a Cloud Attack with Splunk

- What is a reverse proxy? ([article](https://www.cloudflare.com/learning/cdn/glossary/reverse-proxy/))

## Questions

1. **What are the benefits of a forward proxy?**
    - A forward proxy stands between a user endpoint and the internet. This allows it to act as a middleman which can be used for a few different reasons:
      - **To avoid state or institutional browsing restrictions** - Some governments, schools, and other organizations use firewalls to give their users access to a limited version of the Internet. A forward proxy can be used to get around these restrictions, as they let the user connect to the proxy rather than directly to the sites they are visiting.
      - **To block access to certain content** - Conversely, proxies can also be set to block a group of users from access certain sites. For example, a school network might be configured to connect to the web through a proxy which enables content filtering rules, refusing to forward responses from social media sites.
      - **To protect their identity online** - In some cases, regular Internet uses simply desire increased anonymity online, but in other cases, Internet users live in places where the government impose serious consequences to political dissidents. Criticizing the government in web forums or social media can lead to fines or imprisonment for these users. If one of these dissidents uses a forward proxy to connect to a website where they post politically sensitive comments, the IP address used to post the comments will be harder to trace back to the dissident. Only the IP address of the proxy server will be visible.

<img src="https://cf-assets.www.cloudflare.com/slt3lc6tev37/2MZmHGnCdYbQBIsZ4V11C6/25b48def8b56b63f7527d6ad65829676/forward_proxy_flow.png" width=600/>

2. **Explain the differences between a forward and a reverse proxy?**
    - A _forward proxy_ sits in front of the clients before while a _reverse proxy_ sits in front of the web servers. When a client sends requests to a server of a website, a _reverse proxy_ intercepts those requests at the **network edge**. Then the _reverse proxy_ sends those requests to (and receive responses from) server.
    - The difference is subtle:
      - A **forward proxy** sits in front of a client and ensures that no server ever communicates directly with a specific client.
      - A **reverse proxy** sets in front of a server and ensures that no client ever communicates directly with that server.

<img src="https://cf-assets.www.cloudflare.com/slt3lc6tev37/3msJRtqxDysQslvrKvEf8x/f7f54c9a2cad3e4586f58e8e0e305389/reverse_proxy_flow.png" width=600/>

3. **Explain to your manager why your organization might benefit from implementing a reverse proxy?**
    - A reverse proxy can be used for many benefits:
      - **Load balancing** - A popular website gets millions of users every day and may not be able to handle all incoming traffic with a single server. Instead, the site can distribute the load among a pool of servers, all handling requests for the same site. In this case, a reverse proxy can be used for load balancing which will distribute the incoming traffic evenly among the different servers to prevent any single server from being overloaded.
        - This can be extended to **global load balancing**, where traffic is directed to servers located geographically closest to the clients.
      - **Protection from attacks** - A reverse proxy obfuscates a site's IP address. This makes it much harder for attackers to leverage a targeted attack, such as a DDoS attack, against the servers.
      - **Caching** - A reverse proxy can also _cache_ content, resulting in faster performance.
      - **SSL encryption** - Encrypting and decrypting SSL (or TLS) communications for each client can be computationally expensive for an origin server. A reverse proxy can be configured to do all the decryption of incoming requests and encrypt all outgoing responses, freeing up resources of the server.

## Additional Resources

- A Conversation About REST API ([article](https://gist.github.com/brookr/5977550))
- Operationalize Ransomware Detections Quickly and Easily with Splunk ([article](https://www.splunk.com/en_us/blog/industries/operationalize-ransomware-detections-quickly-and-easily-with-splunk.html))
