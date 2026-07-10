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
*   **Definition:** A computer network is a system of interconnected computers and peripheral devices that exchange information and share resources.
*   **Five Major Components:**
    1.  **Message:** The information or data to be communicated. It can consist of text, numbers, pictures, sound, or video.
    2.  **Sender:** The device that sends the data message. It can be a computer, workstation, telephone handset, video camera, and so on.
    3.  **Receiver:** The device that receives the message.
    4.  **Transmission Medium:** The physical path by which a message travels from sender to receiver. It can be guided (wires) or unguided (wireless).
    5.  **Protocol:** A set of rules that govern data communication. It represents an agreement between the communicating devices. Without a protocol, two devices may be connected but not communicating, like a person speaking French and another speaking Japanese.

### 2. OSI Reference Model (7 Layers)
The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a communication system into seven logical layers.

1.  **Physical Layer (Layer 1):** Responsible for the actual physical connection between devices. It handles bits, voltages, and cable specifications.
2.  **Data Link Layer (Layer 2):** Responsible for node-to-node delivery. It handles physical addressing (MAC), framing, and error detection.
3.  **Network Layer (Layer 3):** Responsible for host-to-host delivery and routing. It handles logical addressing (IP) and finds the best path for data.
4.  **Transport Layer (Layer 4):** Responsible for end-to-end communication and reliability. It handles flow control, segmentation, and error correction (TCP/UDP).
5.  **Session Layer (Layer 5):** Manages, maintains, and synchronizes the conversation between different applications.
6.  **Presentation Layer (Layer 6):** Translates, encrypts, and compresses data so that it is readable by the application layer.
7.  **Application Layer (Layer 7):** The topmost layer where the user interacts with the software application (HTTP, FTP, SMTP).

### 3. Transmission Media (Guided & Unguided)
Transmission media are the physical pathways that carry data from the transmitter to the receiver.

*   **Guided Media (Wired):**
    1.  **Twisted Pair Cable:** Two copper wires twisted together to reduce interference. Common in Ethernet LANs (UTP/STP).
    2.  **Coaxial Cable:** A central copper conductor surrounded by insulation and a metallic shield. Used for Cable TV and high-speed internet.
    3.  **Fiber Optic Cable:** Uses pulses of light to transmit data through glass or plastic fibers. Offers the highest bandwidth and is immune to electromagnetic interference.
*   **Unguided Media (Wireless):**
    1.  **Radio Waves:** Omnidirectional waves used for AM/FM radio, cordless phones, and WiFi.
    2.  **Microwaves:** Unidirectional waves used for line-of-sight communication like satellite and mobile networks.
    3.  **Infrared:** Short-range waves used in remote controls and wireless keyboards.

### 4. Network Topologies
Topology refers to the physical or logical arrangement of nodes and connections in a network.

1.  **Mesh Topology:** Every device has a point-to-point link to every other device. It is highly reliable but very expensive and complex to install.
2.  **Star Topology:** All devices connect to a central Hub or Switch. It is easy to install and manage. If one link fails, others stay up; however, if the hub fails, the whole network fails.
3.  **Bus Topology:** All devices connect to a single central cable called the backbone. It is inexpensive for small networks but hard to troubleshoot.
4.  **Ring Topology:** Each device has a point-to-point connection with only the two devices on either side of it. Data travels in one direction.
5.  **Tree Topology:** A combination of Star and Bus topologies. It has a root node connected to several other nodes in a hierarchical manner.

### 5. Switching and Routing
*   **Switching:** The process of moving data from one network segment to another.
    *   **Circuit Switching:** A dedicated physical path is established for the duration of the communication (e.g., telephone calls).
    *   **Packet Switching:** Data is broken into small packets and sent independently. Packets may take different routes and are reassembled at the destination (e.g., Internet).
*   **Routing:** The process of selecting the best path for data packets to travel across a network toward their destination. It uses routing tables and protocols like RIP, OSPF, and BGP.

### 6. TCP/IP Model (Layers and Comparison)
The TCP/IP model is the practical model used on the internet. It has four layers:

1.  **Network Access Layer:** Combines OSI Physical and Data Link layers. It deals with hardware and MAC addresses.
2.  **Internet Layer:** Equivalent to the OSI Network layer. It uses the IP protocol to route packets.
3.  **Transport Layer:** Equivalent to the OSI Transport layer. It uses TCP (Reliable) and UDP (Fast) for end-to-end communication.
4.  **Application Layer:** Combines OSI Session, Presentation, and Application layers. It includes protocols like HTTP, FTP, and SMTP.
*   **Comparison:** OSI is a theoretical 7-layer model; TCP/IP is a 4-layer practical model. OSI provides a clear distinction between services, interfaces, and protocols.

### 7. IEEE Standards (802.3 and 802.11)
IEEE standards ensure that networking hardware from different vendors can communicate.

*   **IEEE 802.3 (Ethernet):** Defines the standard for wired LANs. It specifies the Physical and Data Link layer properties, including the CSMA/CD protocol, cabling types, and MAC frame format.
*   **IEEE 802.11 (WiFi):** Defines the standard for Wireless LANs. It includes several variations like 802.11a, b, g, n, and ac, each offering different speeds and frequencies (2.4 GHz and 5 GHz). It uses CSMA/CA (Collision Avoidance).

