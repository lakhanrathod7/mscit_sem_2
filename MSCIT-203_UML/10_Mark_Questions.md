# MSCIT-203: Object Oriented Analysis and Design using UML
## 10-Mark Questions (Important for Exam)

1.  **⭐⭐⭐ UML Diagram Types:** Narrate in detail about different types of diagrams in UML. Explain structural vs behavioral diagrams. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
2.  **⭐⭐⭐ Sequence Diagram:** Write a detailed note on Sequence Diagrams. Explain its notations (lifelines, messages) and draw an example for a specific process (e.g., User Login). (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
3.  **⭐⭐⭐ Interaction Diagrams:** Write a detailed note on Interaction Diagrams. List and explain the different types (Sequence, Communication, Timing, Interaction Overview). (Repeated: Aug 2022, Jan 2023, July 2025)
4.  **⭐⭐⭐ Use Case Diagrams:** Explain Use Case diagrams in great detail with examples. Discuss actors and their relationships. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
5.  **⭐⭐⭐ Web Engineering:** Discuss in detail Web Engineering and various attributes/characteristics of web-based systems. (Repeated: Aug 2022, Jan 2023, July 2023, July 2025)
6.  **⭐⭐⭐ Design Patterns:** Explain Creational, Structural, and Behavioral patterns in detail. Discuss specific examples like Builder, Observer, or Decorator. (Repeated: Aug 2022, Jan 2023, July 2023)
7.  **⭐⭐⭐ Class Diagram:** Explain Class Diagrams with proper examples. Discuss attributes, operations, and relationships. (Repeated: Jan 2023, July 2023)
8.  **⭐⭐⭐ OOAD Concepts:** Explain elements and features of Object-Oriented Programming (Abstraction, Encapsulation, Inheritance, Polymorphism). Discuss the Object Relationship Model. (Repeated: Aug 2022, Jan 2023, July 2023)
9.  **⭐⭐ Web Design Pyramid:** Narrate about the design pyramid for Web engineering (Aesthetic, Content, Architecture, Navigation, Interface, Component design). (Repeated: Jan 2023, July 2023, July 2025)
10. **⭐⭐ UML Modeling Tools:** Describe various UML Modeling Tools in brief and their applications. (Repeated: Aug 2022, Jan 2023)
11. **⭐⭐ Collaboration/Communication Diagram:** Explain Communication or Collaboration diagrams with an example and notation. (Repeated: Jan 2023, July 2023)
12. **⭐⭐ Object-Oriented Analysis Model:** Explain generic components of the object-oriented analysis model. (Repeated: July 2025)
13. **⭐⭐ Object Design Process:** Discuss a brief about the Object Design Process. (Repeated: July 2025)
14. **⭐⭐ Requirement Analysis for WebApps:** Explain the requirement analysis process specifically for web-based applications. (Repeated: Jan 2023)
15. **⭐⭐ Message Categories:** Describe different categories of messages in interaction diagrams (Synchronous, Asynchronous, Reply, etc.). (Repeated: July 2023)

---

## Detailed Answers (10-Mark Questions)

### 1. UML Diagram Types (Structural vs Behavioral)
*   **Structural Diagrams:** Show the static structure of a system (the "nouns" and their properties).
    1.  **Class Diagram:** Most common; shows classes, attributes, methods, and relationships.
    2.  **Object Diagram:** Shows a "snapshot" of instances at a specific point in time.
    3.  **Component Diagram:** Shows software modules and their dependencies.
    4.  **Deployment Diagram:** Shows the physical hardware nodes and where the software resides.
*   **Behavioral Diagrams:** Show the dynamic behavior of a system (the "verbs" and actions).
    1.  **Use Case Diagram:** Shows system functionality from an actor's perspective.
    2.  **Activity Diagram:** Shows workflows and parallel processes (like a flowchart).
    3.  **Interaction Diagrams:** (Sequence, Communication) Show message flow between objects.
    4.  **State Machine Diagram:** Shows the life cycle of a single object (e.g., "Order Paid" -> "Shipped").

### 2. Sequence Diagrams (Notations & Example)
*   **Definition:** An interaction diagram that emphasizes the **time ordering** of messages.
*   **Notations:**
    1.  **Actor:** Initiator of the sequence (Stick figure).
    2.  **Lifeline:** Dashed vertical line; represents the object's existence.
    3.  **Activation Bar:** Rectangle on lifeline; indicates the object is active.
    4.  **Messages:** Horizontal arrows.
        *   *Synchronous:* Filled arrowhead (caller waits).
        *   *Asynchronous:* Open arrowhead (caller doesn't wait).
        *   *Return:* Dashed line.
*   **Example (Login):** User sends `input(id, pwd)` -> LoginController. Controller sends `validate()` -> Database. Database returns `success`.

### 3. Interaction Diagrams (Detailed Types)
*   **1. Sequence Diagram:** Focuses on the time-ordered sequence of message exchanges. Great for complex logic.
*   **2. Communication (Collaboration) Diagram:** Focuses on the structural organization of objects. Messages are numbered (1, 1.1, 2) to show order.
*   **3. Timing Diagram:** Shows the change in state of objects over a specific timeline. Used in real-time systems.
*   **4. Interaction Overview Diagram:** A high-level view that uses activity diagram symbols to connect different sequence diagrams.

### 4. Use Case Diagrams (Actors & Relationships)
*   **Components:**
    1.  **Actors:** Human users or external systems interacting with the app.
    2.  **Use Cases:** Specific goals (e.g., "Withdraw Money").
    3.  **System Boundary:** A box enclosing use cases to define the scope.
*   **Relationships:**
    *   **Association:** Line between actor and use case.
    *   **Include (<<include>>):** A mandatory sub-task (e.g., "Withdraw Cash" *includes* "Validate PIN").
    *   **Extend (<<extend>>):** An optional behavior (e.g., "Print Receipt" *extends* "Withdraw Cash").

### 5. Web Engineering (WebE)
*   **Definition:** A disciplined approach used to create high-quality WebApps.
*   **Characteristics:**
    1.  **Network Intensiveness:** Content must travel over the internet.
    2.  **Concurrency:** Multiple users must be handled without performance loss.
    3.  **Unpredictable Load:** Traffic can fluctuate massively.
    4.  **Performance:** Users expect sub-second response times.
    5.  **Aesthetics:** UI design is critical for engagement.
    6.  **Security:** High exposure to global threats requires robust protection.

### 6. Design Patterns (Creational, Structural, Behavioral)
*   **1. Creational:** Focus on object creation (e.g., **Singleton** - only one instance; **Builder** - complex object construction).
*   **2. Structural:** Focus on class/object composition (e.g., **Decorator** - adding functionality dynamically; **Adapter** - connecting incompatible interfaces).
*   **3. Behavioral:** Focus on communication (e.g., **Observer** - 1-to-many notification; **Strategy** - interchangeable algorithms).

### 7. Class Diagrams (Elements & Relationships)
*   **Elements:** Class box has three parts: Name, Attributes (properties), and Operations (methods).
*   **Visibility Symbols:** `+` (public), `-` (private), `#` (protected).
*   **Relationships:**
    *   **Association:** General connection (line).
    *   **Aggregation:** "Part-of" (Hollow diamond).
    *   **Composition:** Strong "Part-of" (Filled diamond).
    *   **Generalization:** Inheritance (Hollow triangle arrow).

### 8. OOAD Concepts (Features)
*   **Abstraction:** Hiding details, showing essential features.
*   **Encapsulation:** Hiding data inside a class, providing access via methods.
*   **Inheritance:** Reusing properties from a parent class.
*   **Polymorphism:** One name, multiple forms (Overloading/Overriding).
*   **Object Relationship Model:** A conceptual model showing how system objects associate and communicate.

### 9. Web Design Pyramid (Layers)
*   **Aesthetic Design:** Visual look and feel (Graphics).
*   **Content Design:** Organizing information objects.
*   **Architecture Design:** Global hypermedia structure.
*   **Navigation Design:** Defining paths between content for different users.
*   **Interface Design:** User interaction mechanisms (UI).
*   **Component Design:** Logic for functional elements.

### 10. UML Modeling Tools
*   **Description:** Specialized software for drawing and managing UML diagrams.
*   **Applications:**
    1.  **Documentation:** Visual record of the system.
    2.  **Communication:** Bridge between developers and stakeholders.
    3.  **Forward Engineering:** Generating code (Java/C++) from diagrams.
    4.  **Reverse Engineering:** Generating diagrams from existing source code.
*   **Tools:** StarUML, Visual Paradigm, Rational Rose, Enterprise Architect.

### 11. Communication Diagram (Collaboration)
*   **Definition:** An interaction diagram emphasizing the structural organization of objects.
*   **Key points:**
    *   Objects are nodes in a graph.
    *   Links show the paths for communication.
    *   Sequence numbers (1.2, 2.1) show the time order.
*   **When to use:** When you want to see the "big picture" of object relationships rather than a strict timeline.

### 12. Object-Oriented Analysis (OOA) Model
*   **Definition:** Translating requirements into a technical model using OO concepts.
*   **Components:**
    *   **Static Model:** Class and Object diagrams.
    *   **Dynamic Model:** State, Sequence, and Activity diagrams.
    *   **Functional Model:** Use Case diagrams.
*   **Outcome:** A clear specification of *what* the system should do.

### 13. Object Design Process (OOD)
*   **Steps:**
    1.  **Refining Classes:** Adding data types and private methods.
    2.  **Designing Algorithms:** Logic for each operation.
    3.  **Data Management:** How objects are stored (Relational vs NoSQL).
    4.  **Interface Design:** Finalizing the public API for the class.
*   **Goal:** Translating "what" into "how".

### 14. Requirement Analysis for WebApps
*   **Steps:**
    1.  **Content Analysis:** Defining the media types (Text, Image, Video).
    2.  **Interaction Analysis:** Use Cases for navigation.
    3.  **Functional Analysis:** Defining computational tasks.
    4.  **Configuration Analysis:** Target devices (Mobile, Desktop) and browsers.

### 15. Message Categories
*   **Synchronous:** Caller waits for return (Blocking).
*   **Asynchronous:** Caller continues immediately (Non-blocking).
*   **Return:** Sends data back to caller.
*   **Self-Message:** Object calling its own method.
*   **Found Message:** Message with an unknown sender.
*   **Lost Message:** Message with an unknown receiver.
