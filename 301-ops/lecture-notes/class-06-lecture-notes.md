# Class 06 Lecture

## Access Models

## Geographical Network Types

Where can we access this network from?

![networks](https://codefellows.github.io/ops-301-guide/curriculum/class-06/slides/assets/06_02.png)

- The **Internet** is a **Wide Area Network (WAN)** that spans the Earth.
- **Radio Area Network (RAN)** resides between a device such as mobile phone, computer, and any remotely controlled devices and provides connection with its core network. (Legacy term)
- A **Metropolitan Area Network (MAN)** spans across several LANs over a city or metro area. (Legacy term)
- A network infrastruction covering the school, university, or coprorate premises (campus) can be classified as a **Campus Area Network (CAN)**
- A **Personal Area Network (PAN)** is inteded for personal use within a range of under 10 meaters with usually wireless device.
- **Body Area Networks (BAN)** include body area of wearable devices like smartwatches, fitness bands, biometric RFID implants, and medical devices placed inside the body like pacemakers.
- **Near-me Network (NAN)** encompasses networked devices not necessarily connected on the same LAN but are in close proximity (two friends on Twitter on the same living room)

## Addressing: IPv4 vs. IPv6

**Internet protocol version 4 (IPv4)** and **Internet Protocol version 6 (IPv6)** are two different addressing schemes used to identify and route data packets in computer networks.

![IP comparison](https://codefellows.github.io/ops-301-guide/curriculum/class-06/slides/assets/06_06.png)

### Address Exhaustion

- **IPv4** has a large but **exhaustible** number of addresses
  - Not enough addresses for every device
  - Addresses must be reused and masked
- **IPv6** has a sufficiently large name-space that we will never run out.
- **Subnetting** and **Network Address Translation** are also attempts to address the limited number of available IPv4.

- In addition to an increased address-space, **IPv6 offers several improvements over IPv4:**
  - **Better support** for end-to-end connectivity
  - Simplified network management
  - Built-in Security features
    - Fully **integrated with IPsec** from the start (natively supports AH and ESP)
    - Improved Routing Security
    - Simplified NAT
      -Support for mobile networks and autoconfiguration of devices.
  - However! IPv6 and IPv4 operate at the same speed.

## Network Address Translation

**_Network address translation (NAT):_** altering the IP address is a packet header in transit so that the destination interprets the packet as coming from the new IP instead of actual originating IP.

![nat trans](https://codefellows.github.io/ops-301-guide/curriculum/class-06/slides/assets/06_03.png)

- **Network address translation (NAT)** is performed by routers (Layer 3 : Network) so that the destination interprets the packet as coming from the translated IP instead of the actual orginating IP.

- This allows us to **re-use the same address-spaces** (192.168.x.x. and 10.x.x.x for exampel) over and over without creating address conflcits.

- **NAT** has played a vital role globally in delaying **IPv4 address exhaustion**, reducing the need to transition at large scale to IPv6.
