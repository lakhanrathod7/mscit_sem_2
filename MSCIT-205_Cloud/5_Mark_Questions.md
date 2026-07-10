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
*   **Definition:** Cloud computing is the on-demand delivery of IT resources over the internet.
*   **Five Essential Characteristics (NIST):**
    1.  **On-demand Self-service:** Users can provision computing resources (server time, network storage) automatically as needed without human interaction with the provider.
    2.  **Broad Network Access:** Services are available over the network and accessed through standard mechanisms (Mobile phones, Laptops).
    3.  **Resource Pooling:** The provider's computing resources are pooled to serve multiple consumers using a multi-tenant model.
    4.  **Rapid Elasticity:** Resources can be elastically provisioned and released to scale rapidly outward and inward with demand.
    5.  **Measured Service:** Cloud systems automatically control and optimize resource use by leveraging a metering capability (Pay-per-use).

### 2. GRID Computing
*   **Definition:** A processor architecture that combines computer resources from various domains to reach a main objective. It is a form of distributed computing.
*   **Key Features:**
    1.  **Distributed:** Resources are geographically dispersed and belong to different administrative domains.
    2.  **Heterogeneous:** Involves different types of computers and operating systems.
    3.  **Parallel Processing:** Complex tasks are broken down into smaller pieces and processed simultaneously.
*   **Comparison with Cloud:** Grids are focused on high-performance computing for a single task, while Clouds are focused on on-demand services for many users.

### 3. Cloud Service Models (SaaS, PaaS, IaaS)
*   **IaaS (Infrastructure as a Service):** Provides virtualized hardware resources (Servers, Storage, Networking). Users manage OS and apps. (e.g., AWS EC2).
*   **PaaS (Platform as a Service):** Provides a platform (OS, middleware, runtime) for developers to build and deploy apps without managing hardware. (e.g., Google App Engine).
*   **SaaS (Software as a Service):** Provides a complete software application over the internet. Users only use the app; the provider manages everything. (e.g., Gmail, Salesforce).

### 4. Security as a Service (SecaaS)
*   **Definition:** An outsourcing model for security management where a provider integrates security services into a corporate infrastructure.
*   **Benefits:**
    1.  **Cost Savings:** No need to invest in expensive on-premise security hardware and specialized staff.
    2.  **Constant Updates:** Security signatures and tools are updated in real-time by experts.
    3.  **Expertise:** Access to high-level security professionals and specialized tools.
    4.  **Scalability:** Security services can grow instantly as the organization expands.

### 5. Cloud Database (Relational vs NoSQL)
*   **Relational (SQL):** Structured data using tables. Best for transactional data requiring strict consistency. (e.g., AWS RDS, Azure SQL).
*   **NoSQL:** Unstructured or semi-structured data (Document, Key-Value, Graph). Best for big data, real-time web apps, and high scalability. (e.g., MongoDB, DynamoDB).
*   **Benefits:** High availability, automatic replication, automated backups, and the ability to scale storage and compute independently.

### 6. Cloud Application Security Best Practices
1.  **Identity and Access Management (IAM):** Use strong passwords and Multi-Factor Authentication (MFA).
2.  **Data Encryption:** Encrypt data "at rest" (in storage) and "in transit" (across the network).
3.  **Regular Audits:** Perform frequent vulnerability scanning and penetration testing.
4.  **API Security:** Ensure all application interfaces are authenticated and encrypted.
5.  **Secure DevOps:** Integrate security checks into the development lifecycle (DevSecOps).

### 7. DBaaS Architecture
*   **Definition:** Database-as-a-Service provides database functionality without the need for physical hardware setup.
*   **Architecture Layers:**
    1.  **Service Layer:** The API or Web Console where users request and configure database instances.
    2.  **Management Layer:** Handles the automation of provisioning, scaling, backups, and patching.
    3.  **Resource Layer:** The actual virtual machines and storage clusters that host the database engines.
*   **Core Concept:** The user manages the database *schema* and *data*, while the provider manages the *infrastructure* and *database software*.

### 8. Cloud Security Risk Analysis
*   **Definition:** Identifying and evaluating potential threats to cloud-based assets.
*   **Key Steps:**
    1.  **Asset Identification:** Knowing what data and services are in the cloud.
    2.  **Threat Assessment:** Identifying potential attackers (Hackers, Malicious Insiders).
    3.  **Vulnerability Analysis:** Finding weaknesses in the cloud configuration or APIs.
    4.  **Impact Analysis:** Determining the financial and operational damage if a breach occurs.
*   **Outcome:** A risk mitigation strategy (e.g., using better encryption or stricter IAM).

### 9. Cloud Native vs Traditional Applications
*   **Traditional Applications:**
    *   **Monolithic:** One large block of code.
    *   **Hard to Scale:** Must scale the whole app even if only one feature needs it.
    *   **Tied to Infrastructure:** Dependent on specific servers or OS.
