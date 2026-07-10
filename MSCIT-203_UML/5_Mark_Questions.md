# MSCIT-203: Object Oriented Analysis and Design using UML
## 5-Mark Questions (Short Notes)

1.  **⭐⭐⭐ Sequence Diagram Notations:** List and explain any 5 Sequence Diagram notations in detail. (Repeated: July 2025)
2.  **⭐⭐⭐ Interaction Diagrams:** Discuss a brief about Interaction Diagrams and common terms/symbols used. (Repeated: July 2025, July 2023)
3.  **⭐⭐⭐ Creational Patterns:** Explain creational patterns in brief with examples. (Repeated: Jan 2023, July 2023)
4.  **⭐⭐⭐ OOAD vs Structured Approach:** Differentiate between the Structured and Object-Oriented approach. (Repeated: July 2023)
5.  **⭐⭐⭐ Use Case Diagram:** Explain Use Case diagrams with an example. (Repeated: Aug 2022, July 2025)
6.  **⭐⭐⭐ Design Patterns Elements:** Explain four important elements while describing a design pattern (Name, Problem, Solution, Consequences). (Repeated: July 2023)
7.  **⭐⭐⭐ WebE Design Pyramid:** Explain the four layers of the OO design pyramid / WebE Design Pyramid. (Repeated: Aug 2022, Jan 2023)
8.  **⭐⭐⭐ UML Modelling Tools:** Explain UML Modelling Tools in brief. (Repeated: Aug 2022, Jan 2023)
9.  **⭐⭐⭐ OOA Process:** List and explain generic components of the object-oriented analysis model. (Repeated: July 2025)
10. **⭐⭐⭐ Object Design Process:** Write a short note on the Object Design Process. (Repeated: July 2025)
11. **⭐⭐ Behavioral Patterns:** Write a detailed note on Behavioral Patterns. (Repeated: Aug 2022)
12. **⭐⭐ Web-Based System Attributes:** List and explain attributes of web-based systems and applications. (Repeated: Aug 2022, July 2023)
13. **⭐⭐ UML Goals:** What is UML? Explain the goals of UML. (Repeated: Aug 2022)
14. **⭐⭐ SE vs WebE:** Give a comparison between Software Engineering and Web Engineering. (Repeated: Aug 2022)
15. **⭐⭐ OOD Steps:** Write steps of Object-Oriented Design. (Repeated: Aug 2022)
16. **⭐⭐ Interaction Diagram Types:** List types of interaction diagrams in UML. (Repeated: Aug 2022, Jan 2023)
17. **⭐⭐ Object Relationship Model:** Define the Object Relationship Model. (Repeated: Jan 2023, July 2023)
18. **⭐⭐ Requirement Analysis for WebApps:** Explain the requirement analysis for WebApps. (Repeated: Jan 2023)
19. **⭐⭐ Activity Diagram:** Write a short note on Activity Diagrams. (Repeated: Jan 2023)
20. **⭐⭐ Message Categories:** Describe different categories of messages in brief. (Repeated: July 2023)

---

## Detailed Answers (5-Mark Questions)

### 1. Sequence Diagram Notations
*   **Definition:** A Sequence Diagram is a type of interaction diagram that shows how objects operate with one another and in what order. It is a construct of a message sequence chart.
*   **Key Notations:**
    1.  **Actor:** Represented by a stick figure. It is an external entity (Human or System) that interacts with the system to achieve a goal.
    2.  **Lifeline:** A vertical dashed line that represents the existence of an object over a period of time.
    3.  **Activation Bar:** A thin vertical rectangle placed on the lifeline. It indicates that an object is currently performing an operation or is active.
    4.  **Synchronous Message:** A solid horizontal line with a filled arrowhead. It means the sender waits for a response from the receiver before continuing.
    5.  **Return Message:** A horizontal dashed line with an open arrowhead. It represents the data or confirmation being sent back to the original caller.
    6.  **Object Instance:** A box with the name of the object and class (e.g., `myOrder : Order`), always underlined.

