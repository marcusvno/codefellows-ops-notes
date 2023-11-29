# Class 01 Reading Assignment

## Network Traffic Analysis
- Layers of OSI Model ([link](https://www.geeksforgeeks.org/open-systems-interconnection-model-osi/))
- What is Wireshark and How to Use It ([link](https://www.comptia.org/content/articles/what-is-wireshark-and-how-to-use-it))

## OSI model
1. **What does “OSI” stand for?**
    - Open System Interconnections
2. **List the 7 layers of the OSI model and what each one is responsible for.**
    1. *Physical Layer* - The actual physical connection between devices (ethernet cable). 
    2. *Data Link* - Focuses on the physical addressing of the transmission
    3. *Network* - Works for the transmission of the data from one host to another through packet routing and reassembly of data.
    4. *Transport* - It is responsible for the End to End Delivery of the complete message.
    5. *Session* - This layer is responsible for the establishment of connection, maintenance of sessions, and authentication, and also ensures security.
    6. *Presentation* - The presentation layer is also called the Translation layer. The data from the application layer is extracted here and manipulated as per the required format to transmit over the network. 
    7. *Application* - It is the layer in which protocols and rules are in place to determine how the user should interact with data sent or received.
3. **Distinguish which layers are the “hardware layers”, and which layers are the “software layers”. What does that even mean?**
    - Physical and Data link layers are linked to the physical hardware necesssary to network devices and therefore are hardware layers. The other layers are part of the transmission, encapsulation, translation, and production of data, which all happen in the software of a device.
4. **How can the OSI model be used in troubleshooting?**
    - OSI model can be used in troubleshooting by allowing the technician to isolate and test each layer for problem causes and assisting with root cause analysis. 

## Wireshark
1. **What is Wireshark?**
    - Wireshark is a network protocol analyzer, an application that captures packets from network connections, such as between your computer and the internet.
2. **What is a packet?**
    - A packet is a discrete unit of data in a typical Ethernet network.
3. **What 3 high-level things does Wireshark accomplish? How could these be used for nefarious purposes? For benevolent purposes?**
    - Packet Capture: It listens to network connections in real-time and captures streams of traffic, potentially including tens of thousands of packets​​.
    - Filtering: Wireshark can filter the captured data, allowing you to obtain only the information you need​​.
    - Visualization: It allows you to delve into the details of network packets and visualize entire conversations and network streams​​.

    - These activities can be used for benevolent purposes, such as monitoring and troubleshooting a network, but also for nefarious purposes such as trying to intercept traffic on a network or try and find a way in for unauthorized surveillance and access.

## Additional Resources

| **Resource** | **URL** |
|-|-|
|Wireshark website|https://www.wireshark.org/|
|Wireshark sample packet captures|https://wiki.wireshark.org/SampleCaptures|
|Packet captures galore, with an emphasis on security|http://www.malware-traffic-analysis.net/|
|Packet captures by protocol|https://www.netresec.com/?page=pcapfiles|
|Additional packet captures|http://tcpreplay.appneta.com/wiki/captures.html|
|Wireshark cheat sheet 1|http://packetlife.net/media/library/13/Wireshark_Display_Filters.pdf|
|Wireshark cheat sheet 2|https://www.comparitech.com/net-admin/wireshark-cheat-sheet/|
|How to use Wireshark to Capture and Filter Packets| https://www.howtogeek.com/104278/how-to-use-wireshark-to-capture-filter-and-inspect-packets/ |
![wireshark-cheat-sheet](https://cdn.comparitech.com/wp-content/uploads/2019/06/Wireshark-Cheat-Sheet-1.jpg.webp)


## Things I Want to Know More About
How do I use Wireshark for nefarious purposes? 
