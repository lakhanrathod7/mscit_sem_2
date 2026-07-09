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

### 1. Cloud Layered Architecture
*   **Definition:** Cloud computing is built on a layered architecture that allows for modularity and abstraction.
*   **Layers:**
    1.  **Hardware Layer (Datacenter):** The physical foundation (Servers, storage, power, cooling).
    2.  **Infrastructure Layer (IaaS):** Virtualized resources. It creates a pool of compute, storage, and network resources from the hardware.
    3.  **Platform Layer (PaaS):** Provides the operating system and development frameworks. It hides the complexity of infrastructure from developers.
    4.  **Application Layer (SaaS):** The top layer where the actual software applications reside. Users access this via the internet.
*   **Abstraction:** Each layer provides services to the layer above it, hiding the complexity below.

### 2. Cloud Computing Characteristics
*   **Elasticity:** The ability to scale resources up or down rapidly in response to demand.
*   **Scalability:** The capacity of the system to handle a growing amount of work by adding resources (Horizontal: more machines; Vertical: more power to one machine).
*   **Multi-tenancy:** Multiple customers (tenants) share the same physical infrastructure while their data is logically separated.
*   **On-Demand Self-Service:** Users can provision resources automatically without human interaction with the service provider.
*   **Broad Network Access:** Services are available over the internet via multiple devices (Desktop, Mobile).
*   **Resource Pooling:** The provider's resources are pooled to serve many consumers using a multi-tenant model.
*   **Measured Service (Pay-per-use):** Resource usage is monitored and billed based on actual consumption.

### 3. Cloud Service Models (SaaS, PaaS, IaaS)
*   **IaaS (Infrastructure as a Service):**
    *   *Definition:* Provides virtualized hardware.
    *   *Benefits:* Full control over OS and software; highly flexible.
    *   *Examples:* Amazon EC2, Google Compute Engine.
*   **PaaS (Platform as a Service):**
    *   *Definition:* Provides a platform for building and deploying apps.
    *   *Benefits:* Faster development; no need to manage servers or OS updates.
    *   *Examples:* Google App Engine, Heroku.
*   **SaaS (Software as a Service):**
    *   *Definition:* Software is licensed on a subscription basis.
    *   *Benefits:* No installation needed; accessible from anywhere; automatic updates.
    *   *Examples:* Salesforce, Google Workspace.

### 4. Cloud Deployment Models
*   **Public Cloud:** Services are provided over the public internet by third-party providers (AWS, Azure). *Advantage:* Low cost, no maintenance.
*   **Private Cloud:** Dedicated to a single organization. Can be on-premise or hosted. *Advantage:* High security and control.
*   **Hybrid Cloud:** Combines public and private clouds. *Advantage:* Flexibility to keep sensitive data on private cloud and scale using public cloud.
*   **Community Cloud:** Shared by organizations with common goals (e.g., government agencies). *Advantage:* Shared costs and common security standards.

### 5. DBaaS & Cloud Data Challenges
*   **DBaaS (Database as a Service):** A model where users can use a database without the need to set up hardware or install software.
*   **Architecture:** Consists of a service interface, an orchestration layer for management, and the underlying database instances.
*   **Challenges:**
    1.  **Security:** Risk of data breaches in a shared environment.
    2.  **Scalability:** Handling sudden spikes in database traffic.
    3.  **Data Integrity:** Ensuring consistency across redundant copies.
    4.  **Vendor Lock-in:** Difficulty in moving data to another provider.

### 6. Cloud Application Development & SDLC
*   **Requirements:** Scalability, High Availability, Fault Tolerance, and Multi-tenancy.
*   **SDLC Steps:**
    1.  **Planning & Analysis:** Assessing cloud readiness.
    2.  **Design:** Choosing a cloud-native architecture (like Microservices).
    3.  **Implementation:** Coding using cloud SDKs and APIs.
    4.  **Testing:** Testing for performance, security, and scalability.
    5.  **Deployment & Maintenance:** Using automated pipelines (DevOps).

### 7. Cloud Migration
*   **Definition:** Moving data, apps, or business processes from on-premise to the cloud.
*   **Challenges:** Data security during transfer, high initial cost, application incompatibility, and downtime.
*   **Best Practices:** Perform a pilot project, use automated tools, ensure data cleaning, and choose the right migration strategy (Rehost, Replatform, or Refactor).

### 8. SOA-based Cloud Applications
*   **Concept:** Building cloud apps using Service Oriented Architecture (SOA).
*   **Features:**
    1.  **Loose Coupling:** Services are independent.
    2.  **Reusability:** Services can be reused across different apps.
    3.  **Interoperability:** Services can communicate across different platforms.
*   **Benefit:** Enables high flexibility and easier maintenance of complex cloud systems.

### 9. Cloud Security Risk Analysis
*   **Risks:** Data breach, account hijacking, insecure APIs, and insider threats.
*   **Analysis:**
    1.  **Identify Assets:** What data needs protection?
    2.  **Identify Threats:** Who are the potential attackers?
    3.  **Vulnerability Analysis:** Where are the weaknesses in the system?
*   **Best Practices:** MFA, Encryption, regular audits, and the "Shared Responsibility Model".

### 10. Virtualization in Detail
*   **Definition:** Technology that allows creating multiple virtual machines on a single physical machine.
*   **Types:**
    1.  **Full Virtualization:** Guest OS is unaware of virtualization (e.g., VMware).
    2.  **Para-virtualization:** Guest OS is modified to communicate with the hypervisor (e.g., Xen).
    3.  **Hardware-Assisted:** Uses CPU features (Intel VT-x) to improve performance.
*   **Benefits:** Better resource utilization, isolation, and cost reduction.

### 11. GRID Computing vs Cloud
*   **Grid:** Distributed system for high-performance computing tasks. No centralized control.
*   **Cloud:** Centralized management providing on-demand services for business.
*   **Comparison:** Grid is for one big task; Cloud is for many different tasks for many users. Cloud is more user-friendly and commercially oriented.

### 12. Distributed, Grid, Cluster, and Cloud
*   **Distributed System:** Multiple computers working as one.
*   **Cluster:** Similar computers in one location connected by a fast LAN.
*   **Grid:** Heterogeneous resources across many locations.
*   **Cloud:** A commercial model for delivering computing as a utility.

### 13. Cloud Services Brokerage (CSB)
*   **Concept:** A business model where a third party manages multiple cloud services for a customer.
*   **Value:** It simplifies the complex cloud market for the user.
*   **Roles:** Aggregation (combining services), Arbitrage (finding the best price), and Customization.

### 14. Security as a Service (SecaaS)
*   **Definition:** Security capabilities delivered as a service (subscription).
*   **Features:** Email security, IAM, Intrusion Detection, and Identity Management.
*   **Benefits:** Lower cost, expert-level security, and automatic updates against new threats.

### 15. Cloud Application Security Best Practices
*   **Encryption:** Protecting data at rest and in motion.
*   **IAM:** Strong authentication and role-based access.
*   **API Security:** Protecting the gateways.
*   **Monitoring:** Continuous logging and real-time alerts.
*   **Compliance:** Ensuring data stays within legal boundaries.