### 2. Interaction Diagrams (Common Terms)
*   **Definition:** Interaction diagrams are used to model the dynamic behavior of a system by showing how a group of objects collaborate to perform a specific task.
*   **Common Terms & Symbols:**
    1.  **Object:** Instances of classes involved in the interaction.
    2.  **Link:** A relationship between objects that allows messages to flow. In communication diagrams, links are solid lines.
    3.  **Message Arrow:** Indicates the direction of the call and often includes a sequence number (e.g., `1.1: validate()`) to show the order of execution.
    4.  **Guard Condition:** A boolean expression in brackets `[condition]` that must be true for the message to be sent.
    5.  **Self-Message:** When an object invokes one of its own methods.
    6.  **Frame:** A box surrounding the diagram or a part of it, used to show loops (`loop`) or alternatives (`alt`).

### 3. Creational Design Patterns
*   **Definition:** Creational patterns provide various object creation mechanisms, which increase flexibility and reuse of existing code. They help make a system independent of how its objects are created, composed, and represented.
*   **Examples:**
    1.  **Singleton:** Ensures that a class has only one instance and provides a global point of access to it (e.g., a shared Database connection).
    2.  **Factory Method:** Defines an interface for creating an object but lets subclasses decide which class to instantiate.
    3.  **Abstract Factory:** Provides an interface for creating families of related or dependent objects without specifying their concrete classes.
    4.  **Builder:** Used to construct a complex object step by step. It separates the construction process from the final representation.
    5.  **Prototype:** Allows creating new objects by cloning/copying an existing object.

### 4. OOAD vs Structured Approach
*   **Structured Approach (Traditional):**
    *   **Focus:** It is **process-centric**. It decomposes the system based on functions or processes.
    *   **Components:** Data and logic (functions) are separate.
    *   **Tools:** Uses Data Flow Diagrams (DFD) and Entity-Relationship Diagrams (ERD).
    *   **Scale:** Good for small, stable systems but difficult to maintain for large, complex applications.
*   **Object-Oriented (OOAD):**
    *   **Focus:** It is **data-centric**. It identifies objects that combine both data and behavior.
    *   **Components:** Uses Encapsulation to bundle data and methods together.
    *   **Tools:** Uses UML diagrams (Class, Use Case, Sequence).
    *   **Scale:** Highly modular, promotes code reusability, and is better suited for evolving software projects.

### 5. Use Case Diagram with Example
*   **Definition:** A Use Case Diagram describes a set of actions (use cases) that some system or systems (subject) should or can perform in collaboration with one or more external users (actors).
*   **Components:** Actors (Stick figures), Use Cases (Ovals), and Relationships (Associations).
*   **Example: ATM System**
    *   **Actor:** Customer, Bank Technician.
    *   **Use Cases:** Withdraw Cash, Check Balance, Change PIN, Repair Machine.
    *   **Relationships:** "Withdraw Cash" might have an `<<include>>` relationship with "Validate User", meaning validation is a mandatory part of every withdrawal.

### 6. Design Pattern Elements
According to Gamma et al., a design pattern has four essential elements:
1.  **Pattern Name:** A handle we can use to describe a design problem, its solutions, and consequences in a word or two. It increases our design vocabulary.
2.  **Problem:** Describes when to apply the pattern. It explains the problem and its context.
3.  **Solution:** Describes the elements that make up the design, their relationships, responsibilities, and collaborations. It is a general template, not a concrete implementation.
4.  **Consequences:** The results and trade-offs of applying the pattern. They are critical for evaluating design alternatives and for understanding the costs and benefits of applying the pattern.