### 8. Internet and Intranet Services
*   **Internet:** A global public network of interconnected computer networks that use the TCP/IP protocol suite. Services include World Wide Web (WWW), Email, File Transfer, Social Networking, and E-commerce.
*   **Intranet:** A private network accessible only to an organization's members. It uses the same technologies as the internet but is protected by a firewall.
*   **Services:**
    1.  **Web Services:** Accessing information through browsers.
    2.  **Communication:** Email and instant messaging.
    3.  **File Sharing:** Centralized storage for documents.
    4.  **Remote Access:** Accessing resources from outside via VPN.

### 9. Distance Vector Routing Algorithm
Distance Vector Routing is a dynamic routing algorithm where each router maintains a table (Vector) giving the minimum distance (Hops) to every destination.

*   **Working:**
    1.  Routers share their entire routing table only with their immediate neighbors at regular intervals.
    2.  They update their tables based on the information received using the **Bellman-Ford algorithm**.
    3.  If a shorter path is found, the routing table is updated.
*   **Pros:** Easy to configure and maintain for small networks.
*   **Cons:** "Count to Infinity" problem and slow convergence in large networks.

### 10. Twisted Pair Cables (UTP/STP)
Twisted pair cabling consists of pairs of copper wires twisted around each other to cancel out electromagnetic interference.

*   **UTP (Unshielded Twisted Pair):** It has no metallic shield. It is the most common type of networking cable, used in standard Ethernet. It is cheap, flexible, and easy to install.
*   **STP (Shielded Twisted Pair):** It has an additional metallic foil or braiding to protect the signals from interference. It is used in industrial environments with high electrical noise.
*   **Categories:** Cat5e (1 Gbps), Cat6 (10 Gbps), Cat7 (High speed with better shielding).

### 11. Local Area Network (LAN)
*   **Definition:** A LAN is a network that is confined to a relatively small geographical area, such as a single room, a building, or a campus.
*   **Key Characteristics:**
    1.  **High Speed:** LANs offer high data transfer rates, typically from 10 Mbps to 10 Gbps.
    2.  **Low Error Rate:** Due to short distances and high-quality cabling.
    3.  **Private Ownership:** Usually owned and operated by a single person or organization.
*   **Technologies:** Uses Ethernet (Wired) or IEEE 802.11 (Wireless).
*   **Components:** Computers, NICs (Network Interface Cards), Hubs/Switches, and Cables.

### 12. Communication Theory Fundamentals
Communication theory is the study of the process of sending and receiving information through various media.

*   **Basic Model:**
    1.  **Information Source:** Generates the message.
    2.  **Transmitter:** Encodes the message into a signal.
    3.  **Channel:** The medium that carries the signal.
    4.  **Receiver:** Decodes the signal back into a message.
    5.  **Destination:** The intended recipient.
*   **Key Concepts:**
    *   **Baud Rate:** Number of signal changes per second.
    *   **Bit Rate:** Number of bits transmitted per second.
    *   **Modulation:** Changing the characteristics of a carrier wave (Amplitude, Frequency, Phase) to encode data.

### 13. Connectivity Devices (Detailed)
1.  **Hub:** A Physical Layer device that repeats data to all its ports. It broadcasts everything, leading to high traffic.
2.  **Switch:** A Data Link Layer device that filters data by MAC address. It is more efficient than a hub because it sends data only to the intended recipient.
3.  **Router:** A Network Layer device that connects different networks and routes data using IP addresses.
4.  **Bridge:** Connects two similar LAN segments and filters traffic by MAC address.
5.  **Gateway:** A complex device used to connect two networks with entirely different protocols (e.g., connecting a LAN to a Mainframe).

### 14. Transmission Impairment
As a signal travels through a medium, it undergoes changes that can degrade its quality.

1.  **Attenuation:** The signal gets weaker as it travels further. Repeaters are used to boost the signal.
2.  **Distortion:** The signal changes its shape because different frequency components travel at different speeds.
3.  **Noise:** Unwanted electrical signals that get added to the original signal.
    *   **Thermal Noise:** Caused by random motion of electrons.
    *   **Induced Noise:** From external sources like motors.
    *   **Crosstalk:** Interference from an adjacent wire.
    *   **Impulse Noise:** Spikes caused by lightning or power surges.

### 15. Conceptualizing OSI Layers
The OSI model divides the complex process of networking into manageable layers.

*   **Data Encapsulation:** As data moves from the Application to the Physical layer, each layer adds its own "Header" containing control information. The Data Link layer also adds a "Trailer".
*   **Peer-to-Peer Communication:** Logically, Layer N on one machine communicates with Layer N on the other machine using a specific protocol.
*   **Units of Data:**
    *   **Application/Presentation/Session:** Data.
    *   **Transport:** Segment.
    *   **Network:** Packet.
    *   **Data Link:** Frame.
    *   **Physical:** Bits.
*   **Purpose:** Standardizes hardware and software so they can work together regardless of the manufacturer.
