# Class 02 Reading Assignment

## Network Scanning with nmap ([link](https://www.varonis.com/blog/port-scanning-techniques))

- Common Ports ([link](https://www.professormesser.com/network-plus/n10-008/n10-008-video/common-ports-n10-008/))

1. **What is a port? Describe it with an analogy that would help a family member understand.**
   - A port is a virtual location where networking communication starts and ends. Like the door to a business, it can be open and accepting new customers, closed to any customer, or blocked off.
2. **What does a port scanner send to a port to check the current status?**
   - A port scanner sends a packet of data, sometimes made for a specific type of request, such as a ICMP echo request (also known as a ping). The type of port scanning done depends on the type and content of the packet.
3. **When a port scanner sends a request to connect, what are the three possible responses? Describe them.** -**Open, Accepted:** The computer (or server) responds, indicating readiness to provide the requested service. -**Closed, Not Listening:** The computer responds, indicating the port is currently in use and unavailable. -**Filtered, Dropped, Blocked:** The computer doesn’t respond at all.
4. **What is the difference between TCP and UDP?**
   - While they are common protocols in IP networks, **TCP** (Tranmission Control Protocol) has redudancy and error-checking, it sends each packet in order, verifies, and has a 3-way handshake to confirm each packet was sent successfully. **UDP** (User Datagram Protocol) is faster because it isn't does error check, this is useful for when you don't need ever single packet to be arrive perfectly and some data loss is acceptable; such as in video games and streaming video. UDP does not form a connection and just sends the data direct.

## Additional Resources

- The nmap official docs ([link](https://nmap.org/book/man.html))
- nmap cheatsheet ([link](https://cdn.comparitech.com/wp-content/uploads/2019/06/Nmap-Cheat-Sheet.pdf))
  ![nmap cheatsheet](https://cdn.comparitech.com/wp-content/uploads/2019/06/Nmap-Cheat-Sheet-1.webp)

**Extras:**

- What is a Cyber Kill Chain? ([link](https://www.varonis.com/blog/cyber-kill-chain))
- Netcat ([another scanning tool](https://netcat.sourceforge.net/))

## Things I Want to Know More About

How do you to use nmap and other tools with scripting to automate finding vulnerabilities?