### 7. WebE Design Pyramid (Layers)
Web Engineering (WebE) uses a design pyramid to organize the design tasks into six specific layers:
1.  **Content Design:** Focuses on the information objects (text, graphics, audio, video) that will be presented to the user.
2.  **Aesthetic Design:** Describes the visual look and feel of the WebApp (Graphic design).
3.  **Architectural Design:** Focuses on the global hypermedia structure of the WebApp and how it is organized.
4.  **Interface Design:** Describes the mechanisms for user interaction and the layout of the UI components.
5.  **Navigation Design:** Defines the paths (links) that allow users to move between content objects.
6.  **Component Design:** Implements the detailed internal logic of the functional elements.

### 8. UML Modelling Tools
*   **Definition:** Software applications used to create and manage UML diagrams during the software development life cycle.
*   **Key Features:**
    *   **Visual Interface:** Drag-and-drop support for UML elements.
    *   **Code Generation:** Automatically generates code (Java, C++, PHP) from diagrams.
    *   **Reverse Engineering:** Generates diagrams from existing source code.
    *   **Documentation:** Automatically generates project documentation.
*   **Common Tools:**
    *   **StarUML:** Lightweight, fast, and cross-platform.
    *   **Visual Paradigm:** Professional grade with complex business modeling features.
    *   **Enterprise Architect:** Comprehensive tool for large-scale enterprise systems.

### 9. Object-Oriented Analysis (OOA) Process
*   **Definition:** The goal of OOA is to define all classes, their relationships, and behaviors that are relevant to the problem to be solved.
*   **Generic Components:**
    1.  **Static Model:** Consists of Class diagrams that define the structure (attributes and operations) of the objects.
    2.  **Object Relationship Model:** Defines how objects are related through Association, Aggregation, or Composition.
    3.  **Object Behavior Model:** Consists of State diagrams and Interaction diagrams that describe how objects respond to events and collaborate.
*   **Output:** The OOA model serves as the foundation for the Design phase.

### 10. Object Design Process (OOD)
*   **Definition:** OOD is the phase where the analysis model is refined and translated into a technical blueprint that can be implemented in a specific programming language.
*   **Key Activities:**
    1.  **Attribute & Method Refinement:** Adding data types to attributes and signatures to methods.
    2.  **Data Structure Design:** Deciding how data will be stored internally (e.g., using a List or a Map).
    3.  **Interface Design:** Finalizing the public methods that other classes will use.
    4.  **Persistence Design:** Mapping objects to database tables (ORM).
    5.  **Optimization:** Applying design patterns to solve common design issues.

### 11. Behavioral Design Patterns
*   **Definition:** Behavioral patterns are concerned with algorithms and the assignment of responsibilities between objects. They describe not just patterns of objects or classes but also the patterns of communication between them.
*   **Examples:**
    1.  **Observer:** Defines a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.
    2.  **Strategy:** Defines a family of algorithms, encapsulates each one, and makes them interchangeable.
    3.  **Command:** Encapsulates a request as an object, thereby letting you parameterize clients with different requests.
    4.  **Iterator:** Provides a way to access the elements of an aggregate object sequentially without exposing its underlying representation.

### 12. Attributes of Web-Based Systems
*   **Network Intensiveness:** Content and applications reside on a network and serve a diverse community of clients.
*   **Concurrency:** A large number of users may access the WebApp at the same time, requiring robust performance.
*   **Unpredictable Load:** The number of users can vary from a few to thousands in a very short time.
*   **Performance:** Users expect rapid response times; any delay can lead to loss of users.
*   **Aesthetics:** The visual look and feel are critical for user engagement and retention.
*   **Continuous Evolution:** WebApps are updated much more frequently (often daily) compared to traditional software.

### 13. Goals of UML
The Unified Modeling Language (UML) was created to achieve the following goals:
1.  **Expressive Power:** Provide users with a ready-to-use, expressive visual modeling language to develop and exchange meaningful models.
2.  **Extensibility:** Provide extensibility and specialization mechanisms to extend the core concepts (using Stereotypes and Tagged Values).
3.  **Independence:** Be independent of particular programming languages and development processes.
4.  **Standardization:** Provide a formal basis for understanding the modeling language.
5.  **Interoperability:** Encourage the growth of the OO tools market by providing a standard exchange format (XMI).

