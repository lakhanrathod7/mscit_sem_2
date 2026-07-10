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
*   **Key Factors:** It is influenced by:
    1.  **Network Congestion:** High traffic reduces speed.
    2.  **Hardware Limitations:** Processing speed of routers/switches.
    3.  **Distance:** Latency increases with distance.
    4.  **Error Rate:** Re-transmission of lost packets slows down the total flow.
*   **Difference from Bandwidth:** Bandwidth is the *theoretical maximum* speed of a link; throughput is the *actual* speed achieved under real-world conditions.

### 2. Attenuation
*   **Definition:** Attenuation is the loss of signal strength (amplitude) as it travels through a transmission medium. It is a natural phenomenon where signal energy is dissipated.
*   **Causes:**
    1.  **Resistance:** Copper wires resist electrical flow, generating heat.
    2.  **Absorption:** Medium (like air) absorbs some of the signal energy.
    3.  **Physical Obstacles:** Walls or distance.
*   **Measurement:** Measured in Decibels (dB).
*   **Solution:** To overcome attenuation, **Repeaters** (for digital) or **Amplifiers** (for analog) are used to regenerate and boost the signal.

### 3. Token Passing Mechanism
*   **Definition:** A deterministic method of channel access used in some local area networks (LANs) where a special small frame called a "Token" is passed from node to node.
*   **Working:**
    1.  A node can only transmit data if it possesses the Token.
    2.  When a node has data to send, it "captures" the token, attaches its data, and sends it.
    3.  Once the receiver acknowledges or the data reaches the destination, the node releases the Token to the next neighbor in the logical ring.
*   **Benefit:** It eliminates data collisions entirely and provides predictable access time for all nodes.

### 4. Client-Server vs Peer-to-Peer (P2P)
*   **Client-Server:**
    *   **Architecture:** Centralized. One or more powerful computers (Servers) provide resources and services to multiple less powerful computers (Clients).
    *   **Control:** High security and centralized management.
    *   **Scale:** Can support thousands of users.
*   **Peer-to-Peer (P2P):**
    *   **Architecture:** Decentralized. Every node acts as both a client and a server, sharing its own resources directly with others.
    *   **Control:** Low security; hard to manage backups.
    *   **Scale:** Only suitable for small networks (home or small office).

### 5. Bandwidth
*   **Definition:** The maximum data transfer capacity of a network or internet connection. It is the measure of how much data can be sent over a link in a given time.
*   **Measurement:** Bits per second (bps), Kbps, Mbps, Gbps.
*   **Analogy:** If you think of a highway, bandwidth is the number of lanes. More lanes allow more cars (data) to travel simultaneously.
*   **Types:**
    *   *Baseband:* Uses the entire bandwidth for a single signal (Digital).
    *   *Broadband:* Divides bandwidth into multiple channels for different signals (Analog/Cable).

### 6. Ports and Sockets
*   **Port:** A 16-bit numeric identifier (0-65535) used by the Transport Layer (TCP/UDP) to distinguish between different services or applications on the same host. (e.g., HTTP = 80, HTTPS = 443, FTP = 21).
*   **Socket:** The unique combination of an **IP Address** and a **Port Number**.
    *   *Example:* `192.168.1.1:80`
*   **Usage:** Sockets represent an endpoint for communication. Two sockets (one on each host) are needed to establish a complete end-to-end communication link.

### 7. Network Layer (Layer 3)
*   **Definition:** The layer of the OSI model responsible for host-to-host delivery and routing of packets across multiple networks.
*   **Key Functions:**
    1.  **Routing:** Selecting the most efficient path for data packets.
    2.  **Logical Addressing:** Managing IP addresses (IPv4/IPv6).
    3.  **Fragmentation:** Breaking large packets into smaller units for transmission.
*   **Devices:** Routers are the primary devices at this layer.
*   **Protocols:** IP, ICMP (for error reporting), ARP (IP to MAC mapping).

### 8. IEEE 802.3 (Ethernet) Standard
*   **Definition:** The most widely used international standard for wired Local Area Networks (LANs).
*   **Key Features:**
    1.  **CSMA/CD:** Carrier Sense Multiple Access with Collision Detection is the protocol used to manage channel access.
    2.  **Cabling:** Supports various media like Coaxial (10Base2), Twisted Pair (10Base-T), and Fiber (1000Base-X).
    3.  **Addressing:** Uses 48-bit unique hardware addresses called MAC addresses.
*   **Importance:** It ensures interoperability between networking hardware from different manufacturers.

### 9. Hub vs Router
*   **Hub:**
    *   Operates at the Physical Layer (Layer 1).
    *   "Dumb" device: It broadcasts all incoming data to all its ports, causing high network traffic and potential collisions.
*   **Router:**
    *   Operates at the Network Layer (Layer 3).
    *   Intelligent device: It reads IP addresses and forwards data only to the specific network or host where it belongs. It can connect different types of networks (e.g., LAN to WAN).

