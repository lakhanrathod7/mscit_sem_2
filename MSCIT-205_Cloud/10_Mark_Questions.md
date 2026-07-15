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

### 1. Cloud Layered Architecture (Exhaustive)
**Introduction:** Cloud computing uses a modular layered architecture to provide services. Each layer abstracts the complexity of the one below it.

*   **Layer 1: Hardware/Datacenter Layer:**
    *   The physical foundation: Servers, storage devices, cooling systems, and power supplies.
    *   Cloud providers manage massive datacenters globally (e.g., AWS US-East-1).
*   **Layer 2: Infrastructure (Virtualization) Layer:**
    *   Uses Hypervisors (VMM) to partition physical hardware into Virtual Machines (VMs).
    *   Provides "Compute", "Storage", and "Networking" as a pool of resources.
    *   This is the basis for **IaaS**.
*   **Layer 3: Platform Layer:**
    *   Sits on top of Infrastructure. Provides OS, middleware, runtime environments, and databases.
    *   Allows developers to focus on code without worrying about server maintenance.
    *   This is the basis for **PaaS**.
*   **Layer 4: Application Layer:**
    *   The software that end-users interact with (e.g., Google Docs).
    *   Fully managed by the provider; users only need a web browser.
    *   This is the basis for **SaaS**.
*   **Layer 5: Management/Governance Layer (Horizontal):**
    *   Handles cross-cutting concerns: Billing, IAM (Security), Metering, Monitoring, and Service Level Agreements (SLAs).

---

### 2. Cloud Computing Characteristics (NIST Standard)
According to the National Institute of Standards and Technology (NIST), there are five essential characteristics:

1.  **On-demand Self-service:** A consumer can provision computing capabilities (server time, network storage) automatically as needed without human interaction with the provider.
2.  **Broad Network Access:** Capabilities are available over the network and accessed through standard mechanisms (Heterogeneous platforms like mobiles, laptops).
3.  **Resource Pooling:** Provider resources are pooled to serve multiple consumers using a **multi-tenant model**. Physical and virtual resources are dynamically assigned based on demand.
4.  **Rapid Elasticity:** Resources can be elastically provisioned and released (often automatically) to scale rapidly outward (up) and inward (down) commensurate with demand. To the user, resources appear unlimited.
5.  **Measured Service:** Cloud systems automatically control and optimize resource use by leveraging a metering capability (Pay-per-use). Usage is monitored, controlled, and reported for transparency.

---

### 3. Cloud Service Models (IaaS, PaaS, SaaS)
Cloud services are categorized based on what the provider manages vs. what the customer manages.

*   **IaaS (Infrastructure as a Service):**
    *   **Features:** Provides VMs, firewalls, and IP addresses. User installs OS and apps.
    *   **User:** System Administrators.
    *   **Example:** Amazon EC2, Microsoft Azure VMs.
*   **PaaS (Platform as a Service):**
    *   **Features:** Provides runtime (Java, PHP, Python), database, and web servers. User only manages code and data.
    *   **User:** Software Developers.
    *   **Example:** Google App Engine, Heroku, AWS Elastic Beanstalk.
*   **SaaS (Software as a Service):**
    *   **Features:** Complete application hosted by provider. No installation or maintenance needed by user.
    *   **User:** End Users (Business/General Public).
    *   **Example:** Salesforce, Gmail, Office 365, Dropbox.

---

### 4. Cloud Deployment Models
Describes the location and ownership of the cloud infrastructure.

1.  **Public Cloud:** Owned by a third-party provider (AWS). Available to the general public. *Pros:* Low cost, no maintenance. *Cons:* Less security control.
2.  **Private Cloud:** Used exclusively by one organization. Can be hosted on-site or off-site. *Pros:* High security and privacy. *Cons:* Expensive, high maintenance.
3.  **Hybrid Cloud:** A composition of public and private clouds. Data and apps can move between them. *Pros:* Best of both worlds (Security for sensitive data, Public cloud for volume).
4.  **Community Cloud:** Shared by several organizations with shared concerns (e.g., government agencies or healthcare).

---

### 5. DBaaS Architecture & Data Challenges
**DBaaS (Database as a Service)** allows users to use a database without managing the hardware or database software.

