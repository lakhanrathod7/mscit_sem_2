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
Cloud computing is structured into layers to provide abstraction and modularity.

1.  **Hardware Layer (Datacenter):** The foundation consisting of physical servers, storage, and networking hardware.
2.  **Infrastructure Layer (IaaS):** Uses virtualization to pool hardware resources and create Virtual Machines (VMs).
3.  **Platform Layer (PaaS):** Provides OS, databases, and application frameworks. It abstracts server management.
4.  **Application Layer (SaaS):** The top layer where end-user software (like Gmail) resides.
5.  **Management Layer (Cross-cutting):** Handles billing, security policies, and resource monitoring across all layers.

---

### Q2. NIST Essential Characteristics
1.  **On-demand Self-service:** Users can provision resources (like CPU time) automatically without calling the provider.
2.  **Broad Network Access:** Services are available via the internet on any device (Mobile, Laptop).
3.  **Resource Pooling:** Multiple customers share the same physical hardware via a multi-tenant model.
4.  **Rapid Elasticity:** Resources can be scaled up or down instantly based on demand.
5.  **Measured Service (Pay-per-use):** Resource usage is monitored and billed based on actual consumption.

---

### Q3. Cloud Service Models
*   **IaaS (Infrastructure):** Provides virtualized hardware. *User:* System Admins. *Ex:* AWS EC2.
*   **PaaS (Platform):** Provides a platform for building/testing apps. *User:* Developers. *Ex:* Google App Engine.
*   **SaaS (Software):** Provides a complete application. *User:* End Users. *Ex:* Salesforce, Dropbox.

---

### Q5. Virtualization and Hypervisors
**Definition:**
Virtualization is the technology that creates a software-based (virtual) version of something, such as computing, storage, or networking.

**Role of Hypervisor (VMM):**
The Hypervisor is a software layer that manages and runs virtual machines. It partitions the physical hardware among multiple guest OSs.

**Type-1 vs Type-2 Hypervisors:**
*   **Type-1 (Bare Metal):** Runs directly on the physical hardware. Highly efficient. Use Case: Enterprise data centers (e.g., VMware ESXi).
*   **Type-2 (Hosted):** Runs on top of an existing Operating System. Primarily used for testing/development. (e.g., Oracle VirtualBox).

---

## SECTION B: SHORT ANSWERS (5 MARKS EACH)

### Q1. Cloud vs Grid Computing
*   **Control:** Grid is decentralized (many owners); Cloud is centralized (one provider).
*   **Purpose:** Grid is for one massive task (Scientific); Cloud is for many small tasks (Business).
*   **Billing:** Grid is usually free for research; Cloud is pay-per-use.

### Q6. Vertical vs Horizontal Scaling
*   **Vertical (Scale Up):** Adding more power (CPU, RAM) to a single existing server. *Limit:* Hardware maximum.
*   **Horizontal (Scale Out):** Adding more servers to the existing pool. *Limit:* Theoretically unlimited.

---

## SECTION C: OBJECTIVE ANSWERS

### Part A: MCQs
1.  **A.** National Institute of Standards and Technology
2.  **B.** Virtual Machine Monitor
3.  **C.** IaaS
4.  **B.** PaaS
5.  **C.** Rapid elasticity
6.  **C.** Private
7.  **C.** Cloud computing in general
8.  **B.** VMM
9.  **B.** PaaS
10. **A.** Service Oriented Architecture

### Part B: True or False
1.  **True**
2.  **False** (Private is more secure)
3.  **True**
4.  **True**
5.  **True**
6.  **True**
7.  **True**
8.  **True**
9.  **False**
10. **True**
