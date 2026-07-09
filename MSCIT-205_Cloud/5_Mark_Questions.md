# MSCIT-205: Cloud Infrastructure and Services
## 5-Mark Questions (Short Notes)

1.  **⭐⭐⭐ Characteristics of Cloud:** Explain the characteristics of Cloud Computing in brief. (Repeated: Aug 2022, Jan 2023, July 2023)
2.  **⭐⭐⭐ GRID Computing:** Write a short note on GRID Computing. (Repeated: Aug 2022)
3.  **⭐⭐⭐ Cloud Service Models:** Write a short note on Cloud Service Models (SaaS, PaaS, IaaS). (Repeated: Aug 2022, Jan 2023, July 2025)
4.  **⭐⭐⭐ Security as a Service:** Explain benefits of Security as a Service (SecaaS). (Repeated: Aug 2022, July 2025)
5.  **⭐⭐⭐ Cloud Database:** Explain Cloud Database with its types (Relational, NoSQL) and benefits. (Repeated: Aug 2022, Jan 2023)
6.  **⭐⭐⭐ Cloud Application Security:** Explain best practices for cloud application security. (Repeated: Aug 2022, July 2023, July 2025)
7.  **⭐⭐⭐ DBaaS Architecture:** Explain DBaaS architecture in detail. (Repeated: Jan 2023)
8.  **⭐⭐⭐ Cloud Security Risk Analysis:** Explain cloud security risk analysis. (Repeated: Jan 2023)
9.  **⭐⭐⭐ Cloud Native vs Traditional:** Differentiate between cloud native application and traditional application. (Repeated: July 2023, July 2025)
10. **⭐⭐⭐ Hybrid Cloud:** Explain hybrid cloud and its advantages. (Repeated: July 2023, July 2025)
11. **⭐⭐⭐ Cloud Service Brokerage:** Discuss in brief about Cloud Services Brokerage (CSB). (Repeated: July 2023, July 2025)
12. **⭐⭐⭐ Application vs Infrastructure Security:** How does application security differ from infrastructure security in cloud computing? (Repeated: July 2025)
13. **⭐⭐⭐ Client-Server vs Peer-to-Peer:** Differentiate between client-server architecture and peer-to-peer architecture. (Repeated: July 2025)
14. **⭐⭐⭐ Cloud Application Requirements:** What are the major requirements for designing a cloud application? (Repeated: July 2025, Aug 2022)
15. **⭐⭐⭐ Cloud Layered Architecture:** Write a short note on cloud layered architecture. (Repeated: July 2023, Jan 2023)
16. **⭐⭐⭐ SOA vs Cloud Computing:** What are the similarities and differences between Service-Oriented Architecture and Cloud Computing? (Repeated: July 2025)
17. **⭐⭐ Recovery and Disaster Management:** Briefly discuss Cloud Disaster Recovery. (Repeated: Aug 2022)
18. **⭐⭐ Data Challenges:** Discuss various challenges related to cloud data (segregation, redundancy). (Repeated: July 2023, Aug 2022)
19. **⭐⭐ SDLC for Cloud:** List and explain various steps of cloud application software development life cycle. (Repeated: July 2023)
20. **⭐⭐ Virtualization (Hypervisor):** Briefly explain the role of a Hypervisor or VMM. (Repeated: July 2023)

---

## Detailed Answers (5-Mark Questions)

### 1. Characteristics of Cloud Computing
*   **On-demand Self-service:** Users can get computing resources (server time, storage) automatically without needing human interaction with the provider.
*   **Broad Network Access:** Services are available over the network and accessed through standard platforms (Laptops, Mobiles).
*   **Resource Pooling:** Provider's resources are pooled to serve multiple customers (Multi-tenancy).
*   **Rapid Elasticity:** Resources can be scaled up or down instantly based on demand.
*   **Measured Service:** Cloud systems automatically control and optimize resource use by leveraging a metering capability (Pay-per-use).

### 2. GRID Computing
*   **Definition:** A distributed computing architecture that combines computer resources from multiple domains to reach a common main objective (like solving a complex scientific problem).
*   **Key Features:**
    1.  **Heterogeneous:** Involves different types of computers and OS.
    2.  **Geographically Distributed:** Nodes can be located anywhere in the world.
    3.  **Loose Coupling:** Nodes are not strictly dependent on each other.
*   **Example:** SETI@home or large-scale weather modeling.

### 3. Cloud Service Models (SaaS, PaaS, IaaS)
*   **IaaS (Infrastructure as a Service):** Provides virtualized hardware (Servers, Storage). User manages OS and Apps. (e.g., AWS EC2).
*   **PaaS (Platform as a Service):** Provides a platform (OS + Runtime) for developers. User manages only Apps. (e.g., Google App Engine).
*   **SaaS (Software as a Service):** Provides complete software via the web. User only uses the app. (e.g., Gmail, Dropbox).

