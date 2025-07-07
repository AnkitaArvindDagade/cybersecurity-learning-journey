#  Network Fundamentals

This module introduced me to the basics of how devices communicate over networks, how IP addressing works, and common network topologies.

---

##  What is Networking?

- **Networking** simply means connecting things (devices, systems) together.
- The **Internet** is one big global network that consists of many smaller networks.
  - **Private Networks** = Small, internal networks (e.g., home or office)
  - **Public Networks** = Networks that connect multiple smaller networks

---

##  IP Addressing

###  IP (Internet Protocol) Address:
- Used to **identify a device on a network** for a period of time.
- Consists of **4 octets** in IPv4 (e.g., `192.168.1.1`)

###  IPv4 vs IPv6
- **IPv4** allows `2^32` unique addresses.
- **IPv6** allows `2^128` unique addresses (much more scalable).

**Examples:**
- IPv4: `86.157.52.21`
- IPv6: `2000:12c4:1531:c500:425f:cc61:2361:f64d`

---

##  MAC Address (Media Access Control)

- A **12-character hexadecimal** address that identifies hardware on a network.
- Example: `a4:c3:f0:85:ac:2d`

---

##  Tools: Ping (ICMP)

- `ping` is a network tool that uses ICMP (Internet Control Message Protocol) packets.
- Used to test the **connectivity and performance** between devices.

##  Introduction to LAN

**LAN (Local Area Network)** connects devices within a small geographic area like a home or office.

###  Common LAN Topologies

- **Star Topology** – All devices connect to a central hub.
- **Bus Topology** – Devices share a single communication line.
- **Ring Topology** – Each device connects to two others in a circular fashion.

---

##  Networking Devices

###  Switch

- Connects multiple devices using Ethernet.
- Helps in forwarding data within LAN.

###  Router

- Connects different networks and **routes data** between them.
- Useful when devices are connected through multiple paths.

---

##  Subnetting

- **Subnetting** = Dividing a network into smaller, manageable sections (subnets).
- Helps organize and optimize network traffic.

###  Key Identifiers

- **Network Address** – Identifies the network.  
  _Example: `192.168.1.0`_

- **Host Address** – Identifies a specific device.  
  _Example: `192.168.1.100`_

- **Default Gateway** – Device used to send data outside the network.  
  _Example: `192.168.1.1` or `.254`_

---

##  ARP (Address Resolution Protocol)

- ARP allows devices to **discover each other's MAC addresses** on a network.
- Two message types:
  1. ARP Request
  2. ARP Reply

---

##  DHCP (Dynamic Host Configuration Protocol)

- Automatically assigns IP addresses to devices on a network.
- Saves time compared to manual configuration.

###  DHCP Process

1. Discover  
2. Offer  
3. Request  
4. Acknowledge

---

##  OSI Model (Open Systems Interconnection)

The OSI model is a **7-layer framework** for understanding how network communication works.

1. **Physical** – Hardware transmission (cables, devices)  
2. **Data Link** – MAC addressing and switching  
3. **Network** – IP addressing, routing  
4. **Transport** – TCP/UDP protocols  
5. **Session** – Connection management  
6. **Presentation** – Encryption and data format conversion  
7. **Application** – End-user interaction (browsers, apps)



