# MSCIT-201: Object Oriented Concepts and Programming (Java)
## 10-Mark Questions (Important for Exam)

1.  **⭐⭐⭐ OOP Concepts in Java:** Explain basic concepts of OOP (Encapsulation, Polymorphism, Inheritance, Abstraction). Discuss how these are implemented in Java. (Repeated: Aug 2022, Jan 2023, July 2025)
2.  **⭐⭐⭐ JVM Architecture & Features:** Explain the Java Virtual Machine (JVM) architecture in detail. Discuss Java features like Platform Independence, Robustness, and Portability. (Repeated: Aug 2022, July 2023, July 2025)
3.  **⭐⭐⭐ Inheritance:** What is inheritance? Explain different types of inheritance (Single, Multilevel, Hierarchical) with a Java program. (Repeated: Aug 2022, Jan 2023, July 2023)
4.  **⭐⭐⭐ Constructors:** Explain the concept and usage of constructors and its types in Java with examples. (Repeated: Aug 2022, Jan 2023, July 2025)
5.  **⭐⭐⭐ Control Structures/Loops:** Explain different types of loops (for, while, do-while) and control structures available in Java with examples. (Repeated: Aug 2022, Jan 2023)
6.  **⭐⭐⭐ Java Collection Framework:** Explain the Java Collection Framework. Discuss how Lists, Sets, Maps, and Iterators work. (Repeated: July 2023, July 2025)
7.  **⭐⭐⭐ Exception Handling:** Describe the exception handling mechanism. Explain the use of `try`, `catch`, `finally`, `throw`, and `throws` with a program. (Repeated: Jan 2023, July 2025)
8.  **⭐⭐⭐ Multithreading:** How are threads created using the Thread class and Runnable interface? Explain the Thread Life Cycle and states in detail. (Repeated: Aug 2022, July 2023, July 2025)
9.  **⭐⭐⭐ Event Delegation Model:** Discuss the Event Delegation Model in Java. Explain how event sources, listeners, and event objects are connected. (Repeated: Aug 2022, July 2025)
10. **⭐⭐⭐ Package:** What is a Package? Explain the steps for defining and creating a package in Java. (Repeated: Aug 2022, Jan 2023, July 2023)
11. **⭐⭐ Method Overloading & Static Members:** Explain method overloading and static members in Java with examples. (Repeated: July 2025, Aug 2022)
12. **⭐⭐ AWT Components:** What is AWT? Discuss the class hierarchy of AWT and list its components. (Repeated: Aug 2022, July 2023)
13. **⭐⭐ String Handling:** Explain the String class and its methods in detail. (Repeated: Jan 2023, July 2023)
14. **⭐⭐ Vector Class:** Explain the Vector class with an example. (Repeated: Jan 2023, July 2023)
15. **⭐⭐ Graphics Class:** Explain the Graphics class with an example. (Repeated: July 2023)
16. **⭐⭐ Datatypes:** Explain different datatypes available in Java in detail. (Repeated: Aug 2022, Jan 2023)
17. **⭐⭐ Class, Properties, and Methods:** What is a class? What are properties and methods? Explain with a suitable example. (Repeated: Aug 2022, Jan 2023)
18. **⭐ Abstract vs Final Class:** Write the difference between an Abstract class and a Final class. (Repeated: July 2023)
19. **⭐ I/O Streams:** Explain Character streams and Byte streams. Discuss Java I/O streams in brief. (Repeated: July 2023, July 2025)
20. **⭐ Command Line Arguments:** Explain command line arguments in detail with an example. (Repeated: Jan 2023)

---

## Detailed Answers (10-Mark Questions)

### 1. Basic Concepts of OOP (Object-Oriented Programming)
Object-Oriented Programming is a paradigm that organizes software design around data, or objects, rather than functions and logic.

*   **1. Encapsulation (Data Hiding):**
    *   **Definition:** Wrapping data (variables) and code (methods) together into a single unit (Class).
    *   **Implementation:** Variables are made `private`, and access is granted via `public` getter and setter methods.
    *   **Benefit:** Protects data from unauthorized modification and increases modularity.
