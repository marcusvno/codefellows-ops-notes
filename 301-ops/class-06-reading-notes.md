# Class 06 Reading Assignment

## Network Address Translation ([article](https://www.geeksforgeeks.org/network-address-translation-nat/))

1. **What is the main purpose for implementing NAT on a network?**
   - To allow multiple devices access to the Internet through a single public address. To accomplish this, the translation of private IP address to public IP address is required.
2. **At what layer of the OSI model does NAT happen?**
   - Network.
3. **What happens to packets when NAT runs out of addresses in the pool of available IPs?**
   - If the NAT runs out of addresses, then packets will be dropped and the ICMP host unreachable packet is sent to the destination.
4. **What disadvantage does using NAT pose for routers?**
   - Translation results in delays due to switching paths.
   - Certain applicatiosn will not function while NAT is enabled.
   - Complicates tunneling protocols (such as IPSec)

## Additional Resources

- Network Address Translation (NAT) ([video](https://www.professormesser.com/network-plus/n10-007/network-address-translation-3/))
- Common Network Types ([video](https://www.professormesser.com/network-plus/n10-007/common-network-types/))
- IPv4 and IPv6 Addressing ([video](https://www.professormesser.com/network-plus/n10-007/ipv4-and-ipv6-addressing/))

## Things I Want to Know More About

Does a company purchase the entirety of a /24 block? How it does it work for the internet I use at home?
