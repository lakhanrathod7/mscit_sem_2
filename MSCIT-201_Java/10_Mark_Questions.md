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
**Introduction:**
Object-Oriented Programming is a paradigm that organizes software design around data, or objects, rather than functions and logic. It aims to implement real-world entities like inheritance, hiding, polymorphism, etc.

*   **1. Encapsulation (Data Hiding):**
    *   **Definition:** Wrapping data (variables) and code (methods) together into a single unit (Class).
    *   **Implementation:** Variables are made `private`, and access is granted via `public` getter and setter methods.
    *   **Benefit:** Protects data from unauthorized modification and increases modularity.
    *   **Example:**
        ```java
        class Employee {
            private double salary; // Encapsulated data
            public void setSalary(double s) { if(s > 0) salary = s; }
            public double getSalary() { return salary; }
        }
        ```
*   **2. Inheritance (Code Reusability):**
    *   **Definition:** Mechanism where one class (Subclass) acquires properties of another class (Superclass).
    *   **Implementation:** Using the `extends` keyword for classes and `implements` for interfaces.
    *   **Benefit:** Reduces redundancy and creates a natural hierarchy.
*   **3. Polymorphism (One Name, Many Forms):**
    *   **Definition:** Ability of a single method to perform different tasks.
    *   **Types:** 
        *   *Compile-time:* Method Overloading (same name, different parameters).
        *   *Runtime:* Method Overriding (subclass provides specific implementation of a parent method). Java uses **Dynamic Method Dispatch** for this.
*   **4. Abstraction (Hiding Complexity):**
    *   **Definition:** Displaying only essential information and hiding background details.
    *   **Implementation:** Using `abstract` classes (0-100% abstraction) and `interfaces` (100% abstraction).
    *   **Example:** A car driver knows how to use the steering wheel (Interface) but doesn't need to know the engine mechanics (Abstraction).

---

### 2. JVM Architecture & Java Features
**Introduction:**
The **Java Virtual Machine (JVM)** is the heart of Java's "Write Once, Run Anywhere" philosophy. It provides a runtime environment to execute Java bytecode.

**JVM Architecture Components:**
1.  **Class Loader Subsystem:** Responsible for **Loading** (.class files), **Linking** (Verification, Preparation, Resolution), and **Initialization**.
2.  **Runtime Data Areas (Memory):**
    *   *Method Area:* Stores class structures, static variables, and constant pool.
    *   *Heap Area:* Stores all objects and their instance variables. (Shared by all threads).
    *   *Stack Area:* Stores local variables and method call stacks. (Separate for every thread).
    *   *PC Register:* Stores the address of the current execution point.
    *   *Native Method Stack:* For native C/C++ method calls.
3.  **Execution Engine:**
    *   *Interpreter:* Reads bytecode and executes instructions one by one.
    *   *JIT (Just-In-Time) Compiler:* Compiles frequently used code into native machine code to improve performance.
    *   *Garbage Collector (GC):* Automatically reclaims memory from objects that are no longer reachable.

**Key Java Features:**
*   **Platform Independence:** The compiler generates Bytecode, which can run on any OS that has a JVM.
*   **Robustness:** Strong memory management, absence of pointers, and mandatory Exception Handling.
*   **Portability:** Neutral bytecode and standard libraries make it easy to move apps across systems.
*   **Security:** Sandbox environment and bytecode verification prevent unauthorized access.

---

### 3. Inheritance and Its Types
**Definition:**
Inheritance is the process by which one object acquires all the properties and behaviors of a parent object. It represents the **"IS-A" relationship**.

**Types of Inheritance in Java:**
1.  **Single Inheritance:** A subclass inherits from one superclass (A -> B).
2.  **Multilevel Inheritance:** A chain of inheritance (A -> B -> C).
3.  **Hierarchical Inheritance:** Multiple subclasses inherit from a single superclass (A -> B, A -> C).
4.  **Multiple Inheritance:** Java does **not** support multiple inheritance with classes to avoid the **Diamond Problem** (ambiguity). However, it is supported via **Interfaces**.

**Program Example:**
```java
class Animal {
    void eat() { System.out.println("Eating..."); }
}
class Dog extends Animal {
    void bark() { System.out.println("Barking..."); }
    public static void main(String args[]) {
        Dog d = new Dog();
        d.eat();  // Inherited
        d.bark(); // Own
    }
}
```

