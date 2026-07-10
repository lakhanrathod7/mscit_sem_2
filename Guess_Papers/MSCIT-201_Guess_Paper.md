# BAOU M.Sc. IT Semester 2 - Guess Paper (August 2026)
## MSCIT-201: Object Oriented Concepts and Programming (Java)

**Time: 3 Hours | Max Marks: 70**

---

### Section A: Long Answer Questions (Attempt any 3 - 30 Marks)
1. Explain basic concepts of OOP (Encapsulation, Polymorphism, Inheritance, Abstraction). Discuss how these are implemented in Java with examples.
2. Explain the Java Virtual Machine (JVM) architecture in detail with a neat diagram. Discuss its role in platform independence.
3. What is Inheritance? List and explain different types of inheritance supported in Java. Why doesn't Java support multiple inheritance through classes?
4. Define a Package. Explain the steps involved in defining and using a user-defined package in Java with a code snippet.
5. Explain the Thread Life Cycle in detail with a diagram. Discuss how threads can be created using the `Thread` class and `Runnable` interface.

---

### Section B: Short Answer Questions (Attempt any 4 - 20 Marks)
1. Explain the purpose and usage of the `this` and `super` keywords in Java.
2. Discuss the exception handling mechanism in Java using `try`, `catch`, `finally`, `throw`, and `throws`.
3. What is a constructor? Explain different types of constructors with examples.
4. Briefly explain the Java Collection Framework. Discuss the difference between List and Set.
5. Explain the Event Delegation Model in Java.
6. Write a short note on Java I/O streams (Character vs Byte streams).

---

### Section C: Part A - MCQs (10 Marks)
1. .java file is compiled by ________ and converted into .class file.
   A. Interpreter B. JVM C. Java compiler D. None
2. Which keyword is used to inherit a class?
   A. implements B. extends C. inherits D. import
3. Which method is automatically called before an object is garbage collected?
   A. destructor() B. finalize() C. free() D. delete()
4. Vector class is available in _________ package.
   A. java.lang B. java.util C. java.awt D. java.io
5. All interface methods in Java are ________ by default.
   A. private B. protected C. public and abstract D. static
6. Which operator is used to allocate memory for an object in Java?
   A. malloc B. create C. new D. alloc
7. A class which cannot be instantiated is called:
   A. Base class B. Derived class C. Abstract class D. Final class
8. Which of these is NOT a primitive data type?
   A. int B. char C. String D. boolean
9. Which keyword makes a variable's value constant?
   A. static B. final C. constant D. abstract
10. Which method is the starting point of any Java application?
    A. init() B. start() C. run() D. main()

---

### Section C: Part B - Do As Directed (10 Marks)
1. True or False: Static methods can be called without creating an object.
2. Java is both __________ and __________. (compiled / interpreted)
3. Full form of JDK?
4. What is the extension of a compiled Java file?
5. True or False: Multiple inheritance is supported in Java via Interfaces.
6. Which keyword refers to the current class instance?
7. True or False: Constructors have no return type.
8. Name the default package imported in every Java program.
9. True or False: String is a mutable class in Java.
10. Which exception is thrown when dividing by zero?

---
---

# TOPPER'S SOLUTIONS (DETAILED EXAM FORMAT)

## SECTION A: LONG ANSWERS (10 MARKS EACH)

### Q1. Basic Concepts of Object-Oriented Programming (OOP)
**Introduction:**
Object-Oriented Programming (OOP) is a programming paradigm based on the concept of "objects", which can contain data (fields) and code (methods). Java is a strictly object-oriented language that follows these four pillars:

**1. Encapsulation (Data Hiding):**
*   **Concept:** It is the process of wrapping data (variables) and code (methods) together as a single unit. It restricts direct access to some of an object's components.
*   **Java Implementation:** Use `private` access modifiers for variables and provide `public` getter/setter methods to access them.
*   **Example:**
    ```java
    class Student {
        private String name; // Private data
        public void setName(String n) { this.name = n; } // Setter
        public String getName() { return this.name; } // Getter
    }
    ```

**2. Inheritance (Code Reusability):**
*   **Concept:** A mechanism where a new class (subclass) is derived from an existing class (superclass). The subclass inherits all non-private features of the parent.
*   **Java Implementation:** Using the `extends` keyword.
*   **Example:** `class Dog extends Animal { ... }`

**3. Polymorphism (Many Forms):**
*   **Concept:** The ability of a single interface or method to perform different tasks.
*   **Types:**
    *   **Compile-time (Overloading):** Multiple methods with the same name but different parameters.
    *   **Runtime (Overriding):** A subclass provides a specific implementation of a method already defined in its parent class.
*   **Example:** `void draw()` can draw a circle or a square depending on the object type.

