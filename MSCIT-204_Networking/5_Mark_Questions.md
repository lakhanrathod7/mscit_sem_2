# MSCIT-204: Fundamental of Computer Networking
## 5-Mark Questions (Short Notes)

1.  **⭐⭐⭐ Throughput:** What is Throughput? Explain in brief. (Repeated: Aug 2022, July 2023)
2.  **⭐⭐⭐ Attenuation:** What is Attenuation? (Repeated: July 2023)
3.  **⭐⭐⭐ Token Passing:** Define Token Passing mechanism in brief. (Repeated: July 2023, July 2025)
4.  **⭐⭐⭐ Client-Server Network:** Elaborate in brief about Client-Server vs Peer-to-Peer network. (Repeated: July 2023, July 2025)
5.  **⭐⭐⭐ Bandwidth:** Define bandwidth and explain it in brief. (Repeated: July 2025)
6.  **⭐⭐⭐ Ports and Sockets:** Discuss various ports and sockets used in networking. (Repeated: July 2025)
7.  **⭐⭐⭐ Network Layer:** Write a short note on the Network Layer. (Repeated: July 2025)
8.  **⭐⭐⭐ IEEE 802.3 Standard:** Explain in short about the IEEE 802.3 (Ethernet) standard. (Repeated: July 2025)
9.  **⭐⭐⭐ Hub and Router:** Define Hub and Router in brief. (Repeated: Jan 2023)
10. **⭐⭐⭐ DB and Mail Server:** Define Database server and Mail Server in brief. (Repeated: Jan 2023)
11. **⭐⭐ Topologies with Diagram:** Define Bus or Star topology with a diagram. (Repeated: Jan 2023)
12. **⭐⭐ Wireless Media comparison:** Discuss the comparison of different wireless media. (Repeated: Jan 2023)
13. **⭐⭐ Circuit vs Packet Switching:** Write the difference between Circuit switching and Packet switching. (Repeated: Jan 2023, July 2023)
14. **⭐⭐ Periodic vs Aperiodic Signal:** Write the difference between Periodic and Aperiodic signals. (Repeated: July 2023)
15. **⭐⭐ Coaxial Cable:** Define Coaxial Cable and its applications. (Repeated: July 2023)
16. **⭐⭐ UTP vs STP:** Define Unshielded versus Shielded Twisted-Pair cable. (Repeated: July 2023)
17. **⭐⭐ Transmission Media:** Explain Transmission Media in detail. (Repeated: Aug 2022)
18. **⭐⭐ Connectivity Devices:** Explain Connectivity Devices in detail. (Repeated: Aug 2022)
19. **⭐⭐ Data Link Layer:** Explain the Data Link Layer of the OSI model in detail. (Repeated: July 2023)
20. **⭐⭐ Internet/Intranet:** Explain internet and intranet services. (Aug 2022)

---

## Detailed Answers (5-Mark Questions)

### 1. Throughput in Networking
*   **Definition:** Throughput is the actual amount of data that is successfully transferred from one point to another in a given time period (usually bits per second).
*   **Key Factors:** It is influenced by network congestion, hardware limitations, and distance.
*   **Difference from Bandwidth:** Bandwidth is the *theoretical maximum* speed; throughput is the *actual* speed achieved in real-world conditions.
*   **Example:** A 100 Mbps connection (Bandwidth) might only deliver 60 Mbps (Throughput) during peak hours.

### 2. Attenuation
*   **Definition:** Attenuation is the loss of signal strength (amplitude) as it travels through a transmission medium.
*   **Causes:** Resistance of the copper wire, absorption by the air, or scattering in fiber optics.
*   **Measurement:** Measured in Decibels (dB).
*   **Solution:** To overcome attenuation, **Repeaters** (for digital signals) or **Amplifiers** (for analog signals) are used to boost the signal at regular intervals.

### 3. Token Passing Mechanism
*   **Definition:** A deterministic method of channel access where a special small frame called a "Token" is passed from node to node.
*   **Working:**
    1.  A node can only transmit data if it possesses the Token.
    2.  After sending data, the node releases the Token to the next node in the ring.
*   **Topologies:** Used in Ring and Bus topologies (e.g., Token Ring).
*   **Benefit:** Prevents data collisions because only one node can speak at a time.

### 4. Client-Server vs Peer-to-Peer (P2P)
*   **Client-Server:**
    *   **Structure:** Centralized. One powerful computer (Server) serves many clients.
    *   **Control:** High security and centralized backup.
    *   **Cost:** High setup cost (dedicated server).
*   **Peer-to-Peer (P2P):**
    *   **Structure:** Decentralized. Every node acts as both a client and a server.
    *   **Control:** Low security; each user manages their own resources.
    *   **Cost:** Low cost; uses existing computers.

### 5. Bandwidth
*   **Definition:** The maximum data transfer capacity of a network or internet connection.
*   **Measurement:** Bits per second (bps), Kbps, Mbps, Gbps.
*   **Concept:** Think of it as the "width of a pipe." A wider pipe can carry more water (data) at the same time.
*   **Types:**
    *   *Baseband:* Entire bandwidth used for a single signal.
    *   *Broadband:* Bandwidth divided into multiple channels for different signals.

### 6. Ports and Sockets
*   **Port:** A 16-bit numeric identifier (0-65535) used to distinguish between different services or processes on the same computer. (e.g., HTTP = 80, FTP = 21).
*   **Socket:** The combination of an **IP Address** and a **Port Number**.
    *   *Format:* `192.168.1.1:80`
