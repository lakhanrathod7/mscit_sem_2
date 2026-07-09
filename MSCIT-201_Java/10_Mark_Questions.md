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

### 1. Basic Concepts of OOP
*   **1. Encapsulation:** The process of wrapping data (variables) and code (methods) together as a single unit (Class). It ensures **data hiding** by making variables `private` and providing `public` getter/setter methods to access them.
*   **2. Inheritance:** A mechanism where one class (Subclass/Child) acquires the properties and behaviors of another class (Superclass/Parent). It promotes **code reusability**. Keywords: `extends` and `implements`.
*   **3. Polymorphism:** The ability of a single action to perform in different ways.
    *   *Compile-time Polymorphism:* Method Overloading (same name, different parameters).
    *   *Runtime Polymorphism:* Method Overriding (subclass provides specific implementation of parent method).
*   **4. Abstraction:** Hiding internal complexity and showing only essential features to the user. Achieved in Java using **Abstract Classes** (0-100% abstraction) and **Interfaces** (100% abstraction).
*   **5. Class and Object:** A **Class** is a blueprint/template, and an **Object** is a physical instance of that class.

### 2. JVM Architecture & Java Features
*   **JVM Architecture Components:**
    1.  **Class Loader:** Loads `.class` files into memory when needed.
    2.  **Memory Areas:**
        *   *Stack:* Stores local variables and method calls.
        *   *Heap:* Stores all created objects.
        *   *Method Area:* Stores class-level data and static variables.
    3.  **Execution Engine:** Contains the **Interpreter** (reads bytecode) and **JIT Compiler** (Just-In-Time) which optimizes performance by compiling frequently used code into native machine code.
    4.  **Garbage Collector:** Automatically deletes unused objects from the Heap to free memory.
*   **Java Features:**
    *   **Platform Independence:** Java code is compiled into Bytecode, which can run on any OS with a JVM.
    *   **Robustness:** Strong memory management, lack of pointers, and mandatory exception handling.
    *   **Portability:** "Write Once, Run Anywhere" (WORA).

### 3. Inheritance & Its Types
*   **Definition:** Inheritance allows a class to derive properties from another class.
*   **Types in Java:**
    1.  **Single Inheritance:** One subclass inherits from one superclass.
    2.  **Multilevel Inheritance:** A class inherits from a subclass (A -> B -> C).
    3.  **Hierarchical Inheritance:** Multiple subclasses inherit from one superclass.
    *   **Note:** Java does **not** support "Multiple Inheritance" (one class inheriting from two classes) to avoid ambiguity (Diamond Problem). It is achieved using **Interfaces**.
*   **Example Program:**
    ```java
    class Animal { void eat() { System.out.println("Eating..."); } }
    class Dog extends Animal { void bark() { System.out.println("Barking..."); } }
    // Dog object can call both bark() and eat().
    ```

### 4. Constructors & Their Types
*   **Definition:** A special method used to initialize objects. It has the same name as the class and no return type.
*   **Key Characteristics:**
    1.  Called automatically when an object is created.
    2.  Cannot be `static`, `abstract`, or `final`.
*   **Types:**
    1.  **Default Constructor:** Created by compiler if none is defined.
    2.  **Parameterized Constructor:** Used to provide distinct values to different objects during creation.
    3.  **Copy Constructor:** Used to create an object using another object of the same class as a template.
*   **Example:** `Student s1 = new Student("Amit", 101);`

### 5. Control Structures & Loops
*   **1. Selection Statements:**
    *   `if-else`: Executing a block based on a boolean condition.
    *   `switch`: Selecting one of many code blocks to be executed based on a variable's value.
*   **2. Iteration (Loops):**
    *   `for loop`: Best when the number of iterations is fixed.
    *   `while loop`: Entry-controlled; checks condition before executing.
    *   `do-while loop`: Exit-controlled; executes the body at least once even if the condition is false.
*   **3. Jump Statements:**
    *   `break`: Exits the loop or switch.
    *   `continue`: Skips the current iteration and moves to the next.

### 6. Java Collection Framework
*   **Definition:** A set of classes and interfaces that implement commonly used data structures.
*   **Core Interfaces:**
    1.  **List:** Ordered collection that allows duplicates (`ArrayList`, `LinkedList`).
    2.  **Set:** Collection that does not allow duplicates (`HashSet`, `TreeSet`).
    3.  **Map:** Stores Key-Value pairs (`HashMap`, `TreeMap`).
*   **Iterators:** An object that allows you to traverse through any collection one by one. Use `iterator()` method to get an instance.
*   **Advantage:** Provides interoperability between different types of collections and reduces coding effort.

### 7. Exception Handling Mechanism
*   **Definition:** A way to handle runtime errors so the program doesn't crash.
*   **Keywords:**
    *   `try`: Code that might cause an error.
    *   `catch`: Code to handle the error.
    *   `finally`: Code that must run (cleanup).
    *   `throw`: Explicitly triggers an error.
    *   `throws`: Declares that a method might throw an exception.
*   **Program Snippet:**
    ```java
    try {
        int data = 100/0;
    } catch(ArithmeticException e) {
        System.out.println("Cannot divide by zero");
    } finally {
        System.out.println("Done.");
    }
    ```

### 8. Multithreading & Life Cycle
*   **Ways to Create Threads:**
    1.  **By Extending `Thread` Class:** `class MyThread extends Thread { public void run() { ... } }`
    2.  **By Implementing `Runnable` Interface:** `class MyThread implements Runnable { ... }` (Better as it allows inheriting from another class).
