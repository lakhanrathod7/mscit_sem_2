# MSCIT-204: Fundamental of Computer Networking
## 10-Mark Questions (Important for Exam)

1.  **⭐⭐⭐ Networking Components:** What is Networking? Explain its components in detail. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
2.  **⭐⭐⭐ OSI Reference Model:** Explain the OSI Reference Model in detail with all 7 layers and their functions. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
3.  **⭐⭐⭐ Transmission Media:** Explain Guided (Coaxial, Twisted Pair, Fiber Optic) and Unguided (Wireless) media in detail. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
4.  **⭐⭐⭐ Network Topologies:** Define Topology. Explain different types of network topologies (Star, Mesh, Bus, Ring, Tree) with diagrams. (Repeated: Aug 2022, Jan 2023, July 2025)
5.  **⭐⭐⭐ Switching & Routing:** Explain Switching and Routing in networks. Compare Circuit Switching vs Packet Switching. (Repeated: Aug 2022, Jan 2023, July 2023)
6.  **⭐⭐⭐ TCP/IP Model:** List the layers of the TCP/IP model and explain any two in detail. (Repeated: July 2023)
7.  **⭐⭐⭐ IEEE Standards:** Explain IEEE Standards (802.3, 802.11) in detail. (Repeated: Aug 2022, July 2025)
8.  **⭐⭐⭐ Internet & Intranet Services:** Explain internet and intranet services in detail. (Repeated: Aug 2022, July 2025)
9.  **⭐⭐⭐ Distance Vector Routing:** Elaborate in detail about the Distance Vector Routing algorithm. (Repeated: Jan 2023, July 2025)
10. **⭐⭐⭐ Twisted Pair Cables:** Explain about Twisted Pair Cables (UTP/STP) in detail. (Repeated: July 2023, July 2025)
11. **⭐⭐ Local Area Network (LAN):** Explain Local Area Network in detail. (Repeated: Aug 2022)
12. **⭐⭐ Communication Theory:** Explain the fundamentals of Communication Theory in detail. (Repeated: Aug 2022)
13. **⭐⭐ Connectivity Devices:** Explain connectivity devices (Hub, Switch, Router, Bridge, Gateway) in detail. (Repeated: Aug 2022)
14. **⭐⭐ Transmission Impairment:** Explain transmission impairment (Attenuation, Distortion, Noise) in detail. (Repeated: Jan 2023)
15. **⭐⭐ Network Layers Conceptualization:** Explain the conceptualizing of layers of the OSI model in detail. (Repeated: Aug 2022)

---

## Detailed Answers (10-Mark Questions)

### 1. Networking & Its Components
*   **Definition:** A computer network is a system of interconnected computers that share resources and information.
*   **Five Key Components:**
    1.  **Sender:** The device that initiates the data transfer (e.g., PC, Mobile).
    2.  **Receiver:** The device that receives the message.
    3.  **Message:** The actual data being sent (Text, Audio, Video).
    4.  **Transmission Medium:** The physical or wireless path (Cables, Radio waves).
    5.  **Protocol:** The set of rules that govern how data is sent and received (e.g., TCP/IP). Without protocol, devices can connect but cannot understand each other.

### 2. OSI Reference Model (7 Layers)
*   **1. Physical Layer:** Handles bits and hardware (cables, hubs).
*   **2. Data Link Layer:** Handles frames and physical addressing (MAC address, switches).
*   **3. Network Layer:** Handles packets and routing (IP address, routers).
*   **4. Transport Layer:** Handles end-to-end reliability (TCP/UDP, port numbers).
*   **5. Session Layer:** Manages sessions and dialogues between applications.
*   **6. Presentation Layer:** Handles data encryption, compression, and formatting.
*   **7. Application Layer:** The layer users interact with (HTTP, FTP, Email).
*   **Mnemonic:** **A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing.

### 3. Transmission Media (Guided & Unguided)
*   **Guided (Wired):**
    1.  **Twisted Pair:** Most common (Ethernet). UTP is cheap; STP is shielded.
    2.  **Coaxial:** Copper core with shielding. Used for Cable TV.
    3.  **Fiber Optic:** Uses light pulses through glass. Fastest, immune to electrical noise, very expensive.
*   **Unguided (Wireless):**
    1.  **Radio Waves:** For broad broadcasting (WiFi, Bluetooth).
    2.  **Microwaves:** For point-to-point (Satellite). Requires line-of-sight.
    3.  **Infrared:** Very short range (Remote controls).

