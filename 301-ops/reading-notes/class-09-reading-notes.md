# Class 09 Reading Assignment

## Traffic Mirroring

How to capture network traffic? SPAN vs TAP ([article](https://accedian.com/blog/capture-network-traffic-span-vs-tap/))

1. **What are the differences between SPAN and TAP?**
   - SPAN (port mirroring) is software based and copies traffic from one port to another using a switch. It's less expensive than TAP but may drop packets and negatively impact performance.
   - TAP is hardware-based dedicated device to copy and mointor traffic. Does not impact performance and has full visibility onto the traffic, including errors and congestion.
2. **What types of network devices can support network traffic mirroring?**
   - Network traffic mirroring can be supported by devices like switches (for SPAN) and requires hardware devices like TAP for direct traffic capture.
3. **How can network traffic mirroring be used for network security?**
   - Traffic mirroring helps in monitoring and analyzing network traffic for anomalies, intrusions, and performance issues.
4. **Are there any legal or ethical considerations when using network traffic mirroring?**
   - Legal and ethical considerations include ensuring compliance with data protection laws and respecting privacy rights when capturing and analyzing network traffic.

## Additional Resources

Logs and Monitoring ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/logs-and-monitoring-n10-008/))

## Things I Want to Know More About

What about Wireshark?
