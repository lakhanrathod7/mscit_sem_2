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
*   **Definition:** Cloud computing is the on-demand delivery of IT resources (compute, storage, database) over the internet with pay-as-you-go pricing.
*   **Five Essential Characteristics (NIST):**
    1.  **On-demand Self-service:** Consumers can provision computing capabilities automatically without requiring human interaction with the service provider.
    2.  **Broad Network Access:** Services are available over the network and accessed through standard mechanisms (Mobiles, Tablets, Laptops).
    3.  **Resource Pooling:** The provider's computing resources are pooled to serve multiple consumers using a multi-tenant model (Physical/Virtual resources assigned dynamically).
    4.  **Rapid Elasticity:** Capabilities can be elastically provisioned and released to scale rapidly outward and inward commensurate with demand.
    5.  **Measured Service:** Cloud systems automatically control and optimize resource use by leveraging a metering capability (e.g., storage, processing, active user accounts).

### 2. GRID Computing
*   **Definition:** A processor architecture that combines computer resources from various administrative domains to reach a common goal. It is a type of distributed computing.
*   **Key Features:**
    1.  **Resource Sharing:** Sharing of compute power, storage, and data across a network.
    2.  **Coordination:** Coordinated use of heterogeneous resources.
    3.  **High Performance:** Targeted at massive scientific or technical problems (e.g., weather modeling).
*   **Cloud vs Grid:** Grids are typically decentralized and focused on specific high-performance tasks, whereas Clouds are centralized service-oriented platforms for a variety of general-purpose applications.

### 3. Cloud Service Models (SaaS, PaaS, IaaS)
*   **IaaS (Infrastructure as a Service):** Provides virtualized hardware resources (VMs, storage, networks). Users manage the OS, middleware, and applications. (Example: Amazon EC2).
*   **PaaS (Platform as a Service):** Provides a platform (runtime, tools) allowing customers to develop, run, and manage applications without the complexity of infrastructure management. (Example: Google App Engine).
*   **SaaS (Software as a Service):** Provides a complete software application over the internet. The provider manages everything from hardware to the app code. (Example: Salesforce, Gmail).
*   **Key Logic:** As you move from IaaS to SaaS, the provider's responsibility increases, and the user's management effort decreases.

### 4. Security as a Service (SecaaS)
*   **Definition:** An outsourcing model for security management where a provider integrates security services into a corporate infrastructure via the cloud.
*   **Benefits:**
    1.  **Cost Savings:** Eliminates the need for expensive on-premise hardware and specialized staff.
    2.  **Latest Protection:** Providers ensure tools are updated against the latest global threats in real-time.
    3.  **Skill Access:** Gives organizations access to high-level security professionals and specialized tools.
    4.  **Scalability:** Security services can grow instantly as the organization's data footprint expands.

### 5. Cloud Database (Relational vs NoSQL)
*   **Relational (SQL):** Uses structured tables and fixed schemas. Best for consistent, transactional data (e.g., AWS RDS, Azure SQL).
*   **NoSQL:** Handles unstructured or semi-structured data (Key-Value, Document, Graph). Best for massive scale and real-time big data (e.g., MongoDB, DynamoDB).
*   **Benefits:**
    1.  **Elasticity:** Scale storage and throughput up or down.
    2.  **Availability:** Managed replication across data centers.
    3.  **Management:** Automatic backups, patching, and failover provided by the cloud host.

### 6. Cloud Application Security Best Practices
1.  **Identity and Access Management (IAM):** Implement strong Multi-Factor Authentication (MFA) and follow the "Least Privilege" principle.
2.  **Data Encryption:** Encrypt data both "at rest" (in storage) and "in transit" (moving over the network).
3.  **API Security:** Use secure gateways, keys, and tokens to protect application interfaces from unauthorized access.
4.  **Vulnerability Management:** Perform regular scanning, penetration testing, and software patching.
5.  **Monitoring and Logging:** Maintain detailed logs to detect and respond to suspicious activities quickly.

### 7. DBaaS Architecture
*   **Definition:** Database-as-a-Service is a managed service providing database functionality without local hardware.
*   **Architecture Layers:**
    1.  **Service Layer:** The API/Console where users configure and request DB instances.
    2.  **Management Layer:** Handles automation of provisioning, scaling, backups, and security patching.
    3.  **Resource Layer (Physical):** The underlying servers, storage clusters, and hypervisors that host the database engines.
*   **Multi-tenancy:** Uses a shared infrastructure while ensuring logical data isolation between different customers.

### 8. Cloud Security Risk Analysis
*   **Definition:** The systematic process of identifying and evaluating potential threats to cloud-based assets.
*   **Key Steps:**
    1.  **Asset Identification:** Identifying sensitive data and critical services.
    2.  **Threat Assessment:** Identifying potential attackers (hackers, malicious insiders) and attack vectors (API vulnerabilities).
    3.  **Vulnerability Analysis:** Finding weaknesses in the cloud configuration or code.
    4.  **Impact Evaluation:** Estimating the financial and reputational damage of a breach.
*   **Mitigation Strategy:** Deciding whether to avoid, transfer, or mitigate the risk using technical controls.

### 9. Cloud Native vs Traditional Applications
*   **Traditional Applications:**
    *   **Monolithic:** Single large codebase.
    *   **Scale:** Hard to scale (must scale the entire app).
    *   **Infrastructure:** Dependent on specific OS/hardware configurations.
