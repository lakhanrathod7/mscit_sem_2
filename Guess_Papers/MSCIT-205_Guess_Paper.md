# BAOU M.Sc. IT Semester 2 - Guess Paper (August 2026)
## MSCIT-205: Cloud Infrastructure and Services

**Time: 3 Hours | Max Marks: 70**

---

### Section A: Long Answer Questions (Attempt any 3 - 30 Marks)
1. Explain the Cloud Layered Architecture in detail. Discuss the roles of different layers.
2. Discuss the five essential characteristics of Cloud Computing as defined by NIST.
3. Explain Cloud Service Models (SaaS, PaaS, IaaS) with examples and target users.
4. Discuss the different Cloud Deployment Models: Public, Private, Hybrid, and Community Cloud.
5. What is Virtualization? Explain the role of the Hypervisor and the difference between Type-1 and Type-2 hypervisors.

---

### Section B: Short Answer Questions (Attempt any 4 - 20 Marks)
1. Compare Cloud Computing with Grid Computing.
2. What is DBaaS? Briefly explain its architecture.
3. Discuss the security risks and challenges associated with cloud computing.
4. Write a short note on Cloud Migration challenges and best practices.
5. Explain the role of Service Oriented Architecture (SOA) in cloud applications.
6. Differentiate between Vertical and Horizontal Scaling.

---

### Section C: Part A - MCQs (10 Marks)
1. NIST stands for:
   A. National Institute of Standards and Technology B. National Internet Service Team C. New International Science Terminal D. None
2. VMM stands for:
   A. Virtual Machine Mode B. Virtual Machine Monitor C. Virtual Management Mode D. None
3. Which model provides hardware infrastructure as a service?
   A. SaaS B. PaaS C. IaaS D. DBaaS
4. Google App Engine is an example of:
   A. IaaS B. PaaS C. SaaS D. None
5. Which feature refers to automatic scaling of resources?
   A. Multi-tenancy B. Resource pooling C. Rapid elasticity D. Measured service
6. Cloud type providing maximum control:
   A. Public B. Hybrid C. Private D. Community
7. Pay-as-you-go is a feature of:
   A. IaaS only B. PaaS only C. Cloud computing in general D. None
8. Hypervisor is also known as:
   A. Router B. VMM C. Switch D. VM
9. Which service allows developers to deploy apps without managing servers?
   A. IaaS B. PaaS C. SaaS D. DBaaS
10. SOA stands for:
    A. Service Oriented Architecture B. System Oriented Architecture C. Software Oriented Architecture D. None

---

### Section C: Part B - True or False (10 Marks)
1. Cloud computing reduces CAPEX.
2. Public cloud is more secure than private cloud.
3. SaaS hide all underlying infrastructure from the user.
4. Virtualization is the core technology of cloud computing.
5. SLA stands for Service Level Agreement.
6. Microservices are independent small services.
7. Cloud bursting is moving to a public cloud when private is full.
8. Multi-tenancy means sharing resources among many users.
9. Grid computing is the same as Cloud computing.
10. PaaS provides a development environment.

---
---

# TOPPER'S SOLUTIONS (DETAILED EXAM FORMAT)

## SECTION A: LONG ANSWERS (10 MARKS EACH)

### Q1. Cloud Layered Architecture
Cloud computing is built on a modular layered architecture where each layer provides specific services to the one above it.
1.  **Hardware Layer (Datacenter):** The foundation layer consisting of physical servers, storage (SAN/NAS), networking hardware (routers, switches), and power/cooling systems.
2.  **Infrastructure Layer (Virtualization):** This layer uses a Hypervisor to create a pool of virtual compute, storage, and network resources. It is the basis of IaaS.
3.  **Platform Layer:** Provides the OS, runtime environments (Java, Python), databases, and middleware. It allows developers to build apps without managing the underlying VMs.
4.  **Application Layer:** The topmost layer where end-user software (SaaS) resides, such as Gmail, Office 365, or Salesforce.
5.  **Management Layer:** A cross-cutting layer responsible for monitoring, billing, security policies, and resource metering across all other layers.

---

### Q2. NIST Essential Characteristics
The NIST standard defines five "must-have" characteristics for any cloud system:
1.  **On-demand Self-service:** Users can provision resources (like server time or storage) automatically via a web portal without human intervention from the provider.
2.  **Broad Network Access:** Services are accessible over the internet using standard protocols on any device (Mobiles, Tablets, Laptops).
3.  **Resource Pooling:** The provider's resources are pooled to serve multiple customers using a multi-tenant model. Physical resources are dynamically assigned to virtual ones based on demand.
4.  **Rapid Elasticity:** Resources can be scaled up or down instantly. To the user, it feels like the resources are unlimited and can be purchased in any quantity at any time.
5.  **Measured Service:** Cloud usage is metered (like electricity). Users are billed based on exact consumption, providing transparency for both provider and consumer.

---

### Q3. Cloud Service Models (SaaS, PaaS, IaaS)
1.  **IaaS (Infrastructure as a Service):**
    *   **What it provides:** Raw virtualized hardware (VMs, Storage, Networking).
    *   **User Responsibility:** OS, Middleware, Apps, Data.
    *   **User Type:** System Administrators.
    *   **Example:** Amazon EC2, Azure VMs.
