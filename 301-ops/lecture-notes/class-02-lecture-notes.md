# Network Enumberation

Using scanning tools to map out the structure of an unknown network as part of a pentest, or general site survey.

## Port and Protocols

- **port number:** a number assigned to uniquely identify a connection endpoint and to direct data to a specific service.
- **network protocol:** an established set of rules that determine how data is transmitted between different devices in the same network
- **network service:** an application running at Layer 7 (application layer), providing data storage, manipulation, presentation, communication, or other capability according to a _protocol._

Ports _only_ exist as a number attached to incoming and outgoing packets. - Logical Ports exist at Layer 4 (transport) and are **_not the same_** as Layer 1 Physical Ports.

Each port number is associated with a protocol.

### Common Ports and Protocols

| **Protocol** | **Port Number** |
| ------------ | --------------- |
| FTP          | 20-21           |
| SSH          | 22              |
| SFTP         | 22              |
| TELNET       | 23              |
| SMTP         | 25              |
| DNS          | 53              |
| DHCP         | 67-68           |
| HTTP         | 80              |
| NTP          | 123             |
| HTTPS        | 443             |
| SMB          | 445             |
| RDP          | 3389            |

### Port Scanning

A port scanner reveals open ports on a target host by sending specially crafted packets and waiting for a response.

- The `netstat` command lets you check port states on the _local_ host.
- `netstat -an` displays all connections in numerical format.
- `netstat -r` displays the routing table