*   **2. Inheritance (Code Reusability):**
    *   **Definition:** Mechanism where one class acquires properties of another class.
    *   **Implementation:** Using the `extends` keyword for classes and `implements` for interfaces.
    *   **Benefit:** Reduces redundancy and creates a natural hierarchy (Parent-Child).
*   **3. Polymorphism (One Name, Many Forms):**
    *   **Definition:** Ability of a single method to perform different tasks.
    *   **Types:** 
        *   *Compile-time:* Method Overloading.
        *   *Runtime:* Method Overriding (Dynamic Method Dispatch).
*   **4. Abstraction (Hiding Complexity):**
    *   **Definition:** Displaying only essential information and hiding background details.
    *   **Implementation:** Using `abstract` classes and `interfaces`.
    *   **Example:** A car driver knows how to use the steering wheel (Interface) but doesn't need to know how the engine internal combustion works (Abstraction).

### 2. JVM Architecture & Java Features
The **Java Virtual Machine (JVM)** is an engine that provides a runtime environment to drive the Java Code or applications. It converts Java bytecode into machine language.

*   **JVM Architecture Components:**
    1.  **Class Loader:** Responsible for loading `.class` files into the memory area. It performs Loading, Linking, and Initialization.
    2.  **Memory Areas (Runtime Data Areas):**
        *   *Method Area:* Stores class structures, static variables, and method code.
        *   *Heap Area:* Stores all objects and their instance variables. It is shared by all threads.
        *   *Stack Area:* Stores local variables and method call stacks. A separate stack is created for every thread.
        *   *Program Counter (PC) Register:* Stores the address of the currently executing instruction.
        *   *Native Method Stack:* For native methods (written in C/C++).
    3.  **Execution Engine:** Contains the **Interpreter** (runs code line by line) and the **JIT Compiler** (Just-In-Time) which compiles "hot" code segments into native machine code to speed up execution.
    4.  **Garbage Collector (GC):** Automatically manages memory by reclaiming space from objects that are no longer reachable.

*   **Key Java Features:**
    *   **Platform Independence:** The compiler (`javac`) generates Bytecode, which can run on any OS that has a JVM.
    *   **Secure:** No explicit pointers, sandbox environment, and bytecode verifier.
    *   **Robust:** Strong memory management and mandatory Exception Handling.

### 3. Inheritance and Its Types
Inheritance is the process by which one object acquires all the properties and behaviors of a parent object.

*   **Types of Inheritance in Java:**
    1.  **Single Inheritance:** A class inherits from one superclass. (A -> B)
    2.  **Multilevel Inheritance:** A chain of inheritance. (A -> B -> C)
    3.  **Hierarchical Inheritance:** Multiple classes inherit from a single superclass.
    4.  **Multiple Inheritance (via Interfaces):** Java does not support multiple inheritance with classes (to avoid the Diamond Problem) but allows a class to implement multiple interfaces.
*   **Program Example:**
    ```java
    class Employee {
        float salary = 40000;
        void work() { System.out.println("Working..."); }
    }
    class Programmer extends Employee {
        int bonus = 10000;
        public static void main(String args[]) {
            Programmer p = new Programmer();
            p.work(); // Inherited method
            System.out.println("Salary: " + p.salary);
            System.out.println("Bonus: " + p.bonus);
        }
    }
    ```

### 4. Constructors in Detail
A constructor is a block of code similar to a method that is called when an instance of an object is created.

*   **Key Rules:**
    1.  Constructor name must be the same as the class name.
    2.  It must have no explicit return type (not even `void`).
    3.  It is called automatically by the `new` operator.
*   **Types of Constructors:**
    1.  **Default Constructor:** Provided by Java if no constructor is defined. It initializes data members with default values (0, null, etc.).
    2.  **No-Arg Constructor:** Programmer-defined constructor with no parameters.
    3.  **Parameterized Constructor:** Used to initialize objects with specific data during creation.
*   **Constructor Overloading:** Defining multiple constructors with different parameter lists.
*   **Example:**
    ```java
    class Student {
        int id; String name;
        Student() { id = 0; name = "Unknown"; } // No-arg
        Student(int i, String n) { id = i; name = n; } // Parameterized
        void display() { System.out.println(id + " " + name); }
    }
    ```

