# Network Topologies, Cabling, and Connectors

This write-up provides a comprehensive overview of network topologies, cabling, connectors, and related concepts, based on a detailed YouTube transcript. Readers will gain a solid understanding of different network architectures, cabling types, connectors, and troubleshooting techniques.

## Network Topologies

Network topology refers to the physical or logical layout of how devices are connected on a network. Several common topologies exist, each with advantages and disadvantages.

### Star Topology
- All computers connect to a central point (hub or switch)
- Data passes through the central point before reaching its destination
- Advantage: Failure of one computer or cable doesn't affect others
- Disadvantage: Single point of failure (central hub/switch failure brings down the entire network)

### Bus Topology
- Older technology, rarely used today
- Computers and devices connect to a single cable (coaxial)
- Computers connect using BNC (T-connectors)
- Advantage: Relatively cheap and easy to implement
- Disadvantage: Requires termination at both ends; any open connection (removed/added computer, loose terminators) causes signal reflection and disrupts data flow

### Ring Topology
- Computers connect in a closed loop
- Each computer has two neighbors for communication
- Data packets travel around the ring until reaching the destination
- Advantage: Easy to install and troubleshoot
- Disadvantage: Failure of one computer or cable disrupts data flow for the entire network

### Mesh Topology
- Each computer connects to every other computer
- High fault tolerance due to multiple connections
- Advantage: High redundancy; if one or more connections fail, communication can still occur
- Disadvantage: Expensive due to the large amount of cabling and network cards required. Primarily used in WANs like the internet

### Hybrid Topologies
- Combine different topologies (e.g., star-bus, star-ring)
- Offer benefits of multiple topologies. Common in businesses

### Point-to-Point Topology
- Two hosts directly connected with a single cable
- Simplest form of topology

### Client-Server Topology
- Clients connect to a central server for resources
- Commonly used in businesses for centralized resource management

### Point-to-Multipoint Topology
- Central base station connects to multiple wireless clients
- Clients don't communicate directly with each other
- Commonly used in wireless outdoor networks

### Peer-to-Peer Topology
- All clients share resources directly with each other
- No central server
- Simple to set up, commonly found in homes and small businesses

## Network Connectors

Several connectors are used in networking, each with specific applications:

### RJ-11
- 4-wire connector primarily for telephone equipment
- Used for modem connections in some network setups

### RJ-45
- 8-wire connector, the most common network connector
- Used for connecting computers to LANs

### RJ-48C
- Similar to RJ-45, but used with shielded twisted pair cable (STP)
- Primarily used with T1 lines

### UTP Coupler
- Connects two UTP cables with RJ-45 connectors
- Used to extend UTP cables

### BNC Connector
- Used on coaxial cables
- Used for analog and digital video and audio transmissions

### BNC Coupler
- Connects two coaxial cables with BNC connectors

### Fiber Coupler
- Joins two identical fiber optic connectors
- Not to be confused with fiber adapters (join different connector types)

### F-Type Connector
- Threaded connector used on coaxial cables, often by cable providers for cable modems

### USB Connector
- Commonly used on desktops and laptops; some wireless network cards use USB

### IEEE 1394 (Firewire)
- D-shaped connector, increasingly common for peripherals (digital cameras, printers)

### Fiber Optic Connectors
- MTRJ (Mechanical Transfer Registered Jack): Latched push-pull connection, small form factor
- ST (Straight Tip): Half-twist bayonet lock, commonly used with single-mode fiber
- LC (Local Connector): Similar to RJ-45 jack, commonly used between floors in buildings
- SC (Standard Connector): Push-pull connector, commonly used between floors in buildings

### Serial Connectors (DB-9, DB-25)
- Used with RS-232 serial data transmission

### UPC and APC Connectors
- UPC (Ultra Physical Contact): Light reflects directly back, causing signal loss
- APC (Angled Physical Contact): Angled connection reduces signal loss by reflecting light at an angle

## Plenum-Rated Cables

Plenum refers to spaces with open airflow in buildings (usually between ceilings). Cables in plenum spaces must be fire-resistant and produce no toxic fumes when burned.

## Ethernet over Other Media

Standards exist for transmitting Ethernet data over other media:

### Ethernet over HDMI (IEEE 1901-2013)
- HDMI 1.4 adds a channel for 100 Mbps Ethernet communication alongside video and audio

### Ethernet over Powerline (IEEE 1901)
- Uses building's electrical wiring for Ethernet networking. Requires powerline adapters

## Cable Standards

Ethernet cables are categorized by speed, type, and media:

- 10BASE-T: 10 Mbps, baseband transmission, twisted pair
- 10BASE-2 (Thinnet): 10 Mbps, coaxial cable, 200-meter maximum length
- 100BASE-T (Fast Ethernet): 100 Mbps, Category 5 UTP or higher, 100-meter maximum length
- 100BASE-FX: 100 Mbps, fiber-optic cable, 400 meters (half-duplex), 2 kilometers (full-duplex)
- 1000BASE-T (Gigabit Ethernet): 1000 Mbps, Category 5 UTP or higher, 100-meter maximum length
- 1000BASE-TX: 1000 Mbps, two unidirectional pairs (failed commercially)
- 10GBASE-T: 10 Gbps, shielded or unshielded twisted pair, 100 meters (Category 6A), 55 meters (Category 6)
- 10GBASE-SR (Short Range): 10 Gbps, multimode fiber, 300-meter maximum length
- 10GBASE-ER (Extended Reach): 10 Gbps, single-mode fiber, 40-kilometer maximum length
- 10GBASE-SW: 10 Gbps, same as 10GBASE-SR, used with SONET

## Firewalls

Firewalls prevent unauthorized access to a private network by filtering incoming internet traffic.

- Access Control Lists (ACLs): Rules defining permitted and denied network access
- Implicit Deny: Default rule where only explicitly allowed traffic is permitted
- Host-Based Firewalls: Software firewalls installed on individual computers
- Network-Based Firewalls: Hardware and software firewalls protecting entire networks
- Stateful Firewalls: Monitor connections and data streams, keeping records for dynamic protection
- Stateless Firewalls: Use ACLs to allow or deny traffic based on header information only
- Content Filtering: Filters data based on content (e.g., spam filtering)
- Signature Identification: Detects viruses and malware based on known behavior patterns
- Intrusion Detection/Prevention Systems (IDS/IPS): Hardware tools placed between the internet and firewall to detect and prevent attacks

## TIA/EIA 568A and 568B Wiring Standards

These standards define wiring order for twisted pair cables connected to RJ-45 connectors:

- 568A: White/green, green, white/orange, blue, white/blue, orange, white/brown, brown
- 568B: White/orange, orange, white/green, blue, white/blue, green, white/brown, brown

### Cable Types:
- Straight-through Cable: Both ends wired using the same standard (568A or 568B). Connects computers to hubs/switches/modems
- Crossover Cable: Ends wired using different standards (568A and 568B). Connects two similar devices (computers, hubs/switches)
- Rollover Cable: Ends wired completely opposite. Connects a computer/terminal to a router's console port
- Loopback Cable: For testing; connects pin 1 to pin 3, and pin 2 to pin 6

## Twisted Pair Cable Categories

Five categories of twisted pair cables:

- Category 3: 10 Mbps (old 10BASE-T)
- Category 5: 100 Mbps (100BASE-T & TX)
- Category 5e: >1000 Mbps (1000BASE-T)
- Category 6: 1000 Mbps (1000BASE-T), heavier duty than 5e, also used for 10GBASE-T (<100 meters)
- Category 6A: 10 Gbps (10GBASE-T, 100-meter maximum length)

## Other Cabling Types

- Unshielded Twisted Pair (UTP): Most common type, four pairs of unshielded wires
- Shielded Twisted Pair (STP): Similar to UTP, but with a foil shield for EMI protection
- Coaxial Cable: Used by cable providers for internet, earlier used as network backbones (RG-6 for long distances, RG-59 for short distances)
- Fiber Optic Cable: Uses light pulses for high-speed, long-distance data transmission (single-mode for long distances, multimode for short distances)

## Media Converters

Convert between different media types (fiber, Ethernet, coaxial) within a network.

## DOCSIS Cable Modems

Handle incoming and outgoing data signals (internet, video, voice); DOCSIS 3.1 supports 10 Gbps downstream, 1 Gbps upstream.

## Network Devices

- Hubs: Non-intelligent devices that broadcast data to all ports. Passive hubs don't require power, active hubs do
- Switches: Intelligent devices that learn MAC addresses and direct data to specific ports, reducing unnecessary traffic
- Multilayer Switches: Operate at layers 2 and 3 of the OSI model
- Content Switches: Operate at layers 4-7, perform load balancing and advanced filtering (expensive)
- Power over Ethernet (PoE): Provides power and data over the same Ethernet cable
- Spanning Tree Protocol (STP): Prevents broadcast traffic loops in networks with multiple switches
- Bridges: Divide networks into separate collision domains, filtering data based on MAC addresses
- Routers: Forward data between networks based on IP addresses
- Gateways: Connect networks with different protocols, changing data format but not content
- CSU/DSU (Channel Service Unit/Data Service Unit): Converts data between LANs and WANs
- Network Interface Card (NIC): Connects computers to networks, converting serial data to parallel data; has a unique MAC address
- Transceiver: Device with both transmitter and receiver
- Wireless Access Point: Wireless hub connecting wireless devices to a wired network
- Dial-Up Modem: Converts analog data from telephone lines to digital data for computers