---

### 4. Constructors in Detail
**Definition:**
A constructor is a special block of code, similar to a method, that is called automatically when an instance of an object is created.

**Key Rules:**
1. Constructor name must be exactly the same as the class name.
2. It must have no explicit return type (not even `void`).
3. It is called only once per object lifecycle (during `new`).

**Types of Constructors:**
1.  **Default Constructor:** Automatically provided by Java if the programmer defines no constructor. Initializes members with default values (0, null).
2.  **No-Arg Constructor:** Programmer-defined constructor with no parameters.
3.  **Parameterized Constructor:** Used to initialize objects with specific data at creation.
4.  **Constructor Overloading:** Defining multiple constructors with different parameter lists in the same class.

**Example:**
```java
class Student {
    int id; String name;
    Student() { id = 0; name = "New"; } // No-arg
    Student(int i, String n) { id = i; name = n; } // Parameterized
}
```

---

### 5. Control Structures and Loops
Control structures determine the flow of program execution based on conditions.

*   **1. Selection (Decision Making):**
    *   `if`, `if-else`, `if-else-if` ladder: Used for boolean conditions.
    *   `switch` statement: Tests a variable against a list of constant values (cases).
*   **2. Iteration (Loops):**
    *   **for loop:** Used when the number of iterations is known. `for(init; cond; incr)`.
    *   **while loop:** Entry-controlled. Used when the iteration count is unknown. Checks condition first.
    *   **do-while loop:** Exit-controlled. Executes the body at least once, even if the condition is false.
*   **3. Jump Statements:**
    *   `break`: Terminates the current loop or switch immediately.
    *   `continue`: Skips the current iteration and moves to the next one.

---

### 6. Java Collection Framework
**Introduction:**
The Collection Framework is a unified architecture for representing and manipulating collections of objects. It provides high-performance, standard data structures.

**Core Interfaces & Classes:**
1.  **List (Interface):** An ordered collection that allows duplicates.
    *   *Implementations:* `ArrayList` (fast access), `LinkedList` (fast insert/delete), `Vector` (synchronized).
2.  **Set (Interface):** An unordered collection that does NOT allow duplicates.
    *   *Implementations:* `HashSet` (hashtable), `TreeSet` (sorted).
3.  **Map (Interface):** Stores data in **Key-Value** pairs. Keys must be unique.
    *   *Implementations:* `HashMap` (fast), `TreeMap` (sorted keys).
4.  **Iterator:** An object used to traverse through any collection one by one. Methods: `hasNext()`, `next()`, `remove()`.

**Benefits:** Reduces programming effort, increases performance, and allows interoperability between unrelated APIs.

---

### 7. Exception Handling Mechanism
**Introduction:**
Exception handling is a powerful mechanism to handle runtime errors (like divide by zero, file not found) so that the normal flow of the application can be maintained.

**Keywords:**
*   `try`: Encloses code that might throw an exception.
*   `catch`: Handles the exception thrown by the corresponding `try` block.
*   `finally`: Code that executes regardless of whether an exception was handled or not (used for cleanup).
*   `throw`: Used to explicitly throw an exception.
*   `throws`: Declared in method signatures to warn callers about potential checked exceptions.

**Example Program:**
```java
public class ExceptionTest {
    public static void main(String args[]) {
        try {
            int result = 10 / 0; // Throws ArithmeticException
        } catch (ArithmeticException e) {
            System.out.println("Error: " + e.getMessage());
        } finally {
            System.out.println("Cleanup successful.");
        }
    }
}
```

---

### 8. Multithreading & Thread Life Cycle
**Introduction:**
Multithreading in Java is a process of executing multiple threads simultaneously to maximize CPU utilization. A thread is a lightweight sub-process.

**Creating Threads:**
1.  **Extending `Thread` class:** `class T extends Thread { public void run() { ... } }`.
2.  **Implementing `Runnable` interface:** `class R implements Runnable { public void run() { ... } }`. This is preferred as it allows the class to extend another class.

**Thread Life Cycle (States):**
1.  **New:** Thread object is created but `start()` not yet called.
2.  **Runnable:** Ready to run and waiting for CPU time.
3.  **Running:** Currently executing instructions in `run()`.
4.  **Blocked/Waiting:** Waiting for an event (I/O, lock, or `sleep()`).
5.  **Terminated (Dead):** `run()` method has finished execution.

