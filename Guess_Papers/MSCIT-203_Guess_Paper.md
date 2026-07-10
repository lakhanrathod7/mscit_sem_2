# BAOU M.Sc. IT Semester 2 - Guess Paper (August 2026)
## MSCIT-203: Object Oriented Analysis and Design using UML

**Time: 3 Hours | Max Marks: 70**

---

### Section A: Long Answer Questions (Attempt any 3 - 30 Marks)
1. What is UML? Explain the different types of structural and behavioral diagrams in UML.
2. Draw a detailed Use Case diagram for a "Library Management System" including actors, use cases, and relationships.
3. Write a detailed note on Sequence Diagrams. Explain notations like lifelines and activation boxes with an example.
4. Discuss the design pyramid for Web Engineering (Aesthetic, Content, Architecture, Navigation, Interface, and Component Design).
5. Explain Creational, Structural, and Behavioral design patterns with one example each.

---

### Section B: Short Answer Questions (Attempt any 4 - 20 Marks)
1. Differentiate between Aggregation and Composition with examples.
2. Explain the features of OOP: Abstraction, Encapsulation, and Polymorphism.
3. Discuss the 4+1 View Architecture of UML.
4. Explain UML Modelling Tools in brief.
5. Write a short note on Activity Diagrams.
6. What are CRC cards and how are they used in OOA?

---

### Section C: Part A - MCQs (10 Marks)
1. UML stands for:
   A. Universal Modeling Language B. Unified Modeling Language C. United Modeling Language D. Unique Modeling Language
2. Which diagram shows the static structure of a system?
   A. Sequence B. Activity C. Class D. Use Case
3. The symbol '#' in UML represents:
   A. Public B. Private C. Protected D. Package
4. Who are the "Three Amigos" of UML?
   A. Booch, Rumbaugh, Jacobson B. Gates, Jobs, Allen C. Ritchie, Thompson, Stroustrup D. None
5. A design pattern used to restrict access to an object is:
   A. Adapter B. Proxy C. Decorator D. Factory
6. Which relationship represents "is-a"?
   A. Association B. Aggregation C. Generalization D. Composition
7. In an Activity diagram, a diamond shape represents:
   A. Start B. Decision C. End D. Action
8. Interaction diagrams include Sequence and:
   A. Class B. Deployment C. Communication D. Component
9. Full form of CRC:
   A. Class-Role-Call B. Class-Responsibility-Collaborator C. Class-Record-Code D. None
10. Which view is the center of the 4+1 architecture?
    A. Logical B. Process C. Use Case D. Development

---

### Section C: Part B - True or False (10 Marks)
1. Encapsulation is the process of data hiding.
2. Sequence diagrams focus on the timing of messages.
3. UML is a modeling language, not a programming language.
4. An actor must always be a human user.
5. Multiplicity `*` means zero or more.
6. Aggregation is a "part-of" relationship where parts can exist independently.
7. Iterative development is common in OOAD.
8. Component diagrams show the hardware topology.
9. A class is a template for objects.
10. Design patterns solve recurring design problems.

---
---

# TOPPER'S SOLUTIONS (DETAILED EXAM FORMAT)

## SECTION A: LONG ANSWERS (10 MARKS EACH)

### Q1. UML Diagram Types (Exhaustive Breakdown)
**Definition:**
Unified Modeling Language (UML) is a standardized visual modeling language used to specify, visualize, construct, and document software systems. It provides a common vocabulary for developers.

**1. Structural Diagrams (Static View):**
These diagrams represent the static aspects of the system—the "nouns" and how they are organized.
*   **Class Diagram:** The most fundamental UML diagram. It shows classes, their attributes, methods, and relationships (like inheritance and association).
*   **Object Diagram:** Shows instances of classes at a specific moment in time. Useful for modeling complex data structures.
*   **Component Diagram:** Describes how the system is divided into physical software modules (like JAR files or DLLs) and their dependencies.
*   **Deployment Diagram:** Shows the physical hardware nodes (servers, devices) and the software components running on them.
*   **Package Diagram:** Shows how classes are grouped into logical packages.

**2. Behavioral Diagrams (Dynamic View):**
These diagrams show the dynamic behavior of the system—the "verbs" and how the system changes over time.
*   **Use Case Diagram:** High-level view showing system functionality from the perspective of external actors (users).
*   **Interaction Diagrams:**
    *   *Sequence Diagram:* Focuses on the time-ordered sequence of messages.
    *   *Communication Diagram:* Focuses on the structural organization of objects.