## Wireless Technologies

- IEEE 802.11 Standards: A, B, G, N, and AC wireless standards (speeds, frequencies, and release years vary)
- Infrared (IRDA): Wireless technology using light rays (requires line of sight, doesn't work in direct sunlight)
- Bluetooth: Short-range radio for connecting and exchanging data between devices

## MAC Addresses

Unique 6-byte hexadecimal identifiers burned into every NIC by the manufacturer; first 3 bytes identify the manufacturer, last 3 bytes are unique to the device.

## OSI Model

Seven-layer model describing how data moves between computers:

1. Physical Layer: Defines network standards and physical characteristics (connectors, media, cables, etc.)
2. Data Link Layer: Sends data to the physical layer, encodes/decodes data, handles flow control and frame synchronization (MAC and LLC sublayers)
3. Network Layer: Routes data packets based on logical IP addresses, fragments/reassembles packets
4. Transport Layer: Transfers data between end users, resends packets without acknowledgment, ensures delivery
5. Session Layer: Controls communication dialogue, establishes/manages/terminates connections (traffic cop)
6. Presentation Layer: Converts data into a network-transmittable form (compression, encryption, decryption)
7. Application Layer: Manages communication between applications (email, HTTP, FTP)

## IP Addresses

Numeric identifiers for computers and devices on a network:

- IPv4: 32-bit numeric address (four octets separated by periods; 0-255 range per octet)
- IPv6: 128-bit hexadecimal address (eight groups of 16 bits separated by colons)

## Subnet Masks

Numbers resembling IP addresses, revealing how many bits in an IP address are used for the network; masking the network portion.

- Default subnet masks for Class A, B, and C IP addresses should be memorized

## IP Address Classes

- Class A: 1-126 (16 million hosts on 126 networks)
- Class B: 128-191 (65,000 hosts on 16,000 networks)
- Class C: 192-223 (254 hosts on 2 million networks)
- 127: Reserved for internal loopback functions

## Public vs. Private IP Addresses

- Public IP Addresses: Publicly registered on the internet, providing internet access
- Private IP Addresses (RFC 1918): Not publicly registered, used on local networks (homes, schools, businesses); translated to public IP addresses for internet access using NAT
  - Class A: 10.0.0.0 - 10.255.255.255
  - Class B: 172.16.0.0 - 172.31.255.255
  - Class C: 192.168.0.0 - 192.168.255.255

## Subnetting

Breaking down a large network into smaller, more manageable subnets; done by changing the default subnet mask, borrowing bits from the host portion. The formula 2n - 2 (where n is the number of borrowed bits) determines the number of subnets created.

## IP Address Assignment

- Dynamic IP: Automatic assignment from a DHCP server (assigns IP address, subnet mask, default gateway, DNS server)
- Static IP: Manual IP address assignment (permanent, no DHCP server needed)
- APIPA (Automatic Private IP Addressing): Self-assigned IP addresses (169.254.0.0 network) if a DHCP server is unavailable (Windows 98 and later)

## DHCP Servers and Scopes

DHCP servers assign IP addresses from a scope (range of consecutive IP addresses). Reservations can be created to ensure specific devices always receive the same IP address. IP addresses are leased for a specific duration (e.g., one day).

## DHCP Relays

Relay DHCP broadcasts between subnets so computers outside the DHCP server's subnet can receive IP addresses.

## TCP/IP Protocols

### Core Transport Protocols
* **TCP (Transmission Control Protocol)**
  * Connection-oriented protocol
  * Uses three-way handshake (SYN, ACK, ACK)
  * Guarantees data delivery

* **UDP (User Datagram Protocol)**
  * Connectionless protocol
  * No delivery guarantee (fire-and-forget)
  * Faster than TCP

### File Transfer Protocols
* **FTP (File Transfer Protocol)**
  * Standard protocol for file transfer
  * Connection-oriented using TCP
  * Basic file upload/download capabilities

* **TFTP (Trivial File Transfer Protocol)**
  * Simple file transfer for same network
  * Connectionless using UDP
  * No security features

* **SFTP (Secure FTP)**
  * Enhanced FTP with SSH encryption
  * Secure file transfer solution

### Email Protocols
* **SMTP (Simple Mail Transfer Protocol)**
  * Email sending protocol
  * Uses TCP for reliable delivery

* **POP3 (Post Office Protocol version 3)**
  * Email receiving protocol
  * Downloads emails to local computer
  * No synchronization capabilities

* **IMAP4 (Internet Message Access Protocol version 4)**
  * Receives emails
  * Allows access and management on the server
  * Syncs emails and folders

* **HTTP (Hypertext Transfer Protocol)**
  * Views web pages
  * Sends information in clear text

* **HTTPS (Secure HTTP)**
  * HTTP with SSL/TLS encryption
  * Used for secure web pages

* **Telnet**
  * Terminal emulation for accessing remote servers
  * Not secure, sends commands in clear text

* **SSH (Secure Shell)**
  * Secure alternative to Telnet
  * Encrypts data during transfer

* **ARP (Address Resolution Protocol)**
  * Resolves IP addresses to MAC addresses

* **RARP (Reverse ARP)**
  * Resolves MAC addresses to IP addresses

* **NTP (Network Time Protocol)**
  * Synchronizes computer clocks with master clocks

* **SCP (Secure Copy Protocol)**
  * Uses SSH for secure file transfer

* **SNMP (Simple Network Management Protocol)**
  * Used for network management
  * Collects data from network devices

### Ports

Logical connections used by programs to exchange information; numbered 0-65535. Key ports to know for the Network+ exam are listed.

### DNS and WINS

* **DNS (Domain Name System)**
  * Resolves domain names to IP addresses

* **WINS (Windows Internet Name Service)**
  * Resolves NetBIOS names (computer names) to IP addresses

### Network Address Translation (NAT)

Translates IP addresses between private and public networks.

* **PAT (Port Address Translation)**
  * Translates IP addresses based on port numbers

* **SNAT (Static NAT)**
  * Permanently links a public IP address with a private IP address

### Proxy Servers

Retrieve web pages on behalf of users, store them in a cache for faster retrieval; improve speed, save bandwidth, provide security by reporting web page access.

### Remote Desktop Protocol (RDP)

Microsoft technology for accessing remote computer desktops.

### Network Access Methods

* **CSMA/CD (Carrier Sense Multiple Access with Collision Detection)**
  * Used on Ethernet networks
  * Computers sense if the wire is idle before sending data
  * Collisions are detected and data retransmission occurs

* **CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance)**
  * Used in wireless networks
  * Sends a small packet to check if the channel is clear before sending data