*   **Architecture Components:**
    1.  **Request Manager:** Handles API calls from users.
    2.  **Orchestrator:** Automates provisioning of DB instances and handles failover.
    3.  **Instance Manager:** Monitors individual DB instances for health and performance.
    4.  **Storage Engine:** The underlying persistent storage for the data.
*   **Challenges related to Cloud Data:**
    *   **Security:** Multi-tenancy risks (data isolation).
    *   **Data Integrity:** Ensuring data remains accurate across multiple replicas.
    *   **Latency:** Delay caused by geographical distance between user and data center.
    *   **Sovereignty:** Complying with laws that require data to stay in a specific country.

---

### 6. Cloud Application Development & SDLC
Designing cloud applications requires a shift from traditional software development.

*   **Key Requirements:**
    *   **Scalability:** Granular scaling of components.
    *   **Availability:** Design for "Anywhere, Anytime" access.
    *   **Multi-tenancy:** Serving many customers from one instance.
*   **Steps of Cloud SDLC:**
    1.  **Planning:** Assessing cloud suitability (Feasibility).
    2.  **Analysis:** Understanding resource requirements (Compute, Storage).
    3.  **Design:** Choosing architecture (Microservices vs. Serverless).
    4.  **Development:** Using cloud-native SDKs and APIs.
    5.  **Testing:** Testing for elasticity (Scale-up test) and security.
    6.  **Deployment:** Using CI/CD pipelines (DevOps).

---

### 7. Cloud Migration (Challenges & Best Practices)
**Definition:** Cloud migration is the process of moving data, applications, and IT processes from on-premise infrastructure to a cloud environment.

*   **Key Challenges:**
    1.  **Data Security:** Risk of data loss or breach during the transfer process.
    2.  **Application Compatibility:** Legacy applications may not be "cloud-ready" and might require code changes (Refactoring).
    3.  **Cost Management:** Initial migration costs and ongoing monthly operational expenses.
    4.  **Downtime:** Minimizing business disruption during the move.
*   **Migration Strategies (6 Rs):**
    1.  **Rehosting (Lift-and-Shift):** Moving apps as-is.
    2.  **Replatforming:** Making minor optimizations for the cloud.
    3.  **Refactoring:** Redesigning the app using cloud-native features.
    4.  **Repurchasing:** Moving to a different product (usually SaaS).
    5.  **Retiring:** Turning off unneeded apps.
    6.  **Retaining:** Keeping some apps on-premise for now.
*   **Best Practices:**
    *   Start with a Pilot project.
    *   Use automated migration tools (e.g., AWS Migration Hub).
    *   Prioritize data cleaning and governance before moving.

---

### 8. SOA Based Cloud Applications
**Service Oriented Architecture (SOA)** is a software design style where services are provided to application components through a communication protocol over a network.

*   **Core Characteristics:**
    1.  **Loose Coupling:** Services are independent; changing one doesn't break others.
    2.  **Reusability:** A single service can be used by multiple applications.
    3.  **Interoperability:** Services can communicate regardless of the language they are written in.
*   **SOA in Cloud:** Cloud computing provides the infrastructure to host SOA services efficiently.
    *   **Benefit:** Enables flexibility and scalability.
    *   **Relationship:** Most modern cloud applications are built using **Microservices**, which is an evolution of SOA.
    *   **Example:** A "Payment Gateway" service used by various e-commerce sites.

---

### 9. Cloud Security Risk Analysis & Best Practices
Security in the cloud is a **Shared Responsibility**.

*   **Security Risk Analysis Steps:**
    1.  **Asset Identification:** Identifying data, apps, and users.
    2.  **Threat Assessment:** Identifying potential attackers and attack vectors (e.g., SQL injection, DDoS).
    3.  **Vulnerability Scanning:** Finding weaknesses in cloud APIs or configurations.
    4.  **Impact Calculation:** Determining the financial/legal loss if a breach occurs.
*   **Best Practices for Cloud Application Security:**
    *   **IAM:** Strong passwords and Multi-factor Authentication.
    *   **Encryption:** Using AES-256 for data at rest and TLS for data in transit.
    *   **API Gateways:** Protecting the entry points of the application.
    *   **Monitoring:** Continuous logging (e.g., AWS CloudTrail).