*   **Usage:** Sockets allow for unique end-to-end communication between two applications across a network.

### 7. Network Layer (Layer 3)
*   **Definition:** The layer responsible for host-to-host delivery and routing of packets across multiple networks.
*   **Key Functions:**
    1.  **Routing:** Selecting the best path for data.
    2.  **Logical Addressing:** Handling IP addresses.
    3.  **Fragmentation:** Breaking large packets into smaller ones for the underlying media.
*   **Devices:** Routers operate at this layer.
*   **Protocols:** IP (IPv4/IPv6), ICMP, IGMP.

### 8. IEEE 802.3 (Ethernet) Standard
*   **Definition:** The most widely used standard for wired Local Area Networks (LANs).
*   **Key Features:**
    1.  **CSMA/CD:** Uses Collision Detection to manage channel access.
    2.  **Addressing:** Uses 48-bit MAC addresses.
    3.  **Media:** Supports Twisted Pair (10Base-T) and Fiber (1000Base-X).
*   **Goal:** Provides a reliable and high-speed physical/data link layer specification.

### 9. Hub vs Router
*   **Hub:**
    *   Layer 1 (Physical).
    *   Non-intelligent: Broadcasts data to all ports (causes congestion).
    *   Single collision domain.
*   **Router:**
    *   Layer 3 (Network).
    *   Intelligent: Forwards data based on IP addresses.
    *   Connects different networks (LAN to WAN).

### 10. Database vs Mail Server
*   **Database Server:** Stores, manages, and provides access to structured data (e.g., MySQL, Oracle). It handles queries from clients.
*   **Mail Server:** Handles the sending, receiving, and storing of electronic mail (e.g., Microsoft Exchange, Postfix).
    *   *Protocols:* Uses SMTP to send and POP3/IMAP to receive.

### 11. Topologies with Diagram
*   **Bus Topology:** Nodes connect to a single central cable (Backbone).
    *   *Pros:* Simple, cheap. *Cons:* Backbone failure kills the whole network.
*   **Star Topology:** Nodes connect to a central Hub or Switch.
    *   *Pros:* Easy to troubleshoot; if one cable fails, others stay up. *Cons:* Central device failure kills the network.
*   **Diagram:** (Star: Hub in middle with lines to PCs. Bus: Single line with PCs attached).

### 12. Wireless Media Comparison
*   **Radio Waves:** Omnidirectional (360 degrees). Used for AM/FM radio, cordless phones.
*   **Microwaves:** Unidirectional. Requires Line-of-Sight. Used for satellite and mobile communication.
*   **Infrared:** Short-range, high frequency. Cannot pass through walls. Used for remote controls and wireless mice.

### 13. Circuit vs Packet Switching
*   **Circuit Switching:** A dedicated physical path is established for the duration of the communication (e.g., traditional telephone calls). Inefficient for data but good for voice.
*   **Packet Switching:** Data is broken into small packets and sent independently. No dedicated path is required (e.g., Internet). Very efficient for data traffic.

### 14. Periodic vs Aperiodic Signal
*   **Periodic Signal:** Repeats its pattern over a fixed time interval (Period). (e.g., Sine wave, Clock signal).
*   **Aperiodic Signal:** Does not repeat its pattern over time. (e.g., Human voice, data pulses). Represents unpredictable information.

### 15. Coaxial Cable
*   **Definition:** A copper cable with a central conductor, an insulating layer, a metallic shield, and an outer jacket.
*   **Usage:** Cable TV, traditional Ethernet (Thinnet/Thicknet).
*   **Advantages:** Higher bandwidth than twisted pair; less affected by electromagnetic interference (EMI).

### 16. UTP vs STP
*   **UTP (Unshielded Twisted Pair):** No extra shielding. Very common, cheap, flexible. Used in home/office LANs.
*   **STP (Shielded Twisted Pair):** Wires are wrapped in foil to protect against electrical noise. Bulkier and more expensive. Used in industrial areas with high interference.

### 17. Transmission Media
*   **Guided (Wired):** Twisted Pair (Ethernet), Coaxial (TV), Fiber Optic (Light signals).
*   **Unguided (Wireless):** Radio waves, Microwaves, Infrared.
*   **Concept:** The physical path through which electromagnetic signals travel from sender to receiver.

### 18. Connectivity Devices (Detailed)
*   **Hub:** Repeats data to all ports (Layer 1).
*   **Switch:** Forwards data to specific MAC addresses (Layer 2).
*   **Router:** Routes data between different networks using IP (Layer 3).
*   **Bridge:** Connects two similar network segments (Layer 2).
*   **Gateway:** Connects two dissimilar networks (All layers).

### 19. Data Link Layer (Layer 2)
*   **Functions:**
    1.  **Framing:** Organizing bits into frames.
    2.  **Physical Addressing:** Using MAC addresses.
    3.  **Flow Control:** Keeping sender from overwhelming receiver.
    4.  **Error Control:** Detecting and re-transmitting lost frames (CRC).
*   **Sub-layers:** LLC (Logical Link Control) and MAC (Media Access Control).

### 20. Internet vs Intranet
*   **Internet:** A global public network accessible to everyone. Used for global information sharing.
*   **Intranet:** A private network owned by an organization, accessible only to members. Used for internal document sharing and collaboration. Both use TCP/IP.
