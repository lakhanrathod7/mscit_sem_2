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
*   **Definition:** `this` is a reference variable in Java that refers to the "current object" within an instance method or a constructor.
*   **Key Usages:**
    1.  **To refer to instance variables:** Used when a local variable (parameter) has the same name as an instance variable (Shadowing).
        *   Example: `this.name = name;`
    2.  **To invoke current class constructor:** Known as "Constructor Chaining". Must be the first statement in the constructor.
        *   Example: `this();` or `this(10);`
    3.  **To invoke current class method:** If you don't use `this`, the compiler automatically adds it.
    4.  **To pass as an argument:** Can be passed as an argument in a method call or constructor call.
*   **Constraint:** Cannot be used in `static` methods because static methods are called without any object.

### 2. Features of Java (Unique Selling Points)
*   **Platform Independent:** Java uses the "Write Once, Run Anywhere" (WORA) principle. Java code is compiled into **Bytecode**, which runs on any machine equipped with a Java Virtual Machine (JVM).
*   **Object-Oriented:** Everything in Java is an object. It supports core concepts like Encapsulation, Inheritance, and Polymorphism.
*   **Simple:** The syntax is clean and based on C++. It removed confusing features like explicit pointers and operator overloading.
*   **Secure:** Java runs inside a virtual machine (sandbox). It has no pointers to access private memory and includes a "Security Manager" to control access to system resources.
*   **Robust:** Focuses on compile-time and runtime error checking. It has strong memory management (Garbage Collection) and handles exceptions strictly.
*   **Multithreaded:** Java allows writing programs that can do many tasks simultaneously, improving performance for complex applications.

### 3. Java Datatypes
*   **Definition:** Datatypes define the size and type of values that can be stored in variables.
*   **Classification:**
    1.  **Primitive Datatypes:** Predefined by the language.
        *   *Numeric (Integer):* `byte` (1 byte), `short` (2 bytes), `int` (4 bytes), `long` (8 bytes).
        *   *Floating Point:* `float` (4 bytes), `double` (8 bytes).
        *   *Character:* `char` (2 bytes, uses Unicode).
        *   *Logical:* `boolean` (true/false).
    2.  **Non-Primitive (Reference) Datatypes:** Created by the programmer (except String).
        *   Classes, Interfaces, Arrays, and Strings. They store the memory address (reference) of the object.

### 4. Constructors in Java
*   **Definition:** A constructor is a special block of code that is automatically called when an object of a class is created. It has the same name as the class and no return type (not even `void`).
*   **Types:**
    1.  **Default Constructor:** Provided by Java if no constructor is written. It takes no arguments and initializes variables to default values (0, null).
    2.  **No-Arg Constructor:** A programmer-defined constructor with no parameters.
    3.  **Parameterized Constructor:** Takes arguments to initialize an object with specific data.
*   **Constructor Overloading:** A class can have multiple constructors with different parameter lists.

### 5. Subclass Constructor
*   **Definition:** When an object of a subclass is created, the subclass constructor is called. However, it first implicitly calls the constructor of its superclass (parent).
*   **The `super()` Keyword:**
    *   Used to explicitly call a specific constructor of the superclass.
    *   If not used, the compiler adds a default `super()` call as the first line of the subclass constructor.
*   **Example:**
    ```java
    class Parent { Parent() { System.out.println("Parent Created"); } }
    class Child extends Parent { 
        Child() { 
            super(); // Optional, compiler adds it
            System.out.println("Child Created"); 
        } 
    }
    ```

### 6. Method Overriding
*   **Definition:** If a subclass provides a specific implementation for a method that is already defined in its superclass, it is called Method Overriding.
*   **Rules:**
    1.  The method name and parameters must be **exactly the same**.
    2.  There must be an IS-A relationship (Inheritance).
    3.  The access modifier of the overriding method cannot be more restrictive than the parent (e.g., if parent is `protected`, child cannot be `private`).
*   **Usage:** Used to achieve **Runtime Polymorphism**. It allows a subclass to provide its own behavior while sharing the same method signature.

### 7. Nesting of Methods
*   **Definition:** Nesting of methods is a technique where one method calls another method within the same class. In Java, methods cannot be defined *inside* another method, but they can be *invoked* from one another.
*   **Purpose:** To break down a complex task into smaller, reusable steps.
*   **Example:**
    ```java
    class Box {
        int length, width;
        int area() { return length * width; }
        void display() {
            int a = area(); // Nesting call
            System.out.println("Area is: " + a);
        }
    }
    ```

### 8. Multithreading & Thread States
*   **Multithreading:** The ability of a CPU to execute multiple threads (lightweight processes) concurrently to maximize utilization.
*   **Thread States (Life Cycle):**
    1.  **New:** When a thread instance is created but `start()` is not called.
    2.  **Runnable:** Ready to run and waiting for CPU time.
    3.  **Running:** Currently being executed by the processor.
    4.  **Blocked/Waiting:** Waiting for a resource or another thread (e.g., during `sleep()` or I/O).
    5.  **Dead (Terminated):** Execution is finished.

### 9. Built-in Packages in Java
*   **Definition:** Java provides a large library of pre-written classes grouped into packages.
*   **Key Packages:**
    1.  `java.lang`: Fundamental classes (String, Math, System). Imported automatically.
    2.  `java.util`: Utility classes like `Scanner`, `Date`, and the Collection Framework.
    3.  `java.io`: Classes for input and output operations (reading/writing files).
    4.  `java.net`: Classes for networking (Sockets, URL).
    5.  `java.awt`: Original GUI components (Button, Panel).
    6.  `javax.swing`: Modern, lightweight GUI components.

