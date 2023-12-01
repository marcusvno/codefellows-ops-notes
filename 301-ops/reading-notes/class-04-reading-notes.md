# Class 04 Reading Assignment

## Routing

VirtualBox Network Settings Guide ([article](https://www.nakivo.com/blog/virtualbox-network-setting-guide/))

1. **Which network mode in VirtualBox can be used to emulate unplugging the Ethernet cable from the network?**
   - Not attached.
2. **Which network mode would be best if you wanted to run a server on a VM that could be fully accessible from your physical local area network?**
   - Bridged Mode.
3. **What are the three options of promiscuous mode and what does each do?**
   - **Deny** - Any traffic that is not intended to the virtual network adapter of the VM is hidden from the VM. This option is set by default.
   - **Allow VMs** - All traffic is hidden from the VM network adapter except the traffic transmitted to and from other VMs.
   - **Allow All** - There are no restrictions in this mode. A VM network adapter can see all incoming and outgoing traffic.
4. **What is Port Forwarding?**
   - Port forwarding is a process of intercepting traffic addressed to the appropriate IP address and port in addition to redirecting that traffic to a different IP address and/or port.

## Additional Resources

- Network Topologies ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-topologies-5/))
- Routing Technologies ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/routing-technologies-n10-008/))
- Dynamic Routing ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/n10-008-dynamic-routing/))
- Network Switching Overview ([video](https://www.professormesser.com/network-plus/n10-008/n10-008-video/network-switching-overview-n10-008/))

Getting Started with Cisco Packet Tracer [mini-course](https://skillsforall.com/course/getting-started-cisco-packet-tracer?courseLang=en-US)
Packet Tracer - BGP Configuration [mini-tutorial](https://www.packettracernetwork.com/tutorials/bgp.html#:~:text=BGP%20in%20Packet%20Tracer,network%20policies%20and%2For%20rulesets.)
Cisco IOS IP Routing: RIP Command Reference [documentation](https://www.cisco.com/c/en/us/td/docs/ios/iproute_rip/command/reference/irr_book/irr_rip.html)
Static Routing Configuration [mini-tutorial](https://www.computernetworkingnotes.com/ccna-study-guide/static-routing-configuration-guide-with-examples.html)

## Things I Want to Know More About

How does other VM software deal with these same issues? Is it slight differences but ultimately the same approach or are they wildy different?