### 5. Control Structures and Loops
Control structures determine the flow of program execution based on conditions.

*   **1. Selection (Decision Making):**
    *   `if`, `if-else`, `if-else-if` ladder.
    *   `switch` statement: Allows a variable to be tested for equality against a list of values (cases).
*   **2. Iteration (Loops):**
    *   **for loop:** Used when the number of iterations is known. `for(init; condition; incr)`.
    *   **while loop:** Entry-controlled. Used when iterations are not fixed. Checks condition first.
    *   **do-while loop:** Exit-controlled. Executes the body at least once even if the condition is false.
*   **3. Jump Statements:**
    *   `break`: Terminates the loop/switch immediately.
    *   `continue`: Skips the current iteration and goes to the next.
*   **Example:** A `for` loop to print numbers 1 to 5.
    ```java
    for(int i=1; i<=5; i++) {
        System.out.println(i);
    }
    ```

### 6. Java Collection Framework
The Collection Framework provides an architecture to store and manipulate a group of objects. It includes Interfaces, Implementations (Classes), and Algorithms.

*   **Core Interfaces:**
    1.  **Collection:** The root interface.
    2.  **List:** An ordered collection that allows duplicates. Implementations: `ArrayList`, `Vector`, `LinkedList`.
    3.  **Set:** An unordered collection that does NOT allow duplicates. Implementations: `HashSet`, `LinkedHashSet`, `TreeSet`.
    4.  **Map:** A separate hierarchy (not under Collection). Stores Key-Value pairs. Implementations: `HashMap`, `TreeMap`.
*   **Iterators:** Objects used to traverse through a collection one by one. Methods: `hasNext()`, `next()`, `remove()`.
*   **Benefits:** Reduces development time, provides high-performance data structures, and promotes code reusability.

### 7. Exception Handling Mechanism
Exception handling is a powerful mechanism to handle runtime errors so that the normal flow of the application can be maintained.

*   **Keywords and Usage:**
    *   `try`: Encloses code that might throw an exception.
    *   `catch`: Handles the exception thrown by the `try` block.
    *   `finally`: Code that executes regardless of whether an exception was handled or not (e.g., closing a DB connection).
    *   `throw`: Used to explicitly throw an exception.
    *   `throws`: Used in method signatures to declare that the method might throw exceptions.
*   **Example Program:**
    ```java
    public class Test {
        public static void main(String args[]) {
            try {
                int a = 10 / 0;
            } catch (ArithmeticException e) {
                System.out.println("Error: " + e.getMessage());
            } finally {
                System.out.println("Execution completed.");
            }
        }
    }
    ```

### 8. Multithreading & Life Cycle
Multithreading in Java is a process of executing multiple threads simultaneously. A thread is a lightweight sub-process.

*   **Creating Threads:**
    1.  **Extending `Thread` class:** `class T extends Thread { public void run() { ... } }`.
    2.  **Implementing `Runnable` interface:** `class R implements Runnable { public void run() { ... } }`. This is preferred as it allows inheriting from another class.
*   **Thread Life Cycle (States):**
    1.  **New:** When a thread is created but not yet started.
    2.  **Runnable:** Ready to run and waiting for CPU.
    3.  **Running:** Currently executing instructions.
    4.  **Blocked/Waiting:** Waiting for I/O, a lock, or another thread (`sleep`, `wait`, `join`).
    5.  **Terminated:** When the `run()` method finishes.
*   **Methods:** `start()`, `run()`, `sleep()`, `join()`, `yield()`, `interrupt()`.

### 9. Event Delegation Model
Java uses the Delegation Event Model to handle GUI events (AWT/Swing).

*   **Components:**
    1.  **Event Source:** The UI component where the event originated (e.g., `JButton`, `JTextField`).
    2.  **Event Object:** Encapsulates the details of the event (e.g., `ActionEvent`, `MouseEvent`). It contains information like source and time.
    3.  **Event Listener:** An interface (e.g., `ActionListener`, `MouseListener`) that receives and processes the event.