### Unicast, Multicast, and Broadcast

* **Broadcast**
  * Single transmitter, multiple receivers

* **Unicast**
  * Single transmitter, single receiver

* **Multicast**
  * Single transmitter, multiple receivers simultaneously

### Routing Concepts and Protocols

* **Loopback Interface**
  * Virtual interface on a router for testing and administration purposes

* **Routing Table**
  * Contains rules showing data packet paths to destinations

* **Routing Protocols**
  * Collect network information and map out best paths for data packets

* **Distance Vector Protocols**
  * Consider distance to destination based on hops (RIP, RIPv2, BGP)

* **Link State Protocols**
  * Routers share information and independently map paths (OSPF, IS-IS)

* **Hybrid Protocols**
  * Combine distance vector and link state (EIGRP)

### Real-Time Protocols

* **SIP (Session Initiation Protocol)**
  * Establishes communication sessions (VoIP, instant messaging, conferencing)

* **RTP (Real-Time Transport Protocol)**
  * Transports real-time data (audio, video)
  * Often used over UDP
  * Used with RTCP for quality monitoring

### Packet Switching vs. Circuit Switching

* **Packet Switching**
  * Data packets take different routes
  * Reassembled at the destination
  * Connectionless; internet uses this

* **Circuit Switching**
  * Data packets take the same dedicated route
  * Connection-oriented; telephone lines

### Internet Connection Technologies

* **ISDN (Integrated Services Digital Network)**
  * Digital transmission over telephone lines (128 Kbps)

* **T1 Lines**
  * Dedicated connections
  * 1.544 Mbps, 24 channels at 64 Kbps each

* **T3 Lines**
  * High-speed connections
  * 43 Mbps, 672 channels at 64 Kbps each

* **E1 Lines (European T1)**
  * 2 Mbps, 32 channels at 64 Kbps each

* **E3 Lines (European T3)**
  * 34 Mbps

* **OCx (Optical Carrier)**
  * SONET fiber-optic technology
  * Speeds calculated as multiples of 51.84 Mbps