**4. Abstraction (Hiding Complexity):**
*   **Concept:** Displaying only essential features of an object to the user while hiding the background internal details.
*   **Java Implementation:** Using `abstract` classes and `interfaces`.
*   **Example:** When you press "accelerate" in a car, you don't need to know the combustion logic. In Java: `interface Car { void accelerate(); }`

---

### Q2. JVM Architecture & Platform Independence
**Introduction:**
The Java Virtual Machine (JVM) is an engine that provides a runtime environment to drive the Java code. It is the heart of the "Write Once, Run Anywhere" (WORA) philosophy.

**Architecture Components:**
1.  **Class Loader Subsystem:** Responsible for loading `.class` files. It has three phases: **Loading** (reading files), **Linking** (Verification, Preparation, Resolution), and **Initialization**.
2.  **Runtime Data Areas (Memory):**
    *   **Method Area:** Stores class-level data, including static variables.
    *   **Heap Area:** Stores all objects created during runtime. It is shared by all threads.
    *   **Stack Area:** Stores local variables and partial results for each thread.
    *   **PC Registers:** Contains the address of the currently executing instruction.
    *   **Native Method Stack:** For native (C/C++) methods.
3.  **Execution Engine:**
    *   **Interpreter:** Executes bytecode line by line.
    *   **JIT Compiler (Just-In-Time):** Compiles frequently used code into native machine code to improve performance.
    *   **Garbage Collector:** Automatically manages memory by reclaiming space from unused objects.

**Role in Platform Independence:**
Java code (`.java`) is compiled into an intermediate form called **Bytecode** (`.class`). Bytecode is not machine code. Every Operating System (Windows, Linux, Mac) has its own version of JVM. The same bytecode can be sent to any OS, and that OS's JVM will translate it into its own machine language. This makes Java platform-independent.

---

### Q3. Inheritance & The "Diamond Problem"
**Definition:**
Inheritance allows a class to derive features from another class, promoting code reusability and establishing a "IS-A" relationship.

**Types of Inheritance in Java:**
1.  **Single:** Subclass B inherits from Superclass A.
2.  **Multilevel:** C inherits from B, and B inherits from A.
3.  **Hierarchical:** Many subclasses (B, C, D) inherit from one parent (A).
4.  **Multiple (Interfaces only):** One class implements multiple interfaces.

**Why Java doesn't support Multiple Inheritance through classes?**
This is to avoid the **Diamond Problem**. If Class B and Class C both inherit from Class A and override a method `display()`, and then Class D inherits from both B and C, Class D would be confused about which version of `display()` to inherit. To keep Java simple and avoid this ambiguity, multiple inheritance for classes was removed.

---

## SECTION B: SHORT ANSWERS (5 MARKS EACH)

### Q1. `this` vs `super`
*   **`this` keyword:**
    1.  Refers to the **current class instance**.
    2.  Used to resolve "Shadowing" (when local variables and instance variables have the same name).
    3.  Used for constructor chaining (calling one constructor from another in the same class).
*   **`super` keyword:**
    1.  Refers to the **immediate parent class instance**.
    2.  Used to invoke the parent class constructor (`super()`).
    3.  Used to call parent methods that have been overridden in the child class.

### Q2. Exception Handling Mechanism
Java handles runtime errors using a robust hierarchy of classes (`Throwable` -> `Exception`).
*   **try:** Wraps the code that might throw an exception.
*   **catch:** Handles the specific exception if it occurs.
*   **finally:** A block that **always** executes, regardless of an error (used for closing files/database connections).
*   **throw:** Used to manually trigger an exception.
*   **throws:** Declared in the method signature to warn the caller that this method might throw certain exceptions.

### Q3. Constructors
A constructor is a special method called when an object is instantiated. It has no return type and the same name as the class.
*   **Default Constructor:** Provided by the compiler if no constructor is written. It initializes fields to 0 or null.
*   **Parameterized Constructor:** Takes arguments to initialize an object with specific data.
    *   *Example:* `Student(int id, String name) { this.id = id; this.name = name; }`
*   **Constructor Overloading:** Defining multiple constructors with different parameter lists in one class.

---

## SECTION C: OBJECTIVE ANSWERS

### Part A: MCQs
1.  **C.** Java compiler
2.  **B.** extends
3.  **B.** finalize()
4.  **B.** java.util
5.  **C.** public and abstract
6.  **C.** new
7.  **C.** Abstract class
8.  **C.** String (It is a class in java.lang)
9.  **B.** final
10. **D.** main()

### Part B: Do As Directed
1.  **True**
2.  **Compiled** and **Interpreted**
3.  **Java Development Kit**
4.  **.class**
5.  **True**
6.  **this**
7.  **True**
8.  **java.lang**
9.  **False** (String is immutable; StringBuffer/StringBuilder are mutable)
10. **ArithmeticException**