*   **Mechanism:**
    1.  The user interacts with the **Source**.
    2.  The Source creates an **Event Object**.
    3.  The Source notifies all registered **Listeners** by passing the Event Object to their predefined methods.
*   **Registration:** Use methods like `addActionListener(this)` to connect a source to a listener.

### 10. Packages in Java
A package is a grouping of related classes, interfaces, and sub-packages.

*   **Steps to Create and Use a Package:**
    1.  **Declare:** First line of the file must be `package packagename;`.
    2.  **Define:** Create your classes and methods inside that file.
    3.  **Compile:** Use `javac -d . FileName.java`. The `-d` flag creates the necessary folder structure based on the package name.
    4.  **Import:** In another class, use `import packagename.ClassName;` or `import packagename.*;`
*   **Advantages:**
    1.  Prevents naming collisions (different packages can have classes with same name).
    2.  Controls access (can make members accessible only within the package).
    3.  Easy to organize large projects.

### 11. Method Overloading & Static Members
*   **Method Overloading:**
    *   Definition: Defining multiple methods in the same class with the same name but different parameters (number, type, or order).
    *   Purpose: Increases readability and consistency.
    *   Example: `add(int a, int b)` and `add(double a, double b)`.
*   **Static Members:**
    *   **Static Variable:** Belong to the class, not to any object. Shared by all instances. Memory is allocated once at class loading.
    *   **Static Method:** Can be called without creating an object (e.g., `Math.sqrt()`). It can only access static data and other static methods.
    *   **Static Block:** Used to initialize static variables. Runs once when the class is loaded.

### 12. AWT Class Hierarchy and Components
AWT (Abstract Window Toolkit) is Java's original GUI library.

*   **Hierarchy:**
    `Object -> Component -> Container -> Window -> Frame`.
    `Component -> Button, Canvas, Label, TextField, Checkbox`.
    `Container -> Panel -> Applet`.
*   **Key Components:**
    1.  **Button:** A clickable control.
    2.  **Label:** Displays a single line of read-only text.
    3.  **TextField:** Single-line text input.
    4.  **TextArea:** Multi-line text input.
    5.  **Checkbox:** A toggle option.
    6.  **Choice:** A dropdown list.
*   **Layout Managers:** `FlowLayout`, `BorderLayout`, `GridLayout`, `GridBagLayout`. They decide how components are arranged in a container.

### 13. String Handling in Java
Strings in Java are objects of the `java.lang.String` class.

*   **Key Feature:** Strings are **immutable**. Once created, their value cannot be changed. Any modification creates a new string object.
*   **StringBuffer vs StringBuilder:** Used for mutable strings. `StringBuffer` is synchronized (thread-safe); `StringBuilder` is faster but not thread-safe.
*   **Common Methods:**
    1.  `length()`, `charAt(index)`.
    2.  `concat(str)`, `toUpperCase()`, `toLowerCase()`.
    3.  `equals()`, `equalsIgnoreCase()`, `compareTo()`.
    4.  `substring(start, end)`, `trim()`, `replace(old, new)`.
    5.  `split(regex)`: Breaks string into an array based on a delimiter.
*   **String Pool:** A special memory area in the Heap where Java stores unique string literals to save space.

### 14. Vector Class with Example
The `Vector` class is a dynamic array of objects. It implements the `List` interface.

*   **Key Features:**
    1.  **Dynamic Sizing:** It can grow or shrink as needed.
    2.  **Synchronized:** It is thread-safe (safe for use in multithreaded environments).
    3.  **Legacy:** It was part of Java 1.0 but later joined the Collection framework.
*   **Example:**
    ```java
    import java.util.*;
    public class VectorTest {
        public static void main(String args[]) {
            Vector<String> v = new Vector<String>();
            v.add("Java");
            v.add("C++");
            v.addElement("PHP"); // Legacy method
            System.out.println("Size: " + v.size());
            System.out.println("First element: " + v.get(0));
        }
    }
    ```

### 15. Graphics Class with Example
The `Graphics` class is part of the `java.awt` package and provides methods for drawing text and shapes on a component.