*   **Cloud Native Applications:**
    *   **Microservices:** Modular independent services.
    *   **Scale:** Granular scaling of specific features.
    *   **Agility:** Uses containers (Docker) and Orchestration (Kubernetes) to run consistently across any cloud.

### 10. Hybrid Cloud
*   **Definition:** A computing environment that combines a private cloud (on-premise) with a public cloud (e.g., AWS, Azure).
*   **Advantages:**
    1.  **Security:** Keep highly sensitive data on the private cloud.
    2.  **Flexibility:** Use the public cloud for less critical, high-volume tasks.
    3.  **Cloud Bursting:** Automatically move workloads to public cloud when the private cloud reaches its capacity.
    4.  **Cost:** Avoid over-provisioning private infrastructure for peak loads.

### 11. Cloud Service Brokerage (CSB)
*   **Definition:** An intermediary (business or software) that adds value to cloud services on behalf of users.
*   **Primary Roles:**
    1.  **Aggregation:** Combining multiple services into a single package.
    2.  **Integration:** Making different cloud services work together (Data movement).
    3.  **Customization:** Tailoring services to specific business needs.
    4.  **Arbitrage:** Finding the best price/performance across different providers.

### 12. Application vs Infrastructure Security
*   **Infrastructure Security:** Protecting the physical servers, storage, network, and hypervisor. In public clouds, this is mainly the **Provider's** responsibility.
*   **Application Security:** Protecting the software code, user input, APIs, and business logic. This is mainly the **Customer's** responsibility.
*   **Shared Responsibility Model:** A framework defining the boundary of security duties between the user and the cloud provider.

### 13. Client-Server vs Peer-to-Peer (P2P)
*   **Client-Server:** Centralized architecture where a powerful server provides resources to multiple clients. Highly secure and easy to manage (e.g., standard websites).
*   **Peer-to-Peer:** Decentralized architecture where every computer acts as both client and server. Highly resilient with no single point of failure (e.g., BitTorrent, Blockchain).
*   **Cloud Context:** Cloud is primarily an evolved Client-Server model where the "Server" is virtualized and globally distributed.

### 14. Cloud Application Requirements
1.  **Elastic Scalability:** Must handle fluctuating traffic automatically.
2.  **High Availability:** Design for "Design for Failure" (multi-zone deployment).
3.  **Stateless Design:** Individual requests should not depend on previous ones being on the same server.
4.  **API-First:** Built to interact easily with other services.
5.  **Multi-tenancy:** Efficiently serving multiple users from shared code/infrastructure.

### 15. Cloud Layered Architecture
*   **Layer 1: Hardware Layer:** Physical data centers and servers.
*   **Layer 2: Infrastructure Layer:** Virtualization (Hypervisors) creating VMs and storage.
*   **Layer 3: Platform Layer:** Operating systems, runtime libraries, and development tools.
*   **Layer 4: Application Layer:** The actual software (SaaS) accessed by users.
*   **Horizontal: Management Layer:** Overlooks all layers for billing, monitoring, and security.

### 16. SOA vs Cloud Computing
*   **SOA (Service Oriented Architecture):** A software design style where services are provided to components via communication protocols over a network.
*   **Cloud Computing:** A delivery model for IT resources.
*   **Comparison:** SOA is the **"blueprint"** for organizing software; Cloud is the **"factory"** that provides the infrastructure to run it. Many cloud apps are built using SOA principles.

### 17. Cloud Disaster Recovery (DR)
*   **Definition:** A strategy to restore data and apps after a catastrophic failure using cloud resources.
*   **Key Benefits:**
    1.  **Cost:** No need to maintain a physical secondary data center.
    2.  **Speed:** Fast recovery using "Pilot Light" or "Warm Standby" configurations.
    3.  **Reliability:** Data is replicated across distant geographical regions.

### 18. Data Challenges in Cloud
1.  **Data Segregation:** Risk of data leaking between tenants in a shared environment.
2.  **Redundancy management:** Balancing the cost of storage against the need for multiple copies.
3.  **Data Sovereignty:** Legal requirements for data to remain within a specific country's borders.
4.  **Vendor Lock-in:** Difficulty and cost of moving massive amounts of data from one provider to another.

### 19. SDLC for Cloud Applications
The process of developing software specifically for the cloud environment:
1.  **Assessment:** Evaluating if the app is suitable for the cloud.
2.  **Architecture:** Choosing Microservices or Serverless.
3.  **Cloud-Native Development:** Using cloud-specific APIs (S3, Lambda).
4.  **Testing:** Testing for elasticity and "chaos engineering" (how it handles server failures).
5.  **Continuous Deployment (CI/CD):** Automated updates without downtime.

### 20. Hypervisor (VMM)
*   **Definition:** Virtual Machine Monitor is software that creates and runs virtual machines.
*   **Types:**
    1.  **Type 1 (Bare Metal):** Runs directly on hardware (e.g., VMware ESXi). Best for performance.
    2.  **Type 2 (Hosted):** Runs on top of an OS (e.g., Oracle VirtualBox). Used for testing.
*   **Role:** It abstracts hardware (CPU, RAM) into multiple isolated virtual instances, allowing multi-tenancy and efficient resource use.
