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
Object-Oriented Programming (OOP) is a paradigm that organizes software design around data, or objects, rather than functions and logic. An object is a real-world entity with a state (attributes) and behavior (methods). Java implements OOP through four fundamental pillars:

**1. Encapsulation (Data Hiding):**
*   **Definition:** Wrapping data (variables) and code (methods) together into a single unit (Class). It protects an object's internal state from unauthorized access.
*   **Analogy:** A medical capsule. The medicine (data) is hidden inside the capsule (class).
*   **Implementation:** 
    1. Declare class variables as `private`.
    2. Provide `public` getter and setter methods to access/modify them.
*   **Example:**
    ```java
    class BankAccount {
        private double balance; // Hidden data
        public double getBalance() { return balance; } // Accessor
        public void deposit(double amt) { if(amt > 0) balance += amt; } // Mutator
    }
    ```

**2. Inheritance (Code Reusability):**
*   **Definition:** A process where one class (Subclass/Child) acquires the properties and behaviors of another class (Superclass/Parent).
*   **Implementation:** Using the `extends` keyword.
*   **Example:** A `Smartphone` inherits from a `BasicPhone`.
    ```java
    class Animal { void eat() { System.out.println("Eating..."); } }
    class Dog extends Animal { void bark() { System.out.println("Barking..."); } }
    ```

**3. Polymorphism (One Name, Many Forms):**
*   **Definition:** The ability of an object or method to perform differently in different contexts.
*   **Types:**
    *   **Compile-time (Overloading):** Multiple methods with the same name but different parameters (number, type, or order).
    *   **Runtime (Overriding):** A subclass provides a specific implementation for a method already defined in its parent. Java uses **Dynamic Method Dispatch** to decide which version to call at runtime.
*   **Example:** A `Shape` class has a `draw()` method. `Circle` and `Square` override `draw()` to draw their respective shapes.

**4. Abstraction (Hiding Complexity):**
*   **Definition:** Showing only essential features to the user while hiding internal background details.
*   **Implementation:** Using `abstract` classes and `interfaces`.
*   **Example:** A TV remote. You only see the buttons (Interface) but don't know how the internal circuit (Abstraction) changes the channel.
    ```java
    interface Remote { void changeChannel(); }
    ```

---

### Q2. JVM Architecture & Platform Independence
**Introduction:**
The **Java Virtual Machine (JVM)** is an abstract machine that provides a runtime environment for Java bytecode execution. It is platform-dependent (different for Windows, Linux, Mac), but it enables Java programs to be platform-independent.

**JVM Architecture Components:**
1.  **Class Loader Subsystem:**
    *   **Loading:** Reads `.class` files into memory.
    *   **Linking:** Verifies bytecode for security, prepares static variables, and resolves symbolic references.
    *   **Initialization:** Executes static blocks and assigns values to static variables.
2.  **Runtime Data Areas (Memory Management):**
    *   **Method Area:** Stores class structures, static variables, and constant pools.
    *   **Heap Area:** The largest area, where all objects and their instance variables are stored. (Managed by Garbage Collector).
    *   **Stack Area:** Created for every thread. Stores local variables and partial results during method execution.
    *   **PC Registers:** Stores the address of the current instruction being executed.
    *   **Native Method Stack:** Stores information for native methods (written in C/C++).
3.  **Execution Engine:**
    *   **Interpreter:** Reads bytecode and executes it line-by-line. (Slow).
    *   **JIT (Just-In-Time) Compiler:** Identifies "hot spots" (frequently used code) and compiles them into native machine code to speed up execution.
    *   **Garbage Collector (GC):** Automatically tracks objects and deletes those that are no longer reachable by the program.

**Platform Independence:**
Java's slogan is **"Write Once, Run Anywhere (WORA)"**. When we compile a `.java` file, the compiler (`javac`) generates **Bytecode** (`.class` file). This bytecode is a neutral language. Any OS with a JVM installed can read this same bytecode and translate it into that OS's specific machine language. Thus, the programmer writes code once, and it runs on all systems.