*   **Cloud Native Applications:**
    *   **Microservices:** Many small, independent services.
    *   **Elastic Scaling:** Only the parts that need more power are scaled.
    *   **Containerized:** Uses Docker/Kubernetes to run anywhere.

### 10. Hybrid Cloud
*   **Definition:** A computing environment that combines a private cloud (on-premise) with a public cloud (like AWS/Azure).
*   **Advantages:**
    1.  **Security:** Highly sensitive data can be kept on the private cloud.
    2.  **Scalability:** Less critical applications can "burst" into the public cloud during peak traffic times.
    3.  **Cost Efficiency:** Organizations only pay for public cloud resources when they actually need extra capacity.

### 11. Cloud Service Brokerage (CSB)
*   **Definition:** An intermediary (business or software) that adds value to one or more cloud services on behalf of users.
*   **Primary Roles:**
    1.  **Aggregation:** Combining multiple services into a single package.
    2.  **Integration:** Making different cloud services work together.
    3.  **Customization:** Tailoring a public service to a specific client's needs.
    4.  **Arbitrage:** Finding the best price and performance from various providers.

### 12. Application vs Infrastructure Security
*   **Infrastructure Security:** Protecting the servers, storage, data center, and virtualization layer. In public clouds, this is mostly the **Provider's** responsibility.
*   **Application Security:** Protecting the software code, APIs, user sessions, and data inside the database. This is the **Customer's** responsibility.
*   **Shared Responsibility Model:** A framework defining who is responsible for what in a cloud environment.

### 13. Client-Server vs Peer-to-Peer
*   **Client-Server:** Centralized control. A dedicated server provides resources. High security and easy management. Used in Web hosting and Enterprise apps.
*   **Peer-to-Peer:** Decentralized. Every computer acts as both client and server. No central authority. Hard to secure but highly resilient (no single point of failure). Used in file sharing (BitTorrent).

### 14. Cloud Application Requirements
1.  **Scalability:** Must handle sudden growth in users.
2.  **High Availability:** Must be accessible 24/7 (uses multiple zones).
3.  **Fault Tolerance:** Must continue working even if one server fails.
4.  **Multi-tenancy:** Should be able to serve many customers from a single instance securely.
5.  **Interoperability:** Must connect with other cloud or on-premise systems via APIs.

### 15. Cloud Layered Architecture
*   **Hardware Layer:** Physical data center infrastructure.
*   **Infrastructure Layer:** Virtualization layer that creates VMs and storage.
*   **Platform Layer:** OS, libraries, and runtime environments for apps.
*   **Application Layer:** The actual software (SaaS) used by the end-user.
*   **Management Layer:** (Horizontal) Overlooks all layers for billing, security, and monitoring.

### 16. SOA vs Cloud Computing
*   **Similarities:** Both promote modularity, service reusability, and loose coupling.
*   **Differences:**
    *   **SOA (Service Oriented Architecture):** Is a design *philosophy* for organizing software components.
    *   **Cloud Computing:** Is a delivery *model* for computing resources (infrastructure).
*   **Integration:** You can build an SOA-based application and host it on the cloud to achieve better scalability.

### 17. Cloud Disaster Recovery (DR)
*   **Definition:** A strategy for restoring data and applications from the cloud after a catastrophic failure.
*   **Key Benefits:**
    1.  **Lower RTO (Recovery Time Objective):** Faster recovery than traditional tape backups.
    2.  **Geographic Redundancy:** Backups are stored in a different city or country.
    3.  **Cost Savings:** No need to maintain a secondary physical data center.

### 18. Data Challenges in Cloud
1.  **Data Segregation:** Ensuring one customer cannot see another customer's data in a multi-tenant environment.
2.  **Data Redundancy:** Keeping multiple copies for safety without blowing the budget.
3.  **Data Sovereignty:** Complying with laws that require data to stay within a specific country's borders.
4.  **Data Lock-in:** The difficulty in moving data from one provider to another.

### 19. SDLC for Cloud Applications
The Software Development Life Cycle for cloud has specific steps:
1.  **Feasibility Study:** Checking if the app can run on the cloud.
2.  **Design:** Choosing between microservices or serverless architecture.
3.  **Development:** Using cloud-specific APIs and SDKs.
4.  **Testing:** Testing for performance, security, and "cloud bursting" capability.
5.  **Deployment:** Using Continuous Integration/Continuous Deployment (CI/CD) tools.

### 20. Hypervisor (VMM)
*   **Definition:** Virtual Machine Monitor is a software layer that creates and runs virtual machines (VMs).
*   **Types:**
    1.  **Type 1 (Bare Metal):** Runs directly on hardware (e.g., VMware ESXi, Xen). Best performance.
    2.  **Type 2 (Hosted):** Runs on top of an OS (e.g., Oracle VirtualBox). Used for testing.
*   **Role:** It manages physical resources (CPU, RAM, Disk) and presents them as isolated virtual hardware to the guest OS.
