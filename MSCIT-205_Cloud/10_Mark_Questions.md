# MSCIT-205: Cloud Infrastructure and Services
## 10-Mark Questions (Important for Exam)

1.  **⭐⭐⭐ Cloud Layered Architecture:** Explain Cloud Computing Layers / Layered Architecture in detail. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
2.  **⭐⭐⭐ Cloud Computing Characteristics:** Explain different characteristics of cloud computing (Elasticity, Scalability, Multi-tenancy, etc.). (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
3.  **⭐⭐⭐ Cloud Service Models:** Explain Service Models (SaaS, PaaS, IaaS) in detail. Discuss benefits and features of each. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
4.  **⭐⭐⭐ Types of Cloud / Deployment Models:** Explain types of cloud (Public, Private, Hybrid, Community). Discuss their advantages. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
5.  **⭐⭐⭐ DBaaS & Cloud Data:** What is DBaaS? Explain its architecture. Discuss challenges related to cloud data. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
6.  **⭐⭐⭐ Cloud Application Development:** Explain cloud application requirements and the SDLC steps involved in cloud application software development. (Repeated: Aug 2022, July 2023, July 2025)
7.  **⭐⭐⭐ Cloud Migration:** What is cloud migration? Discuss the challenges and best practices to ensure smooth migration. (Repeated: July 2025)
8.  **⭐⭐⭐ SOA based Cloud Applications:** Write a short note on Service Oriented Architecture (SOA) based cloud applications. (Repeated: July 2023, July 2025)
9.  **⭐⭐⭐ Cloud Security:** Explain Cloud Security risks, issues, and security risk analysis. Discuss best practices for cloud application security. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
10. **⭐⭐ Virtualization:** Explain virtualization in detail. Discuss Full, Para, and Hardware-assisted virtualization. (Repeated: July 2023, July 2025)
11. **⭐⭐ Grid Computing:** Write a short note on GRID Computing and its comparison with Cloud. (Repeated: Aug 2022, July 2025)
12. **⭐⭐ Distributed vs Grid vs Cluster vs Cloud:** Compare distributed systems, grid computing, cluster computing, and cloud computing with examples. (Repeated: July 2025)
13. **⭐⭐ Cloud Services Brokerage (CSB):** Discuss in brief about Cloud Services Brokerage (CSB). (Repeated: July 2023, July 2025)
14. **⭐⭐ Security as a Service (SecaaS):** Explain the benefits and features of Security as a Service. (Repeated: Aug 2022, July 2025)
15. **⭐⭐ Cloud Application Security Best Practices:** Discuss best practices for securing cloud applications. (Repeated: Aug 2022, July 2023)

---

## Detailed Answers (10-Mark Questions)

### 1. Cloud Layered Architecture (In-Depth)
Cloud computing follows a hierarchical structure to provide services. This architecture is composed of five distinct layers:

1.  **Hardware Layer (Datacenter Layer):** The bottom layer consisting of physical servers, storage, cooling systems, and power supplies. It is the physical foundation of the cloud.
2.  **Infrastructure Layer (IaaS Layer):** Uses virtualization to create a pool of compute, storage, and network resources from the physical hardware. It manages the virtual machines (VMs).
3.  **Platform Layer (PaaS Layer):** Sits on top of infrastructure and provides operating systems, databases, and application frameworks. It abstracts the server management from the developers.
4.  **Application Layer (SaaS Layer):** The topmost layer where actual software applications run. Users access these applications via the internet using web browsers.
5.  **Management Layer (Cross-cutting):** This layer overlooks all other layers. It is responsible for billing, user management, security policies, and resource monitoring across the entire stack.

### 2. Cloud Computing Characteristics
The NIST definition specifies five essential characteristics of cloud computing:

*   **1. On-demand Self-service:** A consumer can unilaterally provision computing capabilities, such as server time and network storage, as needed automatically without requiring human interaction with each service provider.
*   **2. Broad Network Access:** Capabilities are available over the network and accessed through standard mechanisms that promote use by heterogeneous thin or thick client platforms (e.g., mobile phones, tablets, laptops).
*   **3. Resource Pooling:** The provider's computing resources are pooled to serve multiple consumers using a multi-tenant model. Resources like storage, processing, and memory are dynamically assigned according to demand.
*   **4. Rapid Elasticity:** Capabilities can be elastically provisioned and released, in some cases automatically, to scale rapidly outward and inward commensurate with demand. To the consumer, the resources available for provisioning often appear to be unlimited.
*   **5. Measured Service:** Cloud systems automatically control and optimize resource use by leveraging a metering capability (e.g., storage, processing, bandwidth, and active user accounts). Resource usage can be monitored, controlled, and reported, providing transparency for both the provider and consumer of the utilized service.

### 3. Cloud Service Models (SaaS, PaaS, IaaS)
*   **Infrastructure as a Service (IaaS):**
    *   *Features:* Provides fundamental computing resources. Users can install any OS or software.
    *   *Benefits:* Highest level of flexibility and control over infrastructure.
    *   *Example:* Amazon EC2, Microsoft Azure VMs.
*   **Platform as a Service (PaaS):**
    *   *Features:* Provides a platform for developers to develop, test, and manage applications without the complexity of building and maintaining infrastructure.
    *   *Benefits:* Faster development cycles; reduces management overhead.
    *   *Example:* Google App Engine, Heroku.
*   **Software as a Service (SaaS):**
    *   *Features:* Applications are hosted by a provider and made available to customers over a network.
    *   *Benefits:* No installation or maintenance needed by the user; accessible from anywhere.
    *   *Example:* Microsoft 365, Salesforce, Gmail.

### 4. Cloud Deployment Models
Cloud deployment models define the location and management of the cloud infrastructure.

*   **Public Cloud:** The cloud infrastructure is made available to the general public or a large industry group and is owned by an organization selling cloud services. *Benefit:* Low cost (Pay-per-use) and high scalability.
*   **Private Cloud:** The cloud infrastructure is operated solely for a single organization. It may be managed by the organization or a third party and may exist on-premise or off-premise. *Benefit:* Highest security and privacy.
*   **Hybrid Cloud:** The cloud infrastructure is a composition of two or more clouds (private, community, or public) that remain unique entities but are bound together by standardized technology. *Benefit:* Best of both worlds—keep sensitive data private and scale on public cloud.
*   **Community Cloud:** The infrastructure is shared by several organizations and supports a specific community that has shared concerns (e.g., security, compliance).

### 5. DBaaS Architecture & Data Challenges
**Database as a Service (DBaaS)** is a managed service that allows users to use a database without physical hardware or software setup.

*   **Architecture Components:**
    1.  **Service Interface:** The UI or API used for configuration.
    2.  **Orchestration Layer:** Automates the provisioning of DB instances, scaling, and failover.
    3.  **Database Instance:** The actual database (MySQL, PostgreSQL, NoSQL).
    4.  **Shared Storage:** Where the physical data files reside.
*   **Cloud Data Challenges:**
    *   **Data Segregation:** Ensuring that data from different tenants in a multi-tenant environment is logically separated.
    *   **Latency:** The delay in accessing data stored in remote cloud data centers.
    *   **Data Redundancy:** Managing multiple copies of data for safety without excessive cost.
    *   **Security & Privacy:** Complying with global regulations (GDPR, HIPAA) while data is stored in different countries.

### 6. Cloud Application Development & SDLC
Designing cloud applications requires a different mindset than traditional apps.

*   **Requirements:** Scalability, High Availability (HA), Multi-tenancy, and Security.
*   **SDLC Steps for Cloud:**
    1.  **Planning:** Assessing which parts of the application should be on cloud.
    2.  **Analysis:** Understanding the resource requirements (CPU, RAM, Bandwidth).
    3.  **Design:** Choosing a microservices-based architecture to allow independent scaling of features.
    4.  **Development:** Writing code using cloud-native APIs (like AWS Lambda or S3).
    5.  **Testing:** Testing for elasticity (Does it scale up during heavy load?) and security.
    6.  **Deployment:** Using DevOps pipelines for automated, zero-downtime releases.

### 7. Cloud Migration: Challenges & Best Practices
**Cloud Migration** is the process of moving an organization's data, applications, and IT processes from on-premise servers to the cloud.

*   **Challenges:**
    1.  **Data Security:** Protecting sensitive data during the transfer.
    2.  **Cost Management:** Initial migration costs and ongoing monthly bills.
    3.  **Application Incompatibility:** Older "legacy" apps may not run on modern cloud platforms.
    4.  **Downtime:** Keeping the business running during the move.
*   **Best Practices:**
    1.  **Assessment:** Audit existing resources and prioritize what to move first.
    2.  **Strategy:** Choose a method (Rehosting, Replatforming, or Refactoring).
    3.  **Pilot Project:** Move a small, non-critical application first to learn the process.
    4.  **Automation:** Use specialized tools (like AWS Migration Hub) to reduce manual errors.

### 8. SOA-Based Cloud Applications
**Service-Oriented Architecture (SOA)** is a software design style where services are provided to other components by application components through a communication protocol over a network.

*   **Core Concepts:**
    1.  **Loose Coupling:** Services are independent. Changes in one service do not break another.
    2.  **Interoperability:** Services can communicate across different languages and platforms.
    3.  **Reusability:** A single service (like a "Payment Gateway") can be reused by multiple applications.
*   **SOA in Cloud:** SOA provides the blueprint for building modular applications, while Cloud provides the elastic infrastructure to run them. Most modern SaaS applications are built using SOA principles.

### 9. Cloud Security Risk Analysis & Best Practices
Security is the top concern for cloud users.

*   **Risks:** Data breach, account hijacking, insecure APIs, and "insider threats" (disgruntled employees of the provider).
*   **Security Risk Analysis Steps:**
    1.  **Identify Assets:** What data are we storing?
    2.  **Identify Threats:** Who could attack us?
    3.  **Vulnerability Scanning:** Where are the holes in our defense?
    4.  **Impact Evaluation:** What happens if we are hacked?
*   **Best Practices:**
    *   **MFA:** Mandatory Multi-Factor Authentication for all users.
    *   **Encryption:** Encrypt data at rest and in motion.
    *   **Principle of Least Privilege:** Give users only the access they need to do their jobs.
    *   **Logging:** Record every action taken in the cloud environment.

### 10. Virtualization: Types & Benefits
Virtualization is the core technology that enables cloud computing by allowing multiple operating systems to run on a single physical machine.

*   **Types of Virtualization:**
    1.  **Full Virtualization:** The guest OS is completely isolated and is unaware it is running in a virtual environment. It requires no modification (e.g., VMware).
    2.  **Para-virtualization:** The guest OS is modified to communicate with the hypervisor, improving efficiency (e.g., Xen).
    3.  **Hardware-assisted Virtualization:** Uses special CPU instructions (Intel VT-x) to handle virtualization tasks directly in hardware.
*   **Benefits:** Better resource utilization, reduced hardware costs, easier backups (snapshots), and environment isolation.

### 11. GRID Computing & Comparison with Cloud
**Grid Computing** is a processor architecture that combines computer resources from various domains to reach a main objective.

*   **Grid vs. Cloud Comparison:**
    1.  **Control:** Grid is usually decentralized (many owners); Cloud is centralized (one provider).
    2.  **Goal:** Grid is for one massive calculation (Scientific); Cloud is for many small tasks (Business).
    3.  **Billing:** Grid is often free for researchers; Cloud is pay-per-use.
    4.  **Interface:** Grid uses command-line tools; Cloud uses user-friendly web consoles.

### 12. Distributed, Cluster, Grid, and Cloud
1.  **Distributed System:** A collection of independent computers that appear to the user as a single coherent system.
2.  **Cluster Computing:** A group of similar computers connected by a high-speed LAN to work as a single unit (e.g., Beowulf cluster).
3.  **Grid Computing:** A distributed system that coordinates heterogeneous resources across different geographical locations.
4.  **Cloud Computing:** A model for enabling convenient, on-demand network access to a shared pool of configurable computing resources.

### 13. Cloud Services Brokerage (CSB)
A **Cloud Service Brokerage** is an IT role and business model in which a company or other entity adds value to one or more cloud services on behalf of users of those services.

*   **Three Main Roles:**
    1.  **Aggregation:** Combining multiple services into one or more new services.
    2.  **Integration:** Making a public cloud service work with an organization's existing on-premise software.
    3.  **Customization:** Altering a public cloud service to meet the specific security or performance needs of a client.

### 14. Security as a Service (SecaaS)
SecaaS is a business model in which a large service provider integrates their security services into a corporate infrastructure on a subscription basis.

*   **Key Features:**
    1.  **Identity Management:** Managing user logins and permissions.
    2.  **Intrusion Detection:** Monitoring traffic for signs of a hack.
    3.  **Email Security:** Filtering spam and malware.
    4.  **Vulnerability Scanning:** Automatically checking for weaknesses.
*   **Benefits:** Lower cost of ownership, up-to-date protection, and specialized expertise.

### 15. Cloud Application Security Best Practices
1.  **Adopt a Zero Trust Model:** Never trust anyone inside or outside the network; verify everything.
2.  **Data Masking:** Hiding sensitive parts of data (like credit card numbers) from unauthorized viewers.
3.  **API Gateway Security:** Protect the "front door" of your application.
4.  **Automated Security Testing:** Integrate security tools into the CI/CD pipeline.
5.  **Regular Compliance Checks:** Ensure the cloud setup meets industry standards (like ISO 27001).