---

### 9. Event Delegation Model
**Introduction:**
Java uses the **Delegation Event Model** to handle GUI interactions (like button clicks) in AWT and Swing.

**Key Components:**
1.  **Event Source:** The UI component where the event originated (e.g., `JButton`, `JTextField`). It generates the event object.
2.  **Event Object:** Encapsulates details of the event (e.g., `ActionEvent`, `MouseEvent`). Contains source and timestamp.
3.  **Event Listener:** An interface that receives and processes the event. The listener class must implement specific methods (e.g., `actionPerformed()`).

**The Mechanism:**
1. The **Source** registers a **Listener** (e.g., `btn.addActionListener(this)`).
2. When the user interacts with the Source, it creates an **Event Object**.
3. The Source then **delegates** the task to the registered Listener by calling its event-handling method.

---

### 10. Packages in Java
**Definition:**
A package is a grouping of related classes, interfaces, and sub-packages. It acts as a container for classes.

**Steps to Create and Use a Package:**
1.  **Declare:** The first line of the file must be `package packagename;`.
2.  **Define:** Create classes and methods inside that file.
3.  **Compile:** Use `javac -d . FileName.java`. The `-d` flag creates the folder structure automatically based on the package name.
4.  **Import:** Use `import packagename.ClassName;` or `import packagename.*;` in other classes.

**Advantages:**
*   **Naming Privacy:** Prevents naming collisions.
*   **Access Control:** Allows making members accessible only within the package.
*   **Organization:** Makes large projects easier to manage.

---

### 11. Method Overloading & Static Members
*   **Method Overloading:**
    *   **Definition:** Defining multiple methods in the same class with the same name but different parameters (number, type, or order).
    *   **Purpose:** Increases readability and consistency.
    *   **Example:** `add(int a, int b)` and `add(double a, double b)`.
*   **Static Members:**
    *   **Static Variable:** Belongs to the class, not instances. One copy shared by all objects. Memory is allocated once during class loading.
    *   **Static Method:** Can be called without creating an object. Can only access static data. (e.g., `Math.sqrt()`).
    *   **Static Block:** Used to initialize static variables. Executes once when the class is first loaded into memory.

---

### 12. AWT Class Hierarchy and Components
**Introduction:**
AWT (Abstract Window Toolkit) is Java's original, platform-dependent GUI library.

**Class Hierarchy:**
`Object` -> `Component` -> `Container` -> `Window` -> `Frame`.
`Component` subclasses include `Button`, `Label`, `TextField`, `Checkbox`.
`Container` subclasses include `Panel` and `Window`.

**Key Components:**
1.  **Frame:** The main window with title and border.
2.  **Button:** A clickable control to trigger actions.
3.  **Label:** Used to display a single line of read-only text.
4.  **TextField:** Single-line user input box.
5.  **TextArea:** Multi-line user input box.
6.  **Layout Managers:** `FlowLayout` (sequential), `BorderLayout` (NSEW), `GridLayout` (rows/cols).

---

### 13. String Handling in Java
**Introduction:**
Strings in Java are objects of the `java.lang.String` class.

**Key Feature - Immutability:**
Once created, the value of a String object cannot be changed. Any modification creates a new String object. This is for security and memory efficiency (String Pool).

**StringBuffer vs StringBuilder:**
Both are used for **mutable** strings. `StringBuffer` is synchronized (thread-safe), while `StringBuilder` is faster but not thread-safe.

**Common Methods:**
1. `length()`, `charAt(index)`.
2. `concat(str)`, `toUpperCase()`, `toLowerCase()`.
3. `equals(str)`, `equalsIgnoreCase(str)`, `compareTo(str)`.
4. `substring(start, end)`, `trim()`, `replace(old, new)`.
5. `split(regex)`: Converts string to array based on delimiter.

---

### 14. Vector Class with Example
**Introduction:**
The `Vector` class implements a growable array of objects. It is part of the original Java API but now implements the `List` interface.

**Key Features:**
1.  **Dynamic Sizing:** Grows automatically when full.
2.  **Synchronized:** It is thread-safe (legacy class).
3.  **Insertion Order:** It maintains the sequence of elements.