### 10. Error Types in Java
*   **1. Compile-time Errors:** Syntax errors caught by the compiler (e.g., missing semicolon, using an undeclared variable). The program won't run until these are fixed.
*   **2. Runtime Errors (Exceptions):** Occur during program execution (e.g., `ArithmeticException` like divide-by-zero, `NullPointerException`).
*   **3. Logical Errors:** The program runs without crashing but gives the wrong output because the logic is incorrect (e.g., using `+` instead of `*` in a formula).

### 11. Java Collection Framework
*   **Definition:** A unified architecture for representing and manipulating collections of objects (like lists, sets, and maps).
*   **Hierarchy:**
    *   **Interface:** `Collection` -> `List`, `Set`, `Queue`.
    *   **List Implementation:** `ArrayList`, `LinkedList`, `Vector`. (Allows duplicates, maintains order).
    *   **Set Implementation:** `HashSet`, `LinkedHashSet`. (No duplicates).
    *   **Map (Separate):** `HashMap`, `TreeMap`. (Key-Value pairs).
*   **Advantage:** Provides high-performance, standard data structures that reduce programming effort.

### 12. Events in Java
*   **Definition:** An event is an object that describes a state change in a source (e.g., a button click, a mouse movement).
*   **Event Handling (Delegation Model):**
    1.  **Event Source:** The UI component (e.g., `JButton`).
    2.  **Event Object:** Encapsulates details of the event (e.g., `ActionEvent`).
    3.  **Event Listener:** An interface that "listens" for the event and defines the action (e.g., `ActionListener`).
*   **Common Listeners:** `MouseListener`, `KeyListener`, `WindowListener`.

### 13. String Class & Methods
*   **Definition:** In Java, Strings are objects, not simple character arrays. They are **immutable**, meaning once created, their value cannot be changed.
*   **Key Methods:**
    1.  `length()`: Returns number of characters.
    2.  `charAt(index)`: Returns char at specific position.
    3.  `indexOf("str")`: Returns the first position of a substring.
    4.  `equals(s)`: Compares content (case-sensitive).
    5.  `substring(start, end)`: Extracts a part of the string.
*   **Note:** Use `StringBuilder` if you need a string that can be modified frequently.

### 14. Command Line Arguments
*   **Definition:** Arguments passed to a Java program during execution via the command prompt.
*   **Mechanism:** They are stored in the `String[] args` array of the `main` method.
*   **Example:** Running `java Test Hello 123`
    *   `args[0]` will be "Hello"
    *   `args[1]` will be "123"
*   **Use Case:** Providing dynamic input to a program without changing the source code.

### 15. Vector Class
*   **Definition:** A legacy class (part of `java.util`) that implements a growable array of objects. It is similar to `ArrayList` but is **synchronized**.
*   **Key Features:**
    1.  It is thread-safe (synchronized).
    2.  It doubles its size when full (by default).
*   **Example:**
    ```java
    Vector v = new Vector();
    v.add("Apple");
    v.addElement("Banana");
    System.out.println(v.get(0));
    ```

### 16. Exception Handling Keywords
*   **try:** Used to wrap the code that might throw an exception.
*   **catch:** Block used to handle the specific exception thrown.
*   **finally:** Block that always executes, used for cleanup (like closing files).
*   **throw:** Used to explicitly throw a single exception.
*   **throws:** Used in method signature to declare which exceptions the method might throw.

### 17. Character vs Byte Streams
*   **Byte Streams:**
    *   Handles data byte-by-byte (8 bits).
    *   Used for binary data like images and audio.
    *   Classes: `FileInputStream`, `FileOutputStream`.
*   **Character Streams:**
    *   Handles data character-by-character (16 bits Unicode).
    *   Used for text files.
    *   Classes: `FileReader`, `FileWriter`.
*   **Rule:** Always use Character streams for text data as they handle international characters better.

### 18. Wrapper Classes
*   **Definition:** Wrapper classes provide a way to use primitive data types as objects.
*   **Mapping:** `int` -> `Integer`, `char` -> `Character`, `double` -> `Double`, etc.
*   **Why needed?** Because the Collection Framework (like `ArrayList`) can only store objects, not primitives.
*   **Autoboxing:** Automatic conversion of primitive to wrapper (e.g., `Integer x = 5;`).
*   **Unboxing:** Automatic conversion of wrapper to primitive.

### 19. Abstract Class vs Final Class
*   **Abstract Class:**
    *   Declared with `abstract`.
    *   **Cannot be instantiated.**
    *   Can have both abstract (no body) and concrete methods.
    *   **Purpose:** To be inherited and provide a template.
*   **Final Class:**
    *   Declared with `final`.
    *   **Cannot be inherited.** (Prevents extension).
    *   All methods are implicitly final.
    *   **Purpose:** For security and performance (e.g., `String` class).

### 20. Java Environment (JDK, JRE, JVM)
*   **JVM (Java Virtual Machine):** An abstract machine that executes bytecode. It is the heart of platform independence.
*   **JRE (Java Runtime Environment):** JVM + Libraries. It is what you need to **run** a Java program.
*   **JDK (Java Development Kit):** JRE + Development Tools (like `javac` compiler, `jdb` debugger). It is what you need to **write and compile** Java programs.
*   **Relationship:** JDK contains JRE, and JRE contains JVM.