*   **Common Methods:**
    1.  `drawRect(x, y, w, h)`, `fillRect(x, y, w, h)`.
    2.  `drawOval(x, y, w, h)`, `fillOval(x, y, w, h)`.
    3.  `drawLine(x1, y1, x2, y2)`.
    4.  `drawString("text", x, y)`.
    5.  `setColor(Color c)`, `setFont(Font f)`.
*   **Example (Applet/Component):**
    ```java
    public void paint(Graphics g) {
        g.setColor(Color.BLUE);
        g.drawRect(10, 10, 100, 50);
        g.setColor(Color.RED);
        g.drawString("Hello Java Graphics", 10, 80);
    }
    ```

### 16. Java Datatypes in Detail
Data types specify the size and type of values that can be stored in variables.

*   **1. Primitive Types (Fixed Size):**
    *   **Integers:** `byte`(1), `short`(2), `int`(4), `long`(8).
    *   **Floating-Point:** `float`(4), `double`(8).
    *   **Character:** `char`(2 bytes, uses Unicode).
    *   **Boolean:** `boolean` (true/false).
*   **2. Non-Primitive (Reference) Types:**
    *   **Classes, Interfaces, Arrays.**
    *   These store memory addresses. Default value is `null`.
*   **Type Casting:**
    *   *Widening (Implicit):* Small type to large type. No data loss.
    *   *Narrowing (Explicit):* Large type to small type. Requires manual casting. `int x = (int)10.5;`.

### 17. Class, Properties, and Methods
*   **Class:** A blueprint or template for creating objects. It defines the structure and behavior of objects.
*   **Properties (Fields/Data Members):** Represent the state or characteristics of an object.
*   **Methods (Member Functions):** Represent the behavior or actions an object can perform.
*   **Example:**
    ```java
    class Car {
        String color; // Property
        int speed;    // Property
        void accelerate() { // Method
            speed += 10;
            System.out.println("Speed is " + speed);
        }
    }
    ```
*   **Analogy:** A "Car" class is a drawing/specification. An "Audi" object is a physical car built using that specification.

### 18. Abstract Class vs Final Class
*   **Abstract Class:**
    *   Declared with the `abstract` keyword.
    *   **Cannot be instantiated.**
    *   Can have both abstract methods (without body) and concrete methods.
    *   Used to provide a base template for other classes.
*   **Final Class:**
    *   Declared with the `final` keyword.
    *   **Cannot be inherited** (cannot have child classes).
    *   Used for security and performance.
    *   Example: `String`, `Math`, `System` classes in Java are final.
*   **Key Difference:** Abstract classes MUST be inherited to be useful; Final classes CANNOT be inherited.

### 19. Java I/O Streams (Character vs Byte)
A stream is a sequence of data. Java I/O is based on streams.

*   **1. Byte Streams (8-bit):**
    *   Handle data byte by byte.
    *   Used for reading/writing binary data like images, audio, video.
    *   Classes: `InputStream` and `OutputStream` (Superclasses). Subclasses: `FileInputStream`, `FileOutputStream`.
*   **2. Character Streams (16-bit):**
    *   Handle data character by character using Unicode.
    *   Used for reading/writing text files.
    *   Classes: `Reader` and `Writer` (Superclasses). Subclasses: `FileReader`, `FileWriter`.
*   **Buffered Streams:** Wrappers that improve efficiency by using a buffer. `BufferedReader`, `BufferedWriter`.

### 20. Command Line Arguments in Detail
Command line arguments are used to provide input to a program during its execution from the terminal.

*   **Working:** Arguments are passed after the class name: `java ClassName arg1 arg2`.
*   **Storage:** They are stored in the `String[] args` array of the `main` method.
*   **Example:**
    ```java
    public class CommandTest {
        public static void main(String[] args) {
            System.out.println("First Argument: " + args[0]);
            int n = Integer.parseInt(args[1]); // Conversion
            System.out.println("Second as int: " + n);
        }
    }
    ```
*   **Note:** If you try to access an index that wasn't provided (e.g., `args[0]` when no arguments were given), you will get an `ArrayIndexOutOfBoundsException`.