**Example:**
```java
import java.util.*;
public class VectorDemo {
    public static void main(String args[]) {
        Vector<String> v = new Vector<String>(2); // Initial capacity 2
        v.add("Java");
        v.add("UML");
        v.add("LAMP"); // Grows automatically
        System.out.println("Size: " + v.size());
        System.out.println("First: " + v.get(0));
    }
}
```

---

### 15. Graphics Class with Example
**Introduction:**
The `Graphics` class (in `java.awt`) provides the drawing context for components. It allows drawing text, lines, and shapes.

**Common Methods:**
1.  `drawLine(x1, y1, x2, y2)`
2.  `drawRect(x, y, w, h)`, `fillRect(x, y, w, h)`
3.  `drawOval(x, y, w, h)`, `fillOval(x, y, w, h)`
4.  `drawString("text", x, y)`
5.  `setColor(Color c)`, `setFont(Font f)`

**Example (Inside a paint method):**
```java
public void paint(Graphics g) {
    g.setColor(Color.RED);
    g.drawRect(20, 20, 100, 50);
    g.setColor(Color.BLUE);
    g.drawString("Java Graphics", 25, 80);
}
```

---

### 16. Java Datatypes in Detail
**1. Primitive Datatypes (Fixed Size):**
*   **Integer types:** `byte` (1), `short` (2), `int` (4), `long` (8).
*   **Floating-point:** `float` (4), `double` (8).
*   **Character:** `char` (2 bytes, uses Unicode).
*   **Boolean:** `boolean` (true/false).
**2. Non-Primitive (Reference) Types:**
*   Includes **Classes**, **Interfaces**, and **Arrays**.
*   They store memory addresses. Default value is `null`.

**Type Casting:**
*   *Widening (Implicit):* Small type to large type (e.g., int to double). Automatic.
*   *Narrowing (Explicit):* Large type to small type (e.g., double to int). Requires manual cast: `int x = (int)10.5;`.

---

### 17. Class, Properties, and Methods
**Class:** A blueprint or template for creating objects. It defines a new data type.
**Properties (Fields/Variables):** Represent the **state** or attributes of an object (e.g., `color`, `speed`).
**Methods (Functions):** Represent the **behavior** or actions an object can perform (e.g., `accelerate()`, `brake()`).

**Example:**
```java
class Car {
    String model; // Property
    int speed;    // Property
    void showSpeed() { // Method
        System.out.println("Speed: " + speed);
    }
}
```
**Analogy:** A Class is like an architect's drawing of a house; an Object is the actual house built from that drawing.

---

### 18. Abstract Class vs Final Class
*   **Abstract Class:**
    *   Declared with `abstract`.
    *   **Cannot be instantiated.**
    *   Used to provide a base template for subclasses.
    *   Can have both abstract methods (no body) and concrete methods.
*   **Final Class:**
    *   Declared with `final`.
    *   **Cannot be inherited** (cannot have child classes).
    *   Used for security and performance.
    *   Example: `String`, `Math`, and `System` classes in Java are final.
*   **Key Difference:** Abstract classes MUST be inherited to be useful; Final classes CANNOT be inherited.

---

### 19. Java I/O Streams (Character vs Byte)
**Introduction:**
A stream is a sequence of data. Java I/O is based on streams.

**1. Byte Streams (8-bit):**
*   Handle data byte by byte.
*   Used for binary data like images, audio, video.
*   Superclasses: `InputStream`, `OutputStream`.
*   Subclasses: `FileInputStream`, `FileOutputStream`.
**2. Character Streams (16-bit):**
*   Handle data character by character using Unicode.
*   Used for text files.
*   Superclasses: `Reader`, `Writer`.
*   Subclasses: `FileReader`, `FileWriter`.
**Buffered Streams:** Wrappers like `BufferedReader` improve performance by reducing the number of I/O operations.

---

### 20. Command Line Arguments in Detail
**Definition:**
Arguments passed to a program during its execution from the terminal or command prompt.

**Working:**
*   They are stored in the `String[] args` array parameter of the `main` method.
*   `args[0]` is the first argument, `args[1]` is the second, and so on.
*   `args.length` tells how many arguments were passed.

**Example:**
```java
public class CmdTest {
    public static void main(String[] args) {
        System.out.println("First arg: " + args[0]);
        // Convert string to int if needed
        int n = Integer.parseInt(args[1]);
    }
}
```
**Note:** Accessing an index that doesn't exist (e.g., `args[0]` when no arguments are given) results in an `ArrayIndexOutOfBoundsException`.