### 4. Network Topologies
*   **Star:** All nodes connect to a central hub. Easy to manage, but hub is a single point of failure.
*   **Bus:** All nodes connect to one backbone cable. Cheap, but hard to troubleshoot.
*   **Ring:** Each node has two neighbors. Data travels in one direction.
*   **Mesh:** Every node connects to every other node. Highest reliability but very expensive.
*   **Tree:** A hierarchical combination of Star and Bus.

### 5. Switching and Routing
*   **Switching:** Moving data across a network.
    *   *Circuit Switching:* Dedicated physical path (Phone call).
    *   *Packet Switching:* Data broken into packets; no dedicated path (Internet).
*   **Routing:** Selecting the best path for packets to reach their destination using IP addresses and routing tables.

### 6. TCP/IP Model
*   **Layers:**
    1.  **Network Access Layer:** (OSI 1 & 2) Physical hardware and MAC.
    2.  **Internet Layer:** (OSI 3) IP addressing and routing.
    3.  **Transport Layer:** (OSI 4) End-to-end delivery (TCP/UDP).
    4.  **Application Layer:** (OSI 5, 6, 7) Services like Web and Email.
*   **Comparison:** OSI is a theoretical model; TCP/IP is the practical model used on the real Internet.

### 7. IEEE Standards (802.3 and 802.11)
*   **IEEE 802.3 (Ethernet):** Defines the physical and data link layers for wired networks. Includes rules for CSMA/CD and cabling.
*   **IEEE 802.11 (WiFi):** Defines standards for Wireless LANs. Includes variations like 802.11a/b/g/n/ac.
*   **Importance:** These standards ensure that equipment from different manufacturers (e.g., Cisco and D-Link) can work together.

### 8. Internet & Intranet Services
*   **Internet:** Public global network. Services: WWW, Email, File Transfer (FTP), Social Media.
*   **Intranet:** Private company network. Services: Internal websites, document sharing (SharePoint), internal messaging.
*   **Difference:** Access control. Anyone can access the Internet; only authorized users can access an Intranet.

### 9. Distance Vector Routing Algorithm
*   **Concept:** Each router maintains a table of distances (hops) to all known destinations.
*   **Mechanism:** Routers share their entire routing table with neighbors periodically.
*   **Algorithm:** Uses the Bellman-Ford algorithm to find the shortest path.
*   **Protocol:** RIP (Routing Information Protocol) is a classic example.

### 10. Twisted Pair Cables (UTP/STP)
*   **Concept:** Two copper wires twisted to reduce electromagnetic interference.
*   **UTP (Unshielded):** No foil. Used in homes/offices. Categories: Cat5e, Cat6.
*   **STP (Shielded):** Has a metal foil shield. Used in factories or areas with high interference.
*   **Connectors:** Usually uses RJ-45 connectors.

### 11. Local Area Network (LAN)
*   **Definition:** A network limited to a small area like a room or building.
*   **Features:** High data transfer speed, low error rate, and private ownership.
*   **Technology:** Usually uses Ethernet (wired) or WiFi (wireless).

### 12. Communication Theory Fundamentals
*   **Model:** Sender -> Encoder -> Channel -> Decoder -> Receiver.
*   **Key Concepts:**
    1.  **Baud Rate:** Number of signal changes per second.
    2.  **Bit Rate:** Number of bits sent per second.
    3.  **Signal-to-Noise Ratio (SNR):** Measure of signal quality.

### 13. Connectivity Devices (Detailed)
*   **Hub:** Layer 1, broadcasts data.
*   **Switch:** Layer 2, filters data by MAC address.
*   **Router:** Layer 3, connects networks via IP.
*   **Bridge:** Connects two LAN segments.
*   **Gateway:** Translates between different protocols.

### 14. Transmission Impairment
*   **Attenuation:** Signal gets weaker over distance.
*   **Distortion:** Signal changes shape due to different frequencies traveling at different speeds.
*   **Noise:** Unwanted electrical signals (Crosstalk, Impulse noise).

### 15. Conceptualizing OSI Layers
*   **Why Layers?** To simplify networking, allow for modularity, and ensure that changes in one layer don't break others.
*   **Data Flow:** As data moves down, it is **Encapsulated** (headers added). As it moves up, it is **Decapsulated** (headers removed).
*   **Units:** Data (Top 3) -> Segment (Transport) -> Packet (Network) -> Frame (Data Link) -> Bits (Physical).