---

### Q3. Inheritance & Types & The Diamond Problem
**Definition:**
Inheritance is a mechanism that allows a new class to inherit attributes and methods from an existing class. It models the **"IS-A" relationship** (e.g., a Dog *is an* Animal).

**Types of Inheritance Supported in Java:**
1.  **Single Inheritance:** One subclass inherits from one superclass.
2.  **Multilevel Inheritance:** A subclass inherits from a class, which itself is a subclass of another class (A -> B -> C).
3.  **Hierarchical Inheritance:** Multiple subclasses inherit from a single superclass (A -> B, A -> C).

**The Diamond Problem (Why Multiple Inheritance is not supported for Classes):**
Consider a scenario where Class B and Class C both inherit from Class A and override a method `display()`. If Class D inherits from both B and C, and we call `D.display()`, the compiler will not know whether to call the version from B or C. This ambiguity is called the **Diamond Problem**.
*   **Java's Solution:** Multiple inheritance is prohibited for classes to keep the language simple and robust. However, it is fully supported through **Interfaces**, because a class can implement multiple interfaces and must provide its own single implementation of the methods, removing ambiguity.

---

### Q4. Java Packages: Definition, Creation, and Usage
**Definition:**
A **Package** is a container that groups related classes, interfaces, and sub-packages. It is used to avoid naming conflicts (e.g., two classes named `Date` in different packages) and to provide access protection.

**Steps to Create and Use a User-Defined Package:**
1.  **Define the Package:** Use the `package` keyword as the very first line in your Java source file.
2.  **Create Classes:** Add classes inside that file.
3.  **Directory Structure:** The file must be saved in a folder name that matches the package name.
4.  **Compilation:** Use the command `javac -d . FileName.java`. The `-d` flag tells the compiler where to put the class file (creating the folder automatically).
5.  **Import:** In another class, use the `import` keyword to access the package members.

**Code Snippet:**
*File 1: saved as `C:\mypack\Greeting.java`*
```java
package mypack; // 1. Defining package
public class Greeting {
    public void msg() { System.out.println("Hello Topper!"); }
}
```
*File 2: saved in a different folder*
```java
import mypack.Greeting; // 2. Importing package
class Test {
    public static void main(String args[]) {
        Greeting obj = new Greeting();
        obj.msg();
    }
}
```

---

### Q5. Thread Life Cycle (Thread States)
**Introduction:**
A thread in Java is a lightweight subprocess. The life cycle of a thread is controlled by the **JVM Thread Scheduler**. A thread can be in one of five distinct states.

**1. New (Born):**
When a thread object is created (using the `new` operator), but the `start()` method has not been called yet.
**2. Runnable:**
After calling `start()`, the thread is ready to run and waiting for CPU time. It is in the "ready pool".
**3. Running:**
The thread is currently being executed by the processor. The `run()` method is active.
**4. Blocked / Waiting (Non-Runnable):**
The thread is alive but not eligible to run. It moves to this state if:
*   It is waiting for I/O.
*   It is sleeping (via `Thread.sleep()`).
*   It is waiting for another thread to finish (via `join()`).
Once the waiting condition is over, it moves back to the **Runnable** state.
**5. Terminated (Dead):**
The thread enters this state when its `run()` method completes execution or if it is stopped due to an error.

**Creating Threads:**
1.  **Extending `Thread` Class:**
    ```java
    class MyThread extends Thread { public void run() { /* code */ } }
    MyThread t = new MyThread(); t.start();
    ```
2.  **Implementing `Runnable` Interface (Preferred):**
    Allows the class to inherit from another class as well.
    ```java
    class MyJob implements Runnable { public void run() { /* code */ } }
    Thread t = new Thread(new MyJob()); t.start();
    ```

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
