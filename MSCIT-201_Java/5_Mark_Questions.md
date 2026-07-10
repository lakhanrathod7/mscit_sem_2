# MSCIT-201: Object Oriented Concepts and Programming (Java)
## 5-Mark Questions (Short Notes)

1.  **⭐⭐⭐ `this` keyword:** Explain the purpose and usage of the `this` keyword in Java. (Repeated: July 2025, July 2023)
2.  **⭐⭐⭐ Features of Java:** List and explain the unique features of Java (Platform independent, Secure, Object-oriented, etc.). (Repeated: Aug 2022, July 2023)
3.  **⭐⭐⭐ Datatypes:** Briefly explain different datatypes available in Java. (Repeated: Aug 2022)
4.  **⭐⭐⭐ Constructors in detail:** Explain different types of constructors. (Repeated: Aug 2022)
5.  **⭐⭐⭐ Subclass Constructor:** Explain the subclass constructor with an example. (Repeated: Jan 2023)
6.  **⭐⭐⭐ Method Overriding:** Explain overriding methods in detail. (Repeated: Jan 2023)
7.  **⭐⭐⭐ Nesting of methods:** What is nesting of methods? Provide an example demonstrating its use. (Repeated: July 2025)
8.  **⭐⭐⭐ Multithreading:** Discuss multithreading and thread states in brief. (Repeated: Aug 2022, July 2025)
9.  **⭐⭐⭐ Built-in Packages:** List five built-in packages in Java and explain them in brief. (Repeated: Jan 2023, July 2023, July 2025)
10. **⭐⭐ Error Types:** Discuss different types of errors (Compile-time, Run-time, Logical) in brief. (Repeated: Aug 2022)
11. **⭐⭐ Collection Framework:** Explain the Collection Framework with a diagram. (Repeated: July 2023)
12. **⭐⭐ Events:** What is an event? Define various types of events in brief. (Repeated: July 2023)
13. **⭐⭐ String class:** Explain the String class and its common methods like `indexOf()`. (Repeated: Jan 2023, Aug 2022)
14. **⭐⭐ Command Line Arguments:** Explain command line arguments in brief. (Repeated: Jan 2023)
15. **⭐⭐ Vector class:** Briefly explain the Vector class with an example. (Repeated: Jan 2023, July 2023)
16. **⭐⭐ Exception handling keywords:** Explain the use of `try`, `catch`, `finally`, `throw`, and `throws`. (Repeated: July 2025)
17. **⭐⭐ Stream types:** Write the difference between Character streams and Byte streams. (Repeated: July 2023)
18. **⭐ Wrapper classes:** What are wrapper classes? (Repeated: Jan 2023)
19. **⭐ Abstract vs Final class:** Briefly explain the difference. (Repeated: July 2023)
20. **⭐ Java Environment:** Briefly discuss the Java development environment (JDK, JRE, JVM). (Repeated: Jan 2023)

---

## Detailed Answers (5-Mark Questions)

### 1. `this` Keyword in Java
*   **Definition:** `this` is a reference variable that refers to the "current object"—the instance of the class whose method or constructor is being called.
*   **Key Usages with Examples:**
    1.  **To refer to instance variables:** Used when a local variable (parameter) has the same name as an instance variable (Shadowing).
        *   Example: `this.rollno = rollno;`
    2.  **To invoke current class constructor:** Known as "Constructor Chaining". Must be the first statement in the constructor.
        *   Example: `this();` calls the default constructor; `this(5);` calls a parameterized one.
    3.  **To invoke current class method:** Useful if you want to explicitly show a method call is on the current object, though the compiler adds it automatically.
    4.  **To pass as an argument:** `this` can be passed as an argument in a method call (e.g., `process(this);`).
    5.  **To return the current class instance:** `return this;` is used in method chaining.
*   **Constraint:** It cannot be used in `static` methods or static blocks because static members belong to the class, not to any specific instance.