2.  **PaaS (Platform as a Service):**
    *   **What it provides:** A platform for development (OS + Runtime + DB).
    *   **User Responsibility:** Application code and Data.
    *   **User Type:** Developers.
    *   **Example:** Google App Engine, Heroku.
3.  **SaaS (Software as a Service):**
    *   **What it provides:** A complete functional software application.
    *   **User Responsibility:** Using the software.
    *   **User Type:** End Users.
    *   **Example:** Gmail, Dropbox, Slack.

---

### Q4. Cloud Deployment Models
1.  **Public Cloud:** Owned and operated by third-party providers. Resources are shared by thousands of customers over the public internet. *Pros:* Low cost, no maintenance.
2.  **Private Cloud:** Used exclusively by one organization. It can be physically located on-site or hosted by a provider. *Pros:* Highest security and control.
3.  **Hybrid Cloud:** A mix of Public and Private clouds. Organizations keep sensitive data on private cloud and use public cloud for heavy workloads (Cloud Bursting).
4.  **Community Cloud:** Shared by several organizations with similar requirements (e.g., all government hospitals or all banks).

---

### Q5. Virtualization and Hypervisors
**Definition:** Virtualization is the process of creating a software-based (virtual) version of something, such as compute, storage, or network resources.
**Role of Hypervisor (VMM):** The Hypervisor is the software that makes virtualization possible. It sits between the hardware and the OS, partitioning the physical resources.
**Type-1 vs Type-2 Hypervisors:**
*   **Type-1 (Bare Metal):** Runs directly on the hardware. It is highly efficient and used in enterprise datacenters. *Example:* VMware ESXi, Microsoft Hyper-V.
*   **Type-2 (Hosted):** Runs as an application on an existing OS (like Windows). Used for testing and development. *Example:* Oracle VirtualBox, VMware Workstation.

---

## SECTION B: SHORT ANSWERS (5 MARKS EACH)

### Q1. Cloud vs Grid Computing
*   **Grid Computing:** A distributed system for one massive scientific task. It is decentralized (many owners) and usually uses idle CPU cycles.
*   **Cloud Computing:** A centralized service-oriented model for many small business tasks. It uses virtualization to provide dedicated resources on a pay-per-use basis.

### Q2. DBaaS (Database as a Service)
**Definition:** A managed service where the provider handles database installation, maintenance, and backups.
**Architecture:** It consists of a **Service Interface** (for user requests), an **Orchestration Layer** (for provisioning), and a **Database Instance Layer** (where data resides).

### Q3. Security Risks and Challenges
1.  **Data Breaches:** Unauthorized access to sensitive customer data.
2.  **Insecure APIs:** Weak interfaces that allow hackers to bypass security.
3.  **Multi-tenancy Risks:** Data "leakage" between different customers on the same physical server.
4.  **Data Loss:** Permanent loss of data due to provider failure or lack of backups.

### Q4. Cloud Migration
**Challenges:** High initial cost, application incompatibility, and downtime during transfer.
**Best Practices:** Perform a pilot project, use automated migration tools, and ensure data encryption during the move.

### Q5. Role of SOA in Cloud
**Service Oriented Architecture (SOA)** allows applications to be built as a collection of independent services. In the cloud, this modularity makes it easy to scale specific parts of an application independently.

### Q6. Vertical vs Horizontal Scaling
*   **Vertical (Scale Up):** Adding more RAM or CPU to a single existing server. *Limit:* Hardware capacity.
*   **Horizontal (Scale Out):** Adding more servers to the existing pool. *Limit:* Virtually unlimited.

---

## SECTION C: OBJECTIVE ANSWERS

### Part A: MCQs
1.  **NIST stands for:** A. National Institute of Standards and Technology
2.  **VMM stands for:** B. Virtual Machine Monitor
3.  **Which model provides hardware infrastructure?** C. IaaS
4.  **Google App Engine is an example of:** B. PaaS
5.  **Which feature refers to automatic scaling?** C. Rapid elasticity
6.  **Cloud type providing maximum control:** C. Private
7.  **Pay-as-you-go is a feature of:** C. Cloud computing in general
8.  **Hypervisor is also known as:** B. VMM
9.  **Which service allows developers to deploy apps without managing servers?** B. PaaS
10. **SOA stands for:** A. Service Oriented Architecture

### Part B: True or False
1.  **Cloud computing reduces CAPEX.** - **True** (Converts it to OPEX)
2.  **Public cloud is more secure than private cloud.** - **False** (Private is more secure)
3.  **SaaS hide all underlying infrastructure from the user.** - **True**
4.  **Virtualization is the core technology of cloud computing.** - **True**
5.  **SLA stands for Service Level Agreement.** - **True**
6.  **Microservices are independent small services.** - **True**
7.  **Cloud bursting is moving to a public cloud when private is full.** - **True**
8.  **Multi-tenancy means sharing resources among many users.** - **True**
9.  **Grid computing is the same as Cloud computing.** - **False**
10. **PaaS provides a development environment.** - **True**
