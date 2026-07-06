# OSI Model (CompTIA Network+)

The OSI model describes how data moves across a network in 7 layers, from physical signals to user applications.

---

# OSI Layers (Top → Bottom)

7. Application – HTTP, HTTPS, DNS, SMTP  
6. Presentation – encryption, formatting, compression  
5. Session – session management  
4. Transport – TCP/UDP, ports  
3. Network – IP addressing, routing  
2. Data Link – MAC addresses, switching  
1. Physical – cables, signals, bits  

---

# Memory Aid

**Please Do Not Throw Sausage Pizza Away**

(P → A = 1 → 7)

---

# Layer 1 – Physical

## Overview
The Physical layer deals with raw transmission of bits over a medium.

It defines:
- Electrical signals
- Light (fiber optics)
- Radio waves (wireless)

No addressing, no protocols — just signal transmission.

---

## PDU
- Bits (1s and 0s)

---

## Core Functions
- Transmits raw electrical/optical/radio signals
- Defines cables, connectors, and physical layout
- Determines how bits are encoded into signals

---

## Media Types

### Copper Cabling
- Twisted pair (UTP/STP)
  - Cat5e, Cat6, Cat6a, Cat8
- Coaxial (RG-6 for cable internet)

### Fiber Optic
- Single-mode: long distance, laser, low attenuation
- Multimode: short distance, LED, cheaper

### Wireless
- Wi-Fi (2.4 GHz, 5 GHz, 6 GHz)
- Cellular
- Satellite

---

## Common Issues (Troubleshooting Layer 1)
- No link lights / link down
- Damaged or incorrect cable type
- Bad termination or crimping
- Excessive cable length (attenuation)
- Duplex/speed mismatch
- Faulty port or transceiver

---

## Tools
- Cable tester (continuity, wiring map)
- Loopback plug (tests NIC/port)
- OTDR (fiber diagnostics)
- Multimeter (electrical faults)
- Visual fault locator (fiber breaks)
- Link lights / LEDs

---

# Layer 2 – Data Link

## Overview
Handles node-to-node communication on the same LAN using MAC addresses.

---

## PDU
- Frame

---

## Core Functions
- Local delivery within the same network
- Uses MAC addresses (48-bit)
- Handles framing and error detection
- Controls access to the physical medium

---

## Key Devices
- Switch
- NIC (Network Interface Card)
- Bridge (legacy)

---

## Protocols
- Ethernet (IEEE 802.3)

---

## Troubleshooting Layer 2
- Same network communication fails
- MAC address issues
- VLAN misconfiguration
- Switch port errors

---

# Layer 3 – Network

## Overview
Responsible for routing data between different networks using IP addresses.

---

## PDU
- Packet

---

## Core Functions
- Logical addressing (IP)
- Routing between networks
- Packet fragmentation
- Path selection

---

## Key Device
- Router

---

## Protocols
- IPv4 / IPv6

---

## Troubleshooting Layer 3
- No route to host
- Incorrect IP address/subnet mask
- Default gateway issues
- Routing table problems

---

# Layer 4 – Transport

## Overview
Provides end-to-end communication between hosts.

---

## PDU
- Segment (TCP)
- Datagram (UDP)

---

## Core Functions
- Segmentation & reassembly
- Flow control
- Error recovery (TCP)
- Application multiplexing via ports

---

## Protocols

### TCP
- Reliable
- Connection-oriented
- Uses ACKs and sequencing

### UDP
- Fast
- Connectionless
- No reliability checks

---

## Key Concept
- Uses port numbers to identify applications

---

# Layer 5 – Session

## Overview
Manages sessions between applications.

---

## PDU
- Data

---

## Core Functions
- Establish sessions
- Maintain sessions
- Terminate sessions
- Session recovery (checkpoints)

---

## Examples
- NetBIOS
- RPC
- SIP (some functions)

---

## Troubleshooting Layer 5
- Session drops
- Cannot reconnect to persistent sessions
- Authentication/session timeout issues

---

# Layer 6 – Presentation

## Overview
Translates and formats data for the application layer.

---

## PDU
- Data

---

## Core Functions
- Data formatting
- Encryption / decryption
- Compression / decompression
- Character encoding

---

## Examples
- SSL / TLS (encryption)
- UTF-8, ASCII
- JPEG, MP3 encoding

---

## Troubleshooting Layer 6
- Garbled data
- Encryption mismatch
- Encoding errors

---

# Layer 7 – Application

## Overview
Closest layer to the user — provides network services directly to applications.

---

## PDU
- Data

---

## Core Functions
- User-facing network services
- Interface between user and network

---

## Common Protocols
- HTTP / HTTPS
- DNS
- SMTP / IMAP / POP3
- FTP / SFTP
- SSH
- DHCP
- SNMP
- Telnet (legacy)

---

## Troubleshooting Layer 7
- Website not loading
- DNS failures
- Email not sending/receiving
- Application login failures