### 2. Features of Java (Unique Selling Points)
*   **Object-Oriented:** Java follows the OOP paradigm, focusing on objects and classes. It supports core concepts like Abstraction, Encapsulation, Inheritance, and Polymorphism.
*   **Platform Independent:** Java uses the "Write Once, Run Anywhere" (WORA) principle. Java code is compiled into **Bytecode**, which is platform-neutral. Any machine with a **JVM** (Java Virtual Machine) can run this bytecode.
*   **Simple:** Removed confusing features of C++ like explicit pointers, operator overloading, and multiple inheritance (for classes). Its syntax is clean and easy to learn.
*   **Secure:** Java provides a secure environment by running code inside a "sandbox" (JVM). It lacks pointers (preventing direct memory access) and has a "Security Manager" to define access rules.
*   **Robust:** Focuses on compile-time and runtime error checking. It has a strong memory management system with **Automatic Garbage Collection** and handles exceptions strictly.
*   **Multithreaded:** Supports concurrent execution of two or more parts of a program to maximum CPU utilization. It provides a built-in `Thread` class and `Runnable` interface.

### 3. Java Datatypes
*   **Definition:** Datatypes define the size and type of values that can be stored in variables.
*   **Classification:**
    1.  **Primitive Datatypes (Predefined):**
        *   **Integer types:** `byte` (1 byte), `short` (2 bytes), `int` (4 bytes), `long` (8 bytes).
        *   **Floating-point:** `float` (4 bytes), `double` (8 bytes).
        *   **Character:** `char` (2 bytes, supports Unicode/international characters).
        *   **Boolean:** `boolean` (stores `true` or `false`).
    2.  **Non-Primitive (Reference) Datatypes:** Created by the programmer (except String). They store the memory address (reference) of the object.
        *   **Classes:** Blueprint for objects (e.g., `Student`).
        *   **Interfaces:** Contract for what a class can do.
        *   **Arrays:** Group of similar typed variables.
        *   **Strings:** Sequence of characters (it is a class in `java.lang`).

### 4. Constructors in Java
*   **Definition:** A constructor is a special block of code that is automatically called when an object of a class is created. It initializes the object's state.
*   **Rules:** It must have the same name as the class and no return type (not even `void`).
*   **Types:**
    1.  **Default Constructor:** Automatically provided by the Java compiler if no constructor is written. It initializes numeric variables to 0 and objects to `null`.
    2.  **No-Arg Constructor:** A programmer-defined constructor that takes no parameters. Used to provide custom default values.
    3.  **Parameterized Constructor:** Takes arguments to initialize an object with specific data.
*   **Constructor Overloading:** Like method overloading, a class can have multiple constructors with different parameter lists.
*   **Example:**
    ```java
    class Box {
        int w, h;
        Box() { w = 10; h = 10; } // No-arg
        Box(int s) { w = s; h = s; } // Parameterized
    }
    ```

### 5. Subclass Constructor
*   **Definition:** When an object of a subclass is created, the subclass constructor is called. However, it must first execute the constructor of its superclass (parent) to initialize inherited members.
*   **The `super()` Keyword:**
    *   Used to explicitly call a specific constructor of the superclass.
    *   It **must** be the first statement in the subclass constructor.
    *   If you don't write `super()`, the compiler automatically inserts a default `super()` call to the parent's no-arg constructor.
*   **Example:**
    ```java
    class Parent { Parent() { System.out.println("Parent Init"); } }
    class Child extends Parent { 
        Child() { 
            super(); // Calls Parent constructor
            System.out.println("Child Init"); 
        } 
    }
    ```

### 6. Method Overriding
*   **Definition:** If a subclass provides a specific implementation for a method that is already defined in its superclass, it is called Method Overriding.
*   **Rules:**
    1.  The method name and parameters must be **exactly the same** (same signature).
    2.  There must be an **Inheritance** (IS-A) relationship.
    3.  The return type must be the same (or a subtype).
    4.  Access modifier cannot be more restrictive (e.g., if parent is `protected`, child cannot be `private`).
*   **Usage:** Used to achieve **Runtime Polymorphism**. It allows a subclass to provide its own behavior for a general method provided by the parent.
*   **Example:** Parent class `Shape` has `draw()`; subclasses `Circle` and `Square` override `draw()` to draw specific shapes.

### 7. Nesting of Methods
*   **Definition:** In Java, a method cannot be defined *inside* another method (no local functions), but a method can **invoke** (call) another method of the same class directly. This is called nesting of methods.
*   **Working:** When one method is called, it performs part of the work and delegates the rest by calling another method.
*   **Example:**
    ```java
    class Calc {
        int square(int n) { return n * n; }
        void display(int x) {
            int result = square(x); // Nesting call
            System.out.println("Result: " + result);
        }
    }
    ```