*   **Activity Diagram:** Shows the workflow or business process, including parallel execution (fork/join).
*   **State Machine Diagram:** Shows the lifecycle of a single object and how it responds to events.

---

### Q3. Sequence Diagrams (Notations & Logic)
**Definition:**
A Sequence Diagram is an interaction diagram that models the chronological flow of messages between objects. It is the primary tool for detailed logic design in OO systems.

**Key Notations:**
1.  **Actor:** Stick figure representing an external initiator (Human or System).
2.  **Lifeline:** A dashed vertical line that represents the existence of an object over time.
3.  **Activation Bar:** A thin vertical rectangle on the lifeline indicating the object is actively performing an operation or waiting for a sub-call to return.
4.  **Synchronous Message:** A solid line with a filled arrowhead. The sender "blocks" and waits for a response.
5.  **Asynchronous Message:** A solid line with an open arrowhead. The sender continues without waiting.
6.  **Return Message:** A dashed line with an open arrowhead returning data to the caller.

**Topper's Tip:** In an exam, always draw a small example.
*Example:* **User** -> `login(id, pwd)` -> **LoginForm** -> `validate()` -> **LoginController** -> `success/fail` -> **LoginForm**.

---

### Q5. Design Patterns (Creational, Structural, Behavioral)
Design patterns are proven, reusable solutions to recurring design problems.

**1. Creational Patterns (Object Creation):**
These patterns abstract the instantiation process, making a system independent of how its objects are created.
*   *Example:* **Singleton Pattern**. Ensures that a class has only one instance and provides a global access point to it. (e.g., a shared Database Connection Pool).

**2. Structural Patterns (Object Composition):**
These patterns deal with how classes and objects are composed to form larger structures.
*   *Example:* **Decorator Pattern**. Adds new functionality to an existing object dynamically without altering its structure or using inheritance. (e.g., adding a "scroll bar" to a "text window").

**3. Behavioral Patterns (Communication):**
These patterns focus on how objects communicate and distribute responsibilities.
*   *Example:* **Observer Pattern**. Defines a one-to-many relationship where when one object changes state, all its dependents (observers) are notified automatically. (e.g., a "News Update" system notifying all subscribers).

---

## SECTION B: SHORT ANSWERS (5 MARKS EACH)

### Q1. Aggregation vs Composition
Both are "Part-of" relationships, but they differ in strength:
*   **Aggregation (Weak):** The "part" can exist independently of the "whole".
    *   *Symbol:* Hollow diamond.
    *   *Example:* A **Library** and its **Books**. If the library closes, the books still exist.
*   **Composition (Strong):** The "part" cannot exist without the "whole". The whole manages the part's lifecycle.
    *   *Symbol:* Filled diamond.
    *   *Example:* A **House** and its **Rooms**. If the house is demolished, the rooms are also destroyed.

### Q3. 4+1 View Architecture
Developed by Philippe Kruchten, this architecture describes a system from five perspectives:
1.  **Logical View:** Focuses on functional requirements (Class/Object diagrams).
2.  **Process View:** Focuses on runtime behavior, performance, and scalability.
3.  **Development View:** Focuses on software management and organization (Component diagrams).
4.  **Physical View:** Focuses on the hardware topology (Deployment diagrams).
5.  **Use Case View (+1):** The center of the model. It ties all other views together by describing the scenarios.

---

## SECTION C: OBJECTIVE ANSWERS

### Part A: MCQs
1.  **B.** Unified Modeling Language
2.  **C.** Class
3.  **C.** Protected
4.  **A.** Booch, Rumbaugh, Jacobson
5.  **B.** Proxy
6.  **C.** Generalization
7.  **B.** Decision
8.  **C.** Communication
9.  **B.** Class-Responsibility-Collaborator
10. **C.** Use Case

### Part B: True or False
1.  **True**
2.  **False** (Sequence diagrams focus on the sequence of messages; Timing diagrams focus on timing)
3.  **True**
4.  **False** (Can be an external system or hardware)
5.  **True**
6.  **True**
7.  **True**
8.  **False** (Deployment diagrams show hardware)
9.  **True**
10. **True**
