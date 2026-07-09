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
*   **Definition:** Sequence diagrams model the chronological flow of messages between objects.
*   **Key Notations:**
    1.  **Actor:** Represented by a stick figure; an external entity interacting with the system.
    2.  **Lifeline:** A vertical dashed line representing the existence of an object over time.
    3.  **Activation Bar:** A thin rectangle on the lifeline showing when an object is performing an action.
    4.  **Synchronous Message:** A solid line with a filled arrowhead; the sender waits for a response.
    5.  **Return Message:** A dashed line with an open arrowhead; returns data to the caller.

### 2. Interaction Diagrams (Common Terms)
*   **Definition:** These diagrams show how objects collaborate to achieve a task.
*   **Common Terms/Symbols:**
    1.  **Object Instance:** A box with `objectName : ClassName` (underlined).
    2.  **Link:** A line connecting objects, representing a relationship that allows message passing.
    3.  **Message Arrow:** Indicates direction of communication.
    4.  **Self-Message:** An arrow looping back to the same object.
    5.  **Found/Lost Messages:** Used when the source or destination is outside the diagram's scope.

### 3. Creational Design Patterns
*   **Definition:** Patterns that deal with object creation mechanisms, making a system independent of how its objects are created.
*   **Examples:**
    1.  **Singleton:** Ensures only one instance of a class exists (e.g., Database connection).
    2.  **Factory Method:** Lets a class defer instantiation to subclasses.
    3.  **Builder:** Separates the construction of a complex object from its representation.
    4.  **Prototype:** Creates new objects by copying an existing instance.

### 4. OOAD vs Structured Approach
*   **Structured Approach:**
    *   Focuses on **Functions/Processes**.
    *   Data and logic are separate.
    *   Uses Data Flow Diagrams (DFD).
    *   Harder to maintain as the system grows.
*   **Object-Oriented (OOAD):**
    *   Focuses on **Objects/Classes**.
    *   Data and logic are bundled (Encapsulation).
    *   Uses UML diagrams.
    *   Highly modular and easier to reuse/maintain.

### 5. Use Case Diagram with Example
*   **Definition:** A high-level diagram showing the system's functional requirements from the perspective of external actors.
*   **Components:** Actors (stick figures), Use Cases (ovals), and Associations (lines).
*   **Example: Library Management System**
    *   *Actors:* Librarian, Member.
    *   *Use Cases:* Search Book, Issue Book, Return Book.
    *   *Relationship:* "Issue Book" might **include** "Check Member ID".

### 6. Design Pattern Elements
*   **Elements:**
    1.  **Pattern Name:** A unique, descriptive handle.
    2.  **Problem:** Describes when to apply the pattern (the context).
    3.  **Solution:** Describes the elements (classes/objects), their relationships, and responsibilities.
    4.  **Consequences:** The results and trade-offs of applying the pattern (e.g., speed vs. memory).

### 7. WebE Design Pyramid (Layers)
*   **Definition:** A framework for designing high-quality web applications.
*   **Layers:**
    1.  **Content Design:** Defining the information objects (text, graphics, video).
    2.  **Architecture Design:** Global structure and flow (hypermedia).
    3.  **Navigation Design:** Defining paths for different users to move through the app.
    4.  **Interface Design:** Interaction mechanisms and visual layout (UI/UX).

### 8. UML Modelling Tools
*   **Definition:** Software that helps developers create, manage, and share UML diagrams.
*   **Key Features:** Drag-and-drop, automated layout, code generation, and reverse engineering.
*   **Examples:**
    *   **StarUML:** Lightweight and widely used.
    *   **Visual Paradigm:** Feature-rich for enterprise design.
    *   **IBM Rational Rose:** A classic industry standard.

### 9. OOA Process (Generic Components)
*   **Components:**
    1.  **Static Model:** Class diagrams showing properties and relationships.
    2.  **Object Relationship Model:** Specific focus on how objects connect (Aggregation, Composition).
    3.  **Object Behavior Model:** State diagrams and interaction diagrams showing how objects change over time.

### 10. Object Design Process (Short Note)
*   **Overview:** The phase where the Analysis model is refined into a detailed design that can be implemented in code.
*   **Activities:**
    *   Designing the class interface (public methods).
    *   Designing the data structures and algorithms.
    *   Designing the persistence layer (Database mapping).
    *   Optimizing for performance and modularity.

### 11. Behavioral Patterns
*   **Definition:** Patterns that focus on how objects communicate and distribute responsibilities.
*   **Examples:**
    1.  **Observer:** One object notifies many others of state changes.
    2.  **Strategy:** Encapsulates different algorithms for the same task.
    3.  **Command:** Encapsulates a request as an object.

### 12. Attributes of Web-Based Systems
*   **Network Intensiveness:** Content delivered over the internet to diverse clients.
*   **Concurrency:** Thousands of users accessing the app simultaneously.
*   **Unpredictable Load:** Traffic can spike suddenly (e.g., a viral post).
*   **Aesthetics:** Visual appeal is as important as functionality.
*   **Continuous Evolution:** Web apps are updated much more frequently than desktop software.

### 13. Goals of UML
*   **Primary Goals:**
    1.  To provide a ready-to-use, expressive visual modeling language.
    2.  To be independent of specific programming languages.
    3.  To support higher-level concepts like collaborations and frameworks.
    4.  To encourage the growth of the OO tools market.

### 14. Software Engineering (SE) vs Web Engineering (WebE)
*   **SE:** Focuses on traditional software (Desktop/Embedded), longer lifecycles, and stable requirements.
*   **WebE:** Focuses on web-based apps, very short "web-time" cycles, emphasis on content, and huge concurrency challenges.

### 15. Steps of Object-Oriented Design (OOD)
1.  **Define the System:** High-level architecture.
2.  **Define Objects:** Identify classes and their attributes.
3.  **Define Interactions:** Sequence and Communication diagrams.
4.  **Define Control:** How the system starts and manages tasks.
5.  **Refine Design:** Applying design patterns for optimization.

### 16. Types of Interaction Diagrams
1.  **Sequence Diagram:** Time-focused.
2.  **Communication Diagram:** Structure-focused.
3.  **Timing Diagram:** Focuses on time constraints.
4.  **Interaction Overview Diagram:** Mix of activity and sequence diagrams.

### 17. Object Relationship Model (ORM)
*   **Definition:** Describes the static structure of the system by showing how classes are connected.
*   **Types of Relationships:**
    *   **Association:** General connection.
    *   **Aggregation:** "Has-a" relationship (part can exist without whole).
    *   **Composition:** Strong "Has-a" (part cannot exist without whole).

### 18. Requirement Analysis for WebApps
*   **Content Analysis:** What data is needed?
*   **Interaction Analysis:** How will users navigate?
*   **Functional Analysis:** What operations must the system perform?
*   **Configuration Analysis:** What browsers/devices must be supported?

### 19. Activity Diagram (Short Note)
*   **Definition:** A flowchart-like diagram showing the flow of control from one activity to another.
*   **Usage:** Best for modeling business processes, logic flows, and parallel tasks.
*   **Symbols:** Rounded rectangles (Activity), Diamonds (Decision), Bars (Fork/Join).

### 20. Message Categories in Interactions
1.  **Synchronous:** Solid head arrow; caller waits for completion.
2.  **Asynchronous:** Open head arrow; caller continues immediately.
3.  **Return:** Dashed arrow returning data.
4.  **Create/Destroy:** Messages that instantiate or delete an object.