*   **Purpose:** To improve code organization, reduce redundancy, and break complex tasks into smaller reusable units.

### 8. Multithreading & Thread States
*   **Multithreading:** The ability of a CPU to execute multiple threads (lightweight processes) concurrently. It allows a program to perform multiple tasks at the same time (e.g., downloading a file while typing in a document).
*   **Thread Life Cycle (States):**
    1.  **New:** Thread object created, but `start()` not called.
    2.  **Runnable:** Ready to run and waiting for CPU time from the thread scheduler.
    3.  **Running:** Currently being executed by the processor.
    4.  **Blocked/Waiting:** Waiting for a resource (I/O) or another thread (via `sleep()`, `wait()`, or `join()`).
    5.  **Terminated (Dead):** The `run()` method has finished execution.
*   **Mechanism:** Achieved by extending the `Thread` class or implementing the `Runnable` interface.

### 9. Built-in Packages in Java
*   **Definition:** Packages are containers for classes that provide a naming space and access control.
*   **Key Built-in Packages:**
    1.  `java.lang`: Contains fundamental classes like `String`, `Math`, `System`, and wrapper classes. It is **imported automatically**.
    2.  `java.util`: Contains utility classes like `Scanner`, `Date`, `Random`, and the entire **Collection Framework** (`ArrayList`, `HashMap`).
    3.  `java.io`: Provides classes for input and output operations (reading/writing to files and streams).
    4.  `java.net`: Contains classes for networking (Sockets, URL handling).
    5.  `java.awt` / `javax.swing`: Used for creating Graphical User Interfaces (GUI) like windows, buttons, and text fields.

### 10. Error Types in Java
*   **1. Compile-time Errors:** Caught by the compiler before the program runs.
    *   *Causes:* Syntax errors (missing `;`, wrong spelling), using undeclared variables, or incompatible types.
    *   *Effect:* Program will not generate a `.class` file.
*   **2. Runtime Errors (Exceptions):** Occur during the execution of the program.
    *   *Causes:* Logical flaws like dividing by zero (`ArithmeticException`), accessing a null object (`NullPointerException`), or array index out of bounds.
    *   *Effect:* Program crashes abruptly if not handled using `try-catch`.
*   **3. Logical Errors:** The program runs without crashing but gives the **wrong output**.
    *   *Causes:* Incorrect logic (e.g., using `+` instead of `*` for area).
    *   *Effect:* Hardest to find; requires debugging.

### 11. Java Collection Framework
*   **Definition:** A unified architecture (set of interfaces and classes) for representing and manipulating collections of objects.
*   **Core Interfaces:**
    *   **List:** Ordered, allows duplicates (e.g., `ArrayList`, `LinkedList`).
    *   **Set:** Unordered, no duplicates allowed (e.g., `HashSet`, `TreeSet`).
    *   **Map:** Key-Value pairs, unique keys (e.g., `HashMap`).
*   **Hierarchy Diagram (Conceptual):**
    `Collection (I) -> List (I), Set (I), Queue (I)`. `Map (I)` is a separate hierarchy.
*   **Advantages:** Reduces programming effort, increases performance, and provides standard data structures that are highly optimized.

### 12. Events in Java (AWT/Swing)
*   **Definition:** An event is an object that describes a state change in a source (e.g., a button click, a key press, or a mouse move).
*   **Delegation Model Components:**
    1.  **Event Source:** The UI component where the event happens (e.g., `JButton`).
    2.  **Event Object:** Encapsulates the details (e.g., `ActionEvent` tells which button was clicked).
    3.  **Event Listener:** An interface (e.g., `ActionListener`) that receives the event and performs an action.
*   **Common Types:**
    *   **Action Event:** Button click, Menu selection.
    *   **Mouse Event:** Clicking, dragging, or moving the mouse.
    *   **Key Event:** Pressing or releasing a key on the keyboard.

### 13. String Class & Common Methods
*   **Definition:** In Java, a String is an object of the `String` class. They are **immutable**, meaning once created, their value cannot be changed in memory.
*   **Common Methods:**
    1.  `length()`: Returns the number of characters.
    2.  `charAt(index)`: Returns the character at a specific position.
    3.  `indexOf("substring")`: Returns the index of the first occurrence of a string.
    4.  `equals(s)`: Compares the **content** of two strings (case-sensitive).
    5.  `substring(start, end)`: Extracts a portion of the string.
    6.  `toLowerCase()` / `toUpperCase()`: Changes the case.