### 10. Database vs Mail Server
*   **Database Server:** A powerful computer that stores, manages, and provides shared access to structured data. It processes complex queries from multiple clients simultaneously. (e.g., MySQL, SQL Server).
*   **Mail Server:** A server dedicated to handling the exchange of electronic mail. It receives emails, stores them, and forwards them to the recipient.
    *   *Protocols:* Uses SMTP (Simple Mail Transfer Protocol) for sending and POP3 or IMAP for receiving and storage.

### 11. Topologies with Diagram
*   **Bus Topology:** All devices connect to a single central cable (Backbone).
    *   *Pros:* Simple, cheap. *Cons:* If backbone fails, whole network goes down.
*   **Star Topology:** All devices connect to a central Hub or Switch.
    *   *Pros:* High reliability; if one cable fails, only that node is affected. *Cons:* If central hub fails, whole network dies.
*   **Diagram Idea:** Star is a central hub with radiating lines; Bus is a single line with branches to PCs.

### 12. Wireless Media Comparison
*   **Radio Waves:** Frequencies from 3 kHz to 1 GHz. Omnidirectional. Used for AM/FM radio, cordless phones. Good for long distances and passing through walls.
*   **Microwaves:** Frequencies from 1 GHz to 300 GHz. Unidirectional (Line-of-Sight). Used for satellite and terrestrial mobile links. High bandwidth but blocked by obstacles.
*   **Infrared:** Very high frequency (300 GHz to 400 THz). Short-range. Cannot pass through walls. Used for remote controls and wireless mice.

### 13. Circuit vs Packet Switching
*   **Circuit Switching:** A dedicated physical path is established between two nodes before communication begins (e.g., traditional phone calls). Bandwidth is reserved, providing a constant bit rate but is inefficient for data.
*   **Packet Switching:** Data is broken into small packets, each containing a header with destination info. Packets can take different routes and are reassembled at the destination (e.g., Internet). Much more efficient for bursty data traffic.

### 14. Periodic vs Aperiodic Signal
*   **Periodic Signal:** A signal that repeats its pattern over a fixed time interval (Period). Examples include Sine waves (Analog) or Clock pulses (Digital).
*   **Aperiodic Signal:** A signal that does not repeat its pattern over time. It represents unpredictable data like human speech or binary data pulses in a computer network.

### 15. Coaxial Cable
*   **Definition:** A cable consisting of a central copper conductor, an insulating layer, a metallic shield (to prevent interference), and an outer protective jacket.
*   **Applications:** Primarily used for Cable TV distribution and older Ethernet LANs (Thinnet/Thicknet).
*   **Pros:** Supports higher bandwidth and longer distances than Twisted Pair; highly resistant to EMI.

### 16. UTP vs STP
*   **UTP (Unshielded Twisted Pair):** No extra foil or braiding. Very common, flexible, and inexpensive. Used in standard home/office Ethernet (Cat5e, Cat6).
*   **STP (Shielded Twisted Pair):** Wires are wrapped in a metallic foil shield to protect against electromagnetic interference (EMI). Bulkier and more expensive. Used in industrial environments with heavy machinery.

### 17. Transmission Media
*   **Definition:** The physical path through which electromagnetic signals travel between the sender and receiver.
*   **Guided (Wired):** Uses physical conductors.
    *   *Twisted Pair:* Ethernet cables.
    *   *Coaxial:* TV cables.
    *   *Fiber Optic:* Uses light pulses through glass (Fastest).
*   **Unguided (Wireless):** Uses air/space.
    *   *Radio waves, Microwaves, Infrared.*

### 18. Connectivity Devices (Summary)
*   **Hub:** Repeats data to all ports (Layer 1).
*   **Switch:** Forwards data based on MAC address (Layer 2).
*   **Router:** Routes data between networks based on IP address (Layer 3).
*   **Bridge:** Connects two similar network segments (Layer 2).
*   **Gateway:** A complex device that connects two networks using completely different protocols (all layers).

### 19. Data Link Layer (Layer 2)
*   **Function:** Responsible for node-to-node delivery and ensuring error-free transmission of data over the physical layer.
*   **Key Tasks:**
    1.  **Framing:** Breaking bits into manageable units called frames.
    2.  **Physical Addressing:** Using MAC addresses (e.g., `AA:BB:CC...`).
    3.  **Flow Control:** Preventing the sender from overwhelming the receiver.
    4.  **Error Control:** Detecting and re-transmitting damaged or lost frames (CRC).

### 20. Internet vs Intranet
*   **Internet:** A global public network of interconnected networks. It is accessible to everyone and provides services like WWW, Email, and FTP.
*   **Intranet:** A private, secure network belonging to an organization. It is accessible only to authorized members/employees. It uses the same technologies (TCP/IP) as the internet but is protected by firewalls.