### 14. Software Engineering (SE) vs Web Engineering (WebE)
*   **Software Engineering:**
    *   Deals with traditional software (Desktop, Embedded).
    *   Emphasis on algorithm complexity and data processing.
    *   Development cycles are usually longer (months/years).
    *   Users are often a specific, known group.
*   **Web Engineering:**
    *   Deals specifically with Web-based systems.
    *   Emphasis on content, UI/UX, and network performance.
    *   Development cycles are very short ("Web-time").
    *   Users are an anonymous, diverse, and global audience.

### 15. Steps of Object-Oriented Design (OOD)
1.  **System Design:** Designing the overall architecture and selecting the platform.
2.  **Object Design:** Defining classes, attributes, and method signatures in detail.
3.  **Interaction Design:** Creating Sequence or Communication diagrams to show how objects will collaborate.
4.  **Database Design:** Designing the schema and persistence logic.
5.  **Interface Design:** Designing the user interface and external APIs.
6.  **Refinement:** Applying design patterns and reviewing the design for modularity.

### 16. Types of Interaction Diagrams in UML
Interaction diagrams are a subset of behavioral diagrams. There are four types:
1.  **Sequence Diagram:** Emphasizes the time-ordered sequence of messages.
2.  **Communication Diagram:** Emphasizes the structural organization of the objects that send and receive messages.
3.  **Timing Diagram:** Focuses on the timing constraints of messages and the state changes of objects over time.
4.  **Interaction Overview Diagram:** A high-level diagram that uses an activity-like notation to show the flow of control between different sequence diagrams.

### 17. Object Relationship Model (ORM)
*   **Definition:** The ORM describes the static relationship between objects in a system. It is usually represented using Class Diagrams.
*   **Types of Relationships:**
    1.  **Association:** A general link where objects know about each other.
    2.  **Aggregation:** A "part-of" relationship where the part can exist independently of the whole (e.g., Department and Professors).
    3.  **Composition:** A strong "part-of" relationship where the part cannot exist without the whole (e.g., House and Rooms).
    4.  **Generalization:** An "is-a" relationship (Inheritance).

### 18. Requirement Analysis for WebApps
Requirement analysis for WebApps involves several specific tasks:
1.  **Content Analysis:** Identifies the full spectrum of content (text, graphics, video) to be provided.
2.  **Interaction Analysis:** Describes how the user will interact with the WebApp (using Use Cases).
3.  **Functional Analysis:** Defines the operations and computational tasks the WebApp must perform.
4.  **Configuration Analysis:** Describes the environment (browsers, devices, operating systems) where the WebApp will run.

### 19. Activity Diagram (Short Note)
*   **Definition:** An Activity Diagram is a behavioral diagram that shows the flow of control from one activity to another. It is essentially a flowchart that supports parallel processing.
*   **Usage:** Used to model business processes, complex workflows, or the logic of a single use case.
*   **Key Symbols:**
    *   **Action/Activity:** A rounded rectangle representing a task.
    *   **Decision Diamond:** A diamond shape for branching based on a condition.
    *   **Fork Bar:** A solid black bar used to split one flow into multiple parallel flows.
    *   **Join Bar:** A solid black bar used to synchronize multiple parallel flows back into one.
    *   **Initial/Final Nodes:** Solid circle for start, bullseye for end.

### 20. Message Categories in Interaction Diagrams
1.  **Synchronous Message:** A solid line with a filled head. The sender waits for a return before continuing.
2.  **Asynchronous Message:** A solid line with an open head. The sender does not wait for a response.
3.  **Return Message:** A dashed line with an open head. Returns a value to the caller.
4.  **Create Message:** A message that results in the instantiation of a new object.
5.  **Destroy Message:** A message that explicitly destroys the receiving object.
6.  **Self-Message:** An object calling one of its own methods.