### 4. Security as a Service (SecaaS)
*   **Definition:** An outsourcing model for security management where a provider integrates security services into a corporate infrastructure.
*   **Benefits:**
    1.  **Cost Savings:** No need to buy expensive security hardware.
    2.  **Constant Updates:** Protection against the newest threats is handled by experts.
    3.  **Expertise:** Access to specialized security professionals.
    4.  **Scalability:** Security grows as the business grows.

### 5. Cloud Database (Relational vs NoSQL)
*   **Relational (SQL):** Structured data using tables and relationships. Best for transactional data (e.g., AWS RDS).
*   **NoSQL:** Unstructured or semi-structured data (Document, Key-Value, Graph). Best for big data and real-time apps (e.g., MongoDB).
*   **Benefits:** High availability, automatic backups, and scalability.

### 6. Cloud Application Security Best Practices
1.  **Identity & Access Management (IAM):** Use Multi-Factor Authentication (MFA).
2.  **Encryption:** Encrypt data at rest (storage) and in transit (network).
3.  **Regular Audits:** Frequent vulnerability scanning and penetration testing.
4.  **API Security:** Authenticate and secure all application interfaces.

### 7. DBaaS Architecture
*   **Definition:** Database-as-a-Service provides database functionality without the need for physical hardware setup.
*   **Architecture Layers:**
    1.  **Service Layer:** Interface for the user.
    2.  **Management Layer:** Handles provisioning, backups, and scaling.
    3.  **Resource Layer:** The actual VMs and storage hosting the database.

### 8. Cloud Security Risk Analysis
*   **Process:** Identifying and evaluating threats to cloud-based data.
*   **Key Risks:** Data loss, account hijacking, insecure APIs, and shared technology vulnerabilities.
*   **Steps:** Asset identification -> Threat assessment -> Vulnerability analysis -> Risk calculation.

### 9. Cloud Native vs Traditional Applications
*   **Traditional:** Monolithic (single block), hard to scale, manual updates, tied to specific hardware.
*   **Cloud Native:** Microservices (modular), containerized (Docker), automated scaling, and independent of specific infrastructure.

### 10. Hybrid Cloud
*   **Definition:** A combination of at least one private cloud and at least one public cloud.
*   **Advantages:**
    1.  **Security:** Sensitive data stays on private cloud.
    2.  **Scalability:** Less critical tasks can "burst" into the public cloud during peak times.
    3.  **Cost:** Pay for public resources only when needed.

### 11. Cloud Service Brokerage (CSB)
*   **Definition:** An intermediary that adds value to one or more cloud services on behalf of users.
*   **Roles:**
    1.  **Aggregation:** Combining multiple services.
    2.  **Integration:** Making different services work together.
    3.  **Customization:** Tailoring services for specific needs.

### 12. Application vs Infrastructure Security
*   **Infrastructure Security:** Protecting the hardware, data center, and network (usually the provider's job).
*   **Application Security:** Protecting the software code, user data, and access logic (usually the customer's job).

### 13. Client-Server vs Peer-to-Peer
*   **Client-Server:** Centralized control. One server serves many clients. Highly secure.
*   **Peer-to-Peer:** Decentralized. Every computer is both a client and a server. Hard to secure but very resilient.

### 14. Cloud Application Requirements
1.  **Scalability:** Handling increased user load.
2.  **Multi-tenancy:** Serving many customers from one instance.
3.  **Availability:** Ensuring the app is always online.
4.  **Interoperability:** Connecting with other systems.

### 15. Cloud Layered Architecture
*   **Layers:**
    1.  **Hardware Layer:** Physical servers.
    2.  **Infrastructure Layer:** Virtualization and storage.
    3.  **Platform Layer:** OS and middleware.
    4.  **Application Layer:** The software users interact with.

### 16. SOA vs Cloud Computing
*   **SOA (Service Oriented Architecture):** A design philosophy (software architecture style).
*   **Cloud:** A delivery model (infrastructure).
*   **Relationship:** SOA-based applications are often hosted on the cloud to take advantage of elasticity.

### 17. Cloud Disaster Recovery (DR)
*   **Concept:** Storing backups in the cloud to restore systems quickly after a failure.
*   **Benefits:** Lower cost than physical DR sites, faster recovery, and geographic redundancy (data is in a different city).

### 18. Data Challenges in Cloud
1.  **Data Segregation:** Keeping one customer's data separate from another.
2.  **Data Redundancy:** Managing multiple copies of data for safety without excessive cost.
3.  **Privacy:** Complying with international data protection laws.

### 19. SDLC for Cloud Applications
1.  **Requirement Analysis:** (Focus on cloud scale).
2.  **Design:** (Using Microservices).
3.  **Development:** (Using Cloud APIs).
4.  **Testing:** (Performance and security testing).
5.  **Deployment:** (Automated via DevOps).

### 20. Hypervisor (VMM)
*   **Definition:** A Virtual Machine Monitor is software that creates and runs virtual machines.
*   **Role:** It allows multiple operating systems to share the same physical hardware resources (CPU, RAM).
*   **Types:** Type 1 (runs on hardware) and Type 2 (runs on an OS).
