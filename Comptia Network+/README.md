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

- TCP (Transmission Control Protocol): Connection-oriented, uses a three-way handshake (SYN, ACK, ACK) to establish sessions, guarantees data delivery
- UDP (User Datagram Protocol): Connectionless, doesn't guarantee delivery (fire-and-forget), faster than TCP
- FTP (File Transfer Protocol): Standard protocol for uploading and downloading files;