*   **Thread Life Cycle:**
    1.  **New:** Thread object is created.
    2.  **Runnable:** `start()` method is called.
    3.  **Running:** Thread gets CPU time.
    4.  **Blocked:** Waiting for I/O or a lock.
    5.  **Terminated:** `run()` method finishes.

### 9. Event Delegation Model
*   **Definition:** The modern way of handling events in Java AWT/Swing.
*   **Components:**
    1.  **Event Source:** The UI component where the action happens (e.g., Button).
    2.  **Event Object:** Created by the source, contains details of the event (e.g., `ActionEvent`).
    3.  **Event Listener:** An interface implemented by the class that wants to handle the event.
*   **The Process:** The source "registers" the listener (e.g., `button.addActionListener(this)`). When the event occurs, the source calls the listener's method and passes the Event Object to it.

### 10. Packages in Java
*   **Definition:** A package is a container for grouping related classes, interfaces, and sub-packages.
*   **Steps to Create:**
    1.  Define the package name at the top: `package mypack;`
    2.  Create the class: `public class MyClass { ... }`
    3.  Compile with directory flag: `javac -d . MyClass.java` (This creates a folder named `mypack`).
*   **Using a Package:** Use the `import` statement: `import mypack.MyClass;`
*   **Benefits:** Avoids naming conflicts and provides access protection.

### 11. Method Overloading & Static Members
*   **Method Overloading:**
    *   Same method name but different parameter list (number or type).
    *   Example: `add(int a, int b)` and `add(int a, int b, int c)`.
*   **Static Members:**
    *   **Static Variable:** Shared by all instances of the class. Only one copy exists in memory.
    *   **Static Method:** Can be called without creating an object. It can only access static data.
    *   Example: `Math.sqrt()` is a static method.

### 12. AWT Components & Hierarchy
*   **Hierarchy:** `Object` -> `Component` -> `Container` -> `Window` -> `Frame`.
*   **Key Components:**
    *   **Label:** Displaying text.
    *   **Button:** Triggering actions.
    *   **TextField:** Single-line input.
    *   **Checkbox:** Multiple choice selection.
    *   **Choice/List:** Dropdown or list of items.
*   **Layout Managers:** `FlowLayout`, `BorderLayout`, `GridLayout` are used to arrange these components.

### 13. String Handling in Detail
*   **String vs StringBuffer:** `String` is immutable (fixed), while `StringBuffer` is mutable (can be changed).
*   **Key Methods:** `concat()`, `split()`, `trim()`, `replace()`, `toLowerCase()`, `toUpperCase()`, `equals()`, `equalsIgnoreCase()`.
*   **String Pool:** Java stores literal strings in a special memory area to save space. If two strings have the same literal value, they point to the same memory location.

### 14. Vector Class with Example
*   **Definition:** A dynamic array that can grow or shrink. It is synchronized (thread-safe).
*   **Example:**
    ```java
    Vector v = new Vector(3, 2); // Initial capacity 3, capacity increment 2
    v.add("A"); v.add("B"); v.add("C");
    v.add("D"); // Capacity becomes 5 (3+2)
    System.out.println("Size: " + v.size());
    ```

### 15. Graphics Class with Example
*   **Definition:** Part of `java.awt`, used to draw shapes, text, and images on the screen.
*   **Methods:** `drawLine()`, `drawRect()`, `fillRect()`, `drawOval()`, `drawString()`, `setColor()`.
*   **Example (Applet/Frame):**
    ```java
    public void paint(Graphics g) {
        g.setColor(Color.red);
        g.drawOval(10, 10, 50, 50);
        g.drawString("Java Graphics", 20, 100);
    }
    ```

### 16. Java Datatypes in Detail
*   **Primitive Types:** 8 types (byte, short, int, long, float, double, char, boolean). Each has a fixed size across all platforms.
*   **Reference Types:** Store memory addresses. Includes Classes, Interfaces, and Arrays.
*   **Type Casting:**
    *   **Widening (Implicit):** Converting small to large (e.g., `int` to `double`). No data loss.
    *   **Narrowing (Explicit):** Converting large to small (e.g., `double` to `int`). Requires `(int)` and might lose data.

### 17. Class, Properties, and Methods
*   **Class:** A blueprint (e.g., `Car`).
*   **Properties (Fields):** State of the object (e.g., `color`, `speed`).
*   **Methods:** Behavior of the object (e.g., `start()`, `brake()`).
*   **Example:**
    ```java
    class Student {
        String name; // Property
        void study() { System.out.println(name + " is studying"); } // Method
    }
    ```

### 18. Abstract Class vs Interface
*   **Abstract Class:** Can have both abstract and non-abstract methods. Can have instance variables. Use `extends`.
*   **Interface:** (Before Java 8) can only have abstract methods. All variables are `public static final`. Use `implements`.
*   **Difference:** A class can implement multiple interfaces but can only extend one abstract class.

### 19. I/O Streams (Character vs Byte)
*   **Byte Streams:** Work with 8-bit bytes. Classes like `FileInputStream`, `FileOutputStream`. Good for images/video.
*   **Character Streams:** Work with 16-bit Unicode. Classes like `FileReader`, `FileWriter`. Best for text/international characters.
*   **Serialization:** The process of converting an object into a byte stream to save it to a file.

### 20. Command Line Arguments in Detail
*   **Definition:** Arguments passed during program startup.
*   **Access:** `public static void main(String[] args)`.
*   **Example:** `java MyApp 10 20`.
    ```java
    int num1 = Integer.parseInt(args[0]);
    int num2 = Integer.parseInt(args[1]);
    System.out.println("Sum: " + (num1 + num2));
    ```
*   **Key points:** Always passed as Strings. Conversion (like `Integer.parseInt`) is often necessary.