*   **Note:** If you need a string that can be modified frequently, use `StringBuilder` or `StringBuffer`.

### 14. Command Line Arguments
*   **Definition:** Arguments passed to a Java program during its execution from the command prompt.
*   **Mechanism:** They are stored as Strings in the `String[] args` array parameter of the `main` method.
*   **Example:**
    *   Run: `java Greet Amit 25`
    *   Inside `main`: `args[0]` is "Amit", `args[1]` is "25".
*   **Conversion:** Since they are strings, you must use wrapper class methods like `Integer.parseInt(args[1])` to convert them to numbers.
*   **Use Case:** Passing configuration settings or input data without changing the source code.

### 15. Vector Class in Java
*   **Definition:** Part of the `java.util` package, `Vector` implements a growable array of objects. It is part of the original Java API (Legacy class) but was retrofitted into the Collection Framework.
*   **Key Features:**
    1.  **Dynamic Sizing:** It automatically doubles its size when the capacity is reached.
    2.  **Synchronized:** It is **thread-safe**, meaning multiple threads can access it without causing data corruption.
    3.  **Insertion Order:** It maintains the order in which elements were added.
*   **Example:**
    ```java
    Vector v = new Vector();
    v.add("Java");
    v.add(100); // Autoboxing
    System.out.println(v.get(0)); // Prints Java
    ```

### 16. Exception Handling Keywords
*   **try:** Used to enclose the code that might throw an exception. It must be followed by either `catch` or `finally`.
*   **catch:** Used to handle the specific exception thrown in the `try` block. You can have multiple catch blocks.
*   **finally:** A block that **always executes** (regardless of whether an exception occurred). Used for cleanup (closing files/databases).
*   **throw:** Used to explicitly throw a single exception (e.g., `throw new ArithmeticException();`).
*   **throws:** Used in a method signature to declare that the method might throw certain exceptions, forcing the caller to handle them.

### 17. Character vs Byte Streams
*   **Byte Streams:**
    *   Data processed 8 bits (1 byte) at a time.
    *   Used for binary data: Images, Audio, Video, Executables.
    *   Main Classes: `InputStream`, `OutputStream` (and subclasses like `FileInputStream`).
*   **Character Streams:**
    *   Data processed 16 bits (2 bytes) at a time (Unicode).
    *   Used for text files: `.txt`, `.html`, `.java`.
    *   Main Classes: `Reader`, `Writer` (and subclasses like `FileReader`).
*   **Rule:** Always use Character streams for reading/writing text as they automatically handle character encoding (Internationalization).

### 18. Wrapper Classes
*   **Definition:** Wrapper classes provide a way to use primitive data types (`int`, `char`, etc.) as objects.
*   **Mapping:** `int -> Integer`, `char -> Character`, `float -> Float`, `double -> Double`.
*   **Why needed?**
    1.  The Collection Framework (e.g., `ArrayList`) only works with objects, not primitives.
    2.  They provide utility methods (e.g., `Integer.parseInt()`).
*   **Autoboxing:** Automatic conversion of primitive to object (e.g., `Integer x = 5;`).
*   **Unboxing:** Automatic conversion of object to primitive (e.g., `int y = x;`).

### 19. Abstract Class vs Final Class
*   **Abstract Class:**
    *   Keyword: `abstract`.
    *   **Cannot be instantiated** (no object creation).
    *   Can have both abstract (no body) and concrete (with body) methods.
    *   **Purpose:** To be inherited and act as a template for subclasses.
*   **Final Class:**
    *   Keyword: `final`.
    *   **Cannot be inherited** (prevents subclassing).
    *   All its methods are implicitly final.
    *   **Purpose:** For security and performance (e.g., the `String` class is final).

### 20. Java Environment (JDK, JRE, JVM)
*   **JVM (Java Virtual Machine):** An abstract machine that executes Java bytecode. It provides a platform-independent environment for Java programs.
*   **JRE (Java Runtime Environment):** Consists of the **JVM + Standard Libraries**. It provides the environment necessary to **run** a Java program.
*   **JDK (Java Development Kit):** Consists of the **JRE + Development Tools** (like `javac` compiler, `jdb` debugger). It is required to **write and compile** Java programs.
*   **Hierarchy:** JDK > JRE > JVM.
