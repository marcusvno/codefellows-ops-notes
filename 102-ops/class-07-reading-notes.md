# Class 07 Reading Assignment
## Why It Matters

## SSH Protocol ([link](https://www.ssh.com/academy/ssh/protocol))
1. **What is the Secure Shell (SSH) Protocol?**
   - The Secure Shell protocol is a way to securely log into another computer through a secure connection with strong authentication. 
3. **What are the typical uses of the SSH protocol?**
   - Secure access for users and automated processes 
   - Remote commands
   - File transfers (interactive or automated)
   - Network infrastructure management
4. **How does the SSH protocol work?**
   - The SSH protocol works by establishing a connection by the SSH client with the SSH server. The client drives the connection setup and uses public key cryptography to verify itself to the SSH server. After the setup, the protocol uses strong symmetric encryption and hashing algorithms to ensure the connection, and data transfered through that connection, remains private.
5. **How is the data kept safe when transmitted between the SSH client and server?**
   - After a SSH client connects to a SSH server, the data sent between the two is encrypted as established in setup. The client and server agree on the symmetric encrtption algorithm to be used and generate an encryption key. The traffic is protected by strong encryption algorithms (such as AES which is also used by Wifi Networks) along with a hashing algoirthm (such as the Standard Hashing Algorithm or SHA-2)
6. **What is SFTP?**
  - SFTP is the Secture File Transfer Protocol and, as the name states, is used to transfer files over a secure connection.

## What is RDP? ([link](https://www.comparitech.com/net-admin/what-is-rdp/))
1. **What is Windows Remote Desktop Connection?**
   - Windows Remote Desktop Connection tool allows for remote users to use Windows to connect to another computer or server and have full access to the tools and software in it.
2. **What is RDP?**
   - The Remote Desktop Protocol is what powers the RDP Connection tool which allows for remote desktop connections to servers and other computers. Unlike SSH, RDP connections allow for full access to the computer's GUI and essentially allows the remote user access to the server's keyboard and mouse as if they were physically at the server.
3. **What is the RDP port number?**
   - Port 3389


## Things I Want to Know More About 
What are some of the more expressed differences between SFTP, SCP, and SSH? Are their functionalities exclusive to one another?