---

### 10. Virtualization: Full, Para, and Hardware-Assisted
Virtualization is the foundation of cloud computing.

1.  **Full Virtualization:** The guest OS is unaware it is being virtualized. It needs no modification. The hypervisor intercepts every hardware call. (e.g., VMware ESXi).
2.  **Para-virtualization:** The guest OS is modified to communicate directly with the hypervisor. It is more efficient than full virtualization. (e.g., Xen).
3.  **Hardware-Assisted Virtualization:** Uses specific CPU features (Intel VT-x or AMD-V) to handle virtualization tasks in hardware, reducing the hypervisor's load.
*   **Benefits:** Better resource utilization, isolation of environments, and environment snapshots (Backups).

---

### 11. GRID Computing & Comparison with Cloud
**GRID Computing** is a processor architecture that combines computer resources from various domains to reach a common goal.

*   **Key Features of GRID:**
    1.  **Distributed:** Resources are geographically dispersed.
    2.  **Loose Coupling:** Machines are not necessarily identical.
    3.  **High Performance:** Targeted at massive scientific problems (e.g., SETI@home).
*   **GRID vs. Cloud Computing:**
    *   **Goal:** Grid is for one big task; Cloud is for many small business tasks.
    *   **Control:** Grid is decentralized; Cloud is centralized (Provider controlled).
    *   **Billing:** Grid is often free/academic; Cloud is pay-per-use.
    *   **Abstraction:** Cloud uses virtualization extensively; Grid focuses on job scheduling.

---

### 12. Distributed, Grid, Cluster, and Cloud (Comparison)
| Feature | Distributed System | Cluster Computing | Grid Computing | Cloud Computing |
| :--- | :--- | :--- | :--- | :--- |
| **Control** | Decentralized | Centralized | Decentralized | Centralized (Provider) |
| **Resources** | Heterogeneous | Homogeneous | Heterogeneous | Homogeneous (Virtual) |
| **Goal** | Task execution | High Performance | Large Scale Science | General Business Services |
| **Model** | Loose coupling | Tight coupling | Loose coupling | Virtualization based |
| **Example** | Internet | Supercomputers | SETI@home | AWS, Azure |

---

### 13. Cloud Services Brokerage (CSB)
**Definition:** A CSB is an intermediary that adds value to one or more cloud services on behalf of users.

*   **Primary Roles of a Broker:**
    1.  **Aggregation:** Combining multiple services into one interface (e.g., a single login for AWS, Azure, and Google Cloud).
    2.  **Integration:** Making different cloud services work together (e.g., moving data from a SaaS app to an IaaS database).
    3.  **Customization:** Altering a public cloud service to meet specific user requirements.
*   **Value Proposition:** Simplifies cloud management, optimizes costs, and improves security for the end-user.

---

### 14. Security as a Service (SecaaS)
SecaaS is an outsourcing model where a provider handles the security functions of an organization.

*   **Key Features:**
    1.  **Identity Management:** Managing who can log in to what.
    2.  **Continuous Monitoring:** Real-time threat detection.
    3.  **Intrusion Detection (IDS/IPS):** Monitoring network traffic for malicious behavior.
    4.  **Email Security:** Filtering spam and malware.
*   **Benefits:**
    *   **Financial:** Low CAPEX (no hardware to buy).
    *   **Expertise:** Access to world-class security professionals.
    *   **Updates:** Constant signature updates for the latest viruses.

---

### 15. Cloud Application Security Best Practices
Detailed security checklist for developers:
1.  **Shared Responsibility:** Understand what you manage vs. what the provider manages.
2.  **Principle of Least Privilege:** Grant only necessary access to users and services.
3.  **Data-in-Transit Encryption:** Always use HTTPS/TLS.
4.  **Data-at-Rest Encryption:** Encrypt volumes and buckets (S3).
5.  **Multi-Factor Authentication (MFA):** Essential for all administrative accounts.
6.  **Patch Management:** Keep OS and libraries updated.
7.  **Serverless Security:** Monitor function permissions and execution times.
