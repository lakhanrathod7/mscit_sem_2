# BAOU M.Sc. IT Semester 2 - Guess Paper (August 2026)
## MSCIT-203: OOAD using UML

**Time: 3 Hours | Max Marks: 70**

---

### Section A: Long Answer Questions (Attempt any 3 - 30 Marks)
1. What is UML? Explain the different types of structural and behavioral diagrams in UML.
2. Draw a detailed Use Case diagram for a "Library Management System" including actors, use cases, and relationships.
3. Write a detailed note on Sequence Diagrams. Explain notations like lifelines and activation boxes with an example.
4. Discuss the design pyramid for Web Engineering (Aesthetic, Content, Architecture, etc.).
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
3. UML is a programming language.
4. An actor must always be a human user.
5. Multiplicity `*` means zero or more.
6. Aggregation is a "part-of" relationship.
7. Iterative development is common in OOAD.
8. Component diagrams show the hardware topology.
9. A class is a template for objects.
10. Design patterns solve recurring design problems.

---
---

# TOPPER'S SOLUTIONS (DETAILED EXAM FORMAT)

## SECTION A: LONG ANSWERS (10 MARKS EACH)

### Q1. UML Diagram Types
**Definition:**
Unified Modeling Language (UML) is a standardized modeling language consisting of an integrated set of diagrams, developed to help system and software developers for specifying, visualizing, constructing, and documenting the artifacts of software systems.

**1. Structural Diagrams (Static View):**
Focuses on the nouns of the system—how it is built.
*   **Class Diagram:** Shows classes, attributes, methods, and their relationships.
*   **Object Diagram:** Snapshot of objects and their states at a point in time.
*   **Component Diagram:** Division of system into physical software modules.
*   **Deployment Diagram:** Mapping of software to physical hardware nodes.

**2. Behavioral Diagrams (Dynamic View):**
Focuses on the verbs—how the system works over time.
*   **Use Case Diagram:** Shows system functionality from a user's perspective.
*   **Interaction Diagrams:** (Sequence & Communication) Show message flow between objects.
*   **Activity Diagram:** Shows the workflow (like a flowchart).
*   **State Machine Diagram:** Life cycle of a single object (e.g., "Order Paid" to "Shipped").

---

### Q3. Sequence Diagrams
**Definition:**
A Sequence Diagram is an interaction diagram that shows how objects operate with one another and in what order. It is effective at visualizing the time-ordered sequence of events.

**Key Notations:**
1.  **Actor:** Stick figure representing an external initiator.
2.  **Lifeline:** Vertical dashed line representing the timeline of an object.
3.  **Activation Bar:** A thin vertical rectangle on the lifeline indicating the object is performing a task.
4.  **Synchronous Message:** Solid line with filled arrow (Sender waits for response).
5.  **Asynchronous Message:** Solid line with open arrow (Sender doesn't wait).
6.  **Return Message:** Dashed line with open arrow.

**Example Logic:**
User -> `login(id, pass)` -> LoginForm -> `validate()` -> Database -> `result` -> LoginForm.

---

### Q5. Design Patterns
A Design Pattern is a reusable solution to a commonly occurring problem in software design.

1.  **Creational (Object Creation):**
    *   **Singleton:** Ensures a class has only one instance and provides a global access point. Use Case: Database connection pool.
2.  **Structural (Class/Object Composition):**
    *   **Decorator:** Adds new functionality to an existing object dynamically without altering its structure. Use Case: Adding "Scrollbar" to a "Window" object.
3.  **Behavioral (Communication):**
    *   **Observer:** Defines a one-to-many relationship where when one object changes state, all its dependents are notified. Use Case: News notification system.

---

## SECTION B: SHORT ANSWERS (5 MARKS EACH)

### Q1. Aggregation vs Composition
*   **Aggregation:** A "Weak" part-of relationship. The part can exist independently of the whole.
    *   *Example:* A Professor and a Department. If the department closes, the professor still exists. Symbol: Hollow diamond.
*   **Composition:** A "Strong" part-of relationship. The part cannot exist without the whole.
    *   *Example:* A Room and a House. If the house is demolished, the room ceases to exist. Symbol: Filled diamond.

### Q3. 4+1 View Architecture
Developed by Philippe Kruchten, it describes software architecture using five concurrent views:
1.  **Logical View:** Functional requirements (Class diagrams).
2.  **Process View:** Non-functional (Performance, Scalability).
3.  **Development View:** Software management (Component diagrams).
4.  **Physical View:** Topology (Deployment diagrams).
5.  **Use Case View (+1):** The center that ties all other views together.

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
2.  **False** (Focuses on sequence; Timing diagram focuses on timing)
3.  **False** (Modeling language)
4.  **False** (Can be another system/hardware)
5.  **True**
6.  **True**
7.  **True**
8.  **False** (Deployment diagrams do)
9.  **True**
10. **True**