* **DSL (Digital Subscriber Line)**
  * Broadband data over telephone lines
  * Types: ADSL, SDSL, VDSL

* **Broadband Cable**
  * High-speed internet over coaxial cable

* **POTS/PSTN**
  * Traditional telephone lines

* **Satellite Communication**
  * Expensive
  * Used where other services are unavailable

* **Mobile Hotspots**
  * Portable devices using cellular networks for internet access

* **WiMAX**
  * Wireless network covering large areas

* **Metro Ethernet**
  * Metropolitan area network based on Ethernet standards

### Network Types

* **PAN (Personal Area Network)**
  * Small network for connecting personal devices
  * Example: Bluetooth

* **LAN (Local Area Network)**
  * Network within a building or close proximity

* **MAN (Metropolitan Area Network)**
  * Network spanning multiple buildings in a city

* **WAN (Wide Area Network)**
  * Largest network type
  * Example: Internet

### SCADA and Industrial Control Systems (ICS)

Software for controlling and monitoring equipment in industrial facilities; communicates with sensors and systems in real time.

### Cellular Network Technologies

* **GSM (Global System for Mobiles)**
  * Widely used radio system

* **CDMA (Code Division Multiple Access)**
  * Alternative radio technology used by some carriers

* **4G LTE (Long Term Evolution)**
  * Fastest current wireless communication speed

* **3G**
  * Speeds from 384 Kbps to 2 Mbps

* **EDGE**
  * Very slow technology

### Remote Access Service (RAS)

Enables remote connection to computers over a dial-up connection.

### Remote Access Protocols

* **SLIP (Serial Line Internet Protocol)**
  * Insecure protocol for communication over serial connections
  * Rarely used

* **PPP (Point-to-Point Protocol)**
  * Secure protocol replacing SLIP
  * Used by ISPs for dial-up connections

* **PPPoE (PPP over Ethernet)**
  * Uses PPP over Ethernet connections
  * For DSL, broadband, wireless

* **PPTP (Point-to-Point Tunneling Protocol)**
  * Default protocol for VPNs

* **GRE (Generic Route Encapsulation)**
  * Creates VPN tunnels with PPTP

### VPNs (Virtual Private Networks)

Private networks using public networks for remote connections; data is encrypted during transfer.

* **VPN Concentrator**
  * Device managing and creating VPN connections

* **VPN Connection Types**
  * Site-to-Site: Connects two offices
  * Host-to-Site: Connects home computer to office
  * Host-to-Host: Connects two computers directly

### Authentication Protocols

* **PAP (Password Authentication Protocol)**
  * Simple but insecure
  * Sends data in clear text

* **CHAP (Challenge Handshake Authentication Protocol)**
  * Encrypts usernames and passwords

* **MS-CHAP**
  * Microsoft's version of CHAP
  * MS-CHAP 2 offers mutual authentication

* **RADIUS**
  * Centralized authentication server

* **Kerberos**
  * Uses tickets for authentication

* **EAP (Extensible Authentication Protocol)**
  * Extension to PPP
  * Supports various authentication methods

### Network Troubleshooting Tools

* **Wire Crimper**
  * Creates custom-length network cables

* **Punch Down Tool**
  * Connects wires to punch-down blocks

* **Media Tester**
  * Tests network cables for proper wiring

* **Cable Stripper**
  * Removes plastic shielding from cables

* **TDR (Time-Domain Reflectometer)**
  * Tests copper cables for problems

* **OTDR (Optical Time-Domain Reflectometer)**
  * Tests fiber optic cables

* **Multimeter**
  * Tests electrical circuits

* **Butt Set**
  * Tests and monitors telephone lines

* **Voltage Event Recorder**
  * Collects data on power quality

* **Tone Generator**
  * Locates cables

* **Protocol Analyzer**
  * Troubleshoots and analyzes network traffic
  * Example: Wireshark

### Viruses and Antivirus Software

Harmful programs altering computer operation; antivirus software is crucial for protection and regular scanning is essential.

### ESD (Electrostatic Discharge) Prevention

ESD can damage computer components; prevention includes using ESD wrist straps and mats.

### Proper Equipment Disposal

Computer equipment contains harmful chemicals; proper disposal methods are outlined in MSDS from manufacturers or the EPA.

### Safety Precautions

* Turn off power and unplug cables before hardware repair
* Remove jewelry
* Know fire extinguisher location and use (Class C for electrical fires)
* Manage cables to prevent tripping hazards
* Lift heavy objects properly using legs, not back

### Virtualization

Consolidating physical servers and their applications onto a single physical server in a virtual environment; saves money on hardware, storage, maintenance
