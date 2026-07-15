00# MSCIT-202: Web Application Development – LAMP
## 10-Mark Questions (Important for Exam)

1.  **⭐⭐⭐ Open Source Software:** Define Open Source Software (OSS). Discuss the advantages and disadvantages (pros and cons) of OSS. (Repeated: Aug 2022, Jan 2023, July 2025)
2.  **⭐⭐⭐ Linux File Permissions:** Discuss file permissions in a Linux system. Explain how to manage permissions with commands like `chmod`, `chown`, and `chgrp`. (Repeated: Aug 2022, July 2023, July 2025)
3.  **⭐⭐⭐ MySQL Datatypes:** List and explain different datatypes available in MySQL in detail. (Repeated: Aug 2022, Jan 2023, July 2025)
4.  **⭐⭐⭐ SQL Sub-languages:** Briefly explain sub-languages of SQL (DDL, DML, DCL, TCL) with examples of each. (Repeated: Aug 2022, Jan 2023, July 2025)
5.  **⭐⭐⭐ PHP-MySQL Operations:** Explain database manipulation operations (Insert, Select, Update, Delete) in PHP with suitable examples. (Repeated: Aug 2022, Jan 2023)
6.  **⭐⭐⭐ HTTP Methods (GET vs POST):** Give a detailed comparison of HTTP methods GET and POST. Discuss when to use each. (Repeated: Aug 2022, July 2023, July 2025)
7.  **⭐⭐⭐ PHP File Handling & Inclusion:** Explain how to perform file handling in PHP. Discuss functions used to include one PHP file into another (`include`, `require`). (Repeated: Jan 2023, July 2023, July 2025)
8.  **⭐⭐⭐ User-Defined Functions:** Describe in brief about User-defined Functions (UDF) in PHP. What are the rules for creating a UDF? (Repeated: Jan 2023, July 2023, July 2025)
9.  **⭐⭐⭐ PHP Cookies & Sessions:** Describe the steps to store and manage form data using Cookies and Sessions in PHP. (Repeated: July 2023, July 2025)
10. **⭐⭐ Data Validation in PHP:** Write a detailed note on data validation and sanitization in PHP. (Repeated: Jan 2023)
11. **⭐⭐ Exception Handling in PHP:** Write a short note on Exception handling in PHP with an example. (Repeated: July 2023)
12. **⭐⭐ String Handling Functions:** List and explain common string handling functions in PHP (e.g., `strlen`, `strpos`, `trim`). (Repeated: July 2025)
13. **⭐⭐ Linux Administration Tools:** List and explain system administrative tools for Linux. (Repeated: Aug 2022, July 2025)
14. **⭐⭐ PHP Arrays:** Explain how to declare, use, and store data in arrays in PHP (Indexed vs Associative). (Repeated: Jan 2023, July 2023)
15. **⭐⭐ SQL Transaction Control (TCL):** What is the need for Transaction Control Language? Explain `COMMIT` and `ROLLBACK` in brief. (Repeated: July 2023)

---

## Detailed Answers (10-Mark Questions)

### 1. Open Source Software (OSS)
*   **Definition:** Open Source Software is software whose source code is released under a license in which the copyright holder grants users the rights to study, change, and distribute the software to anyone and for any purpose. It is often developed in a public, collaborative manner.
*   **Advantages (Pros):**
    1.  **Cost-Effective:** Most OSS is free to download and use, eliminating high licensing fees associated with proprietary software like Windows or Oracle.
    2.  **Reliability & Security:** Since the source code is public, it is peer-reviewed by thousands of developers globally. Bugs are identified and patched much faster than in closed systems ("Linus's Law").
    3.  **Flexibility & Customization:** Organizations can modify the code to fit their specific requirements without waiting for a vendor to release a new feature.
    4.  **No Vendor Lock-in:** Users are not dependent on a single company for updates or support. If one provider fails, others can take over.
    5.  **Community Support:** Extensive documentation and forums are available for popular OSS projects (e.g., Stack Overflow, GitHub).
*   **Disadvantages (Cons):**
    1.  **Learning Curve:** Some OSS (like Linux command line) can be more difficult for non-technical users to master compared to GUI-heavy proprietary software.
    2.  **Lack of Formal Support:** There is often no "help desk" to call. Support relies on the community, though many companies (like Red Hat) now sell professional support for OSS.
    3.  **Hidden Costs:** While the software is free, costs for implementation, training, and maintenance can still be high.
    4.  **Compatibility Issues:** Some specialized proprietary hardware or software may not have drivers or versions available for open-source platforms.

### 2. Linux File Permissions
*   **Overview:** Linux is a secure multi-user system. Access to files and directories is controlled by three sets of permissions: **Owner (User)**, **Group**, and **Others**.
*   **Permission Types:**
    *   **r (Read):** Permission to view file content or list directory contents. (Value: 4)
    *   **w (Write):** Permission to modify file content or create/delete files in a directory. (Value: 2)
    *   **x (Execute):** Permission to run a file as a program or enter a directory. (Value: 1)
*   **Representations:**
    *   **Symbolic:** `-rwxr-xr--` (Owner has rwx, Group has r-x, Others have r--).
    *   **Numeric (Octal):** `754` (7 for owner, 5 for group, 4 for others).
*   **Management Commands:**
    1.  **chmod (Change Mode):** Modifies permissions.
        *   Example: `chmod 777 file.txt` (Full access for everyone).
        *   Example: `chmod u+x script.sh` (Add execute permission for the owner).
    2.  **chown (Change Owner):** Changes the user who owns the file.
        *   Example: `chown admin report.pdf`.
    3.  **chgrp (Change Group):** Changes the group associated with the file.
        *   Example: `chgrp developers source_code.php`.
*   **Importance:** Proper permission management prevents unauthorized access to sensitive system files and user data.

### 3. MySQL Datatypes in Detail
*   **Introduction:** Choosing the correct datatype is crucial for database performance, data integrity, and minimizing storage space.
*   **1. Numeric Types:**
    *   `TINYINT`: 1 byte. Range -128 to 127.
    *   `INT`: 4 bytes. Standard for IDs and whole numbers.
    *   `BIGINT`: 8 bytes. For very large numbers.
    *   `DECIMAL(P, D)`: Exact fixed-point number. Ideal for financial data (e.g., `DECIMAL(10,2)`).
*   **2. String (Text) Types:**
    *   `CHAR(size)`: Fixed-length string (padded with spaces). Faster for short, fixed-size data like country codes ('IN', 'US').
    *   `VARCHAR(size)`: Variable-length string. More efficient for names, addresses, etc.
    *   `TEXT`: For long descriptions or articles (up to 64 KB).
*   **3. Date and Time Types:**
    *   `DATE`: `YYYY-MM-DD`.
    *   `DATETIME`: `YYYY-MM-DD HH:MM:SS`.
    *   `TIMESTAMP`: Stores seconds since Unix epoch. Useful for "Last Updated" fields.
*   **4. Binary Types:**
    *   `BLOB` (Binary Large Object): Used for storing images, PDFs, or encrypted data.
*   **Selection Criteria:** Always use the smallest type that can reliably hold your data to optimize memory and disk I/O.

### 4. SQL Sub-languages (DDL, DML, DCL, TCL)
*   **1. DDL (Data Definition Language):** Used to define or modify the database schema (structure).
    *   *Commands:* `CREATE` (make new table/db), `ALTER` (modify structure), `DROP` (delete table/db), `TRUNCATE` (delete all data but keep structure).
    *   *Example:* `CREATE TABLE Students (ID INT, Name VARCHAR(50));`
*   **2. DML (Data Manipulation Language):** Used to manage data within the objects.
    *   *Commands:* `INSERT` (add rows), `UPDATE` (modify existing rows), `DELETE` (remove rows), `SELECT` (retrieve data).
    *   *Example:* `UPDATE Students SET Name='Amit' WHERE ID=1;`
*   **3. DCL (Data Control Language):** Used to control access to data.
    *   *Commands:* `GRANT` (give access), `REVOKE` (take back access).
    *   *Example:* `GRANT SELECT ON Students TO 'guest_user';`
*   **4. TCL (Transaction Control Language):** Used to manage database transactions.
    *   *Commands:* `COMMIT` (save changes), `ROLLBACK` (undo changes), `SAVEPOINT`.
    *   *Example:* `COMMIT;` (Makes the current session's changes permanent).

### 5. PHP-MySQL Operations (CRUD)
*   **Introduction:** CRUD stands for Create, Read, Update, and Delete. These are the four basic functions of persistent storage.
*   **1. Create (INSERT):**
    ```php
    $sql = "INSERT INTO users (name, email) VALUES ('John', 'john@example.com')";
    if (mysqli_query($conn, $sql)) { echo "New record created"; }
    ```
*   **2. Read (SELECT):**
    ```php
    $sql = "SELECT id, name FROM users";
    $result = mysqli_query($conn, $sql);
    while($row = mysqli_fetch_assoc($result)) {
        echo "id: " . $row["id"]. " - Name: " . $row["name"]. "<br>";
    }
    ```
*   **3. Update (UPDATE):**
    ```php
    $sql = "UPDATE users SET email='new@example.com' WHERE id=1";
    mysqli_query($conn, $sql);
    ```
*   **4. Delete (DELETE):**
    ```php
    $sql = "DELETE FROM users WHERE id=1";
    mysqli_query($conn, $sql);
    ```
*   **Note:** In real applications, always use **Prepared Statements** to prevent SQL Injection attacks.

### 6. HTTP Methods: GET vs POST
*   **Introduction:** HTTP methods define the action to be performed on a resource. GET and POST are the most common.
*   **Detailed Comparison:**
    | Feature | GET | POST |
    | :--- | :--- | :--- |
    | **Data Location** | Appended to URL (Query String) | Inside the Request Body |
    | **Visibility** | Visible in Address Bar | Hidden from user |
    | **Security** | Low (not for passwords) | High (preferred for sensitive data) |
    | **Data Size** | Limited (~2000 chars) | No fixed limit (supports large files) |
    | **Caching** | Can be cached & bookmarked | Cannot be cached |
    | **History** | Stored in Browser History | Not stored in History |
*   **When to use GET:** For idempotent requests (actions that don't change state), like searching, sorting, or filtering data.
*   **When to use POST:** For non-idempotent requests, like creating a new user account, submitting a payment, or uploading a file.

### 7. PHP File Handling & Inclusion
*   **1. File Handling:** PHP treats files as resources.
    *   `fopen($file, $mode)`: Opens a file. Modes: 'r' (Read), 'w' (Write - overwrites), 'a' (Append).
    *   `fread()` / `fwrite()`: Reading/Writing content.
    *   `fgets()`: Reads a single line.
    *   `fclose()`: Closes the file handle to free resources.
*   **2. File Inclusion:** Allows a modular approach to web development.
    *   `include 'header.php';`: Includes the file. If it fails, the script continues with a warning.
    *   `require 'config.php';`: Includes the file. If it fails, the script stops with a fatal error. Use this for critical files like database connections.
    *   `include_once` / `require_once`: Prevents multiple inclusions of the same file, which could cause "function redefined" errors.
*   **Benefits:** Easier maintenance (update one header file instead of 100 pages) and cleaner code organization.

### 8. User-Defined Functions (UDF) in PHP
*   **Definition:** A UDF is a block of code created by the developer to perform a specific task.
*   **Rules for creation:**
    1.  Must start with the keyword `function`.
    2.  The name must be unique and follow variable naming rules (start with letter/underscore).
    3.  Functions are not case-sensitive but should be consistent.
    4.  Can accept **Parameters** (inputs) and **Return** values (outputs).
*   **Advanced Features:**
    *   **Default Arguments:** `function greet($name = "Guest") { ... }`
    *   **Variable Scope:** Variables defined inside a function are local to it unless declared `global`.
    *   **Pass by Reference:** Using `&` (e.g., `function addFive(&$num)`) allows a function to modify the original variable.
*   **Benefit:** UDFs promote the DRY (Don't Repeat Yourself) principle, making debugging and updates much simpler.

### 9. PHP Cookies & Sessions
*   **Introduction:** Since HTTP is stateless, Cookies and Sessions are used to track user data across multiple pages.
*   **1. Cookies:**
    *   *Storage:* On the client's (user's) computer.
    *   *Creation:* `setcookie("user", "Amit", time() + 3600);` (Expires in 1 hour).
    *   *Retrieval:* `$_COOKIE['user']`.
    *   *Usage:* "Remember Me" features, user preferences, tracking.
*   **2. Sessions:**
    *   *Storage:* On the server (more secure). A session ID is stored in a cookie on the client.
    *   *Creation:* `session_start(); $_SESSION['id'] = 123;`.
    *   *Retrieval:* `$_SESSION['id']`.
    *   *Destruction:* `session_destroy();`.
    *   *Usage:* Login systems, shopping carts.
*   **Security:** Sessions are preferred for sensitive data because the user cannot view or modify the data stored on the server.

### 10. Data Validation & Sanitization in PHP
*   **1. Validation:** Checking if input meets requirements.
    *   *Empty check:* `if (empty($_POST['name'])) { ... }`
    *   *Type check:* `if (!is_numeric($age)) { ... }`
    *   *Format check:* `filter_var($email, FILTER_VALIDATE_EMAIL)` or Regular Expressions (`preg_match`).
*   **2. Sanitization:** Cleaning input to prevent attacks.
    *   **Cross-Site Scripting (XSS):** Use `htmlspecialchars($input)` to convert characters like `<` and `>` into HTML entities, preventing them from being executed as scripts in the browser.
    *   **SQL Injection:** Use `mysqli_real_escape_string($conn, $input)` or, ideally, **PDO with Prepared Statements**.
    *   **Whitespace:** Use `trim()` to remove accidental spaces.
*   **Rule:** "Never trust user input." Always validate on the server side even if client-side validation (JavaScript) is present.

### 11. Exception Handling in PHP
*   **Definition:** A mechanism to handle runtime errors gracefully, preventing the application from crashing and showing "ugly" errors to users.
*   **Components:**
    1.  **try:** The code block where an error might occur.
    2.  **throw:** Manually triggers an exception object if a condition is met.
    3.  **catch:** Captures the exception and handles it (e.g., logging or showing a friendly message).
    4.  **finally:** Code that always runs (e.g., closing a database connection).
*   **Example:**
    ```php
    try {
        if ($divisor == 0) { throw new Exception("Division by zero!"); }
        $result = 100 / $divisor;
    } catch (Exception $e) {
        echo "Error: " . $e->getMessage();
    } finally {
        echo "Operation attempted.";
    }
    ```
*   **Benefits:** Separation of error-handling code from normal logic, better debugging with stack traces, and improved security.

### 12. PHP String Handling Functions
*   **Overview:** Text processing is a core part of web development.
*   **Key Functions:**
    1.  **strlen($s):** Returns the length of the string.
    2.  **strpos($s, $find):** Returns the index of the first occurrence of a substring.
    3.  **substr($s, $start, $len):** Extracts a portion of a string.
    4.  **str_replace($old, $new, $s):** Replaces occurrences of a word/character.
    5.  **trim($s):** Removes whitespace from both ends.
    6.  **strtolower() / strtoupper():** Case conversion.
    7.  **md5() / password_hash():** Used for hashing strings (passwords).
*   **Explode and Implode:**
    *   `explode(" ", "Hello World")` -> `["Hello", "World"]` (String to Array).
    *   `implode("-", ["A", "B"])` -> `"A-B"` (Array to String).

### 13. Linux Administration Tools in Detail
*   **Webmin:**
    *   Provides a GUI for Linux admin tasks like user management, setup of Apache/MySQL, and monitoring disk space.
    *   Eliminates the need for a command-line interface for many common tasks.
*   **Cockpit:**
    *   A lightweight, browser-based dashboard for real-time performance monitoring.
    *   Excellent for managing storage, networking, and system logs across multiple servers.
*   **Shorewall:**
    *   A high-level firewall configuration tool based on Netfilter.
    *   Uses simple configuration files to manage zones and complex routing rules.
*   **Zenmap:**
    *   The official Nmap GUI. It provides advanced network mapping, port scanning, and OS detection features.
*   **Conclusion:** These tools significantly reduce human error and improve the efficiency of server maintenance.

### 14. PHP Arrays: Indexed vs Associative
*   **Indexed Arrays:**
    *   Uses numeric keys automatically assigned starting from 0.
    *   *Syntax:* `$fruits = ["Apple", "Banana"];`
    *   *Access:* `$fruits[0]` is "Apple".
*   **Associative Arrays:**
    *   Uses custom named keys (strings).
    *   *Syntax:* `$prices = ["Apple" => 100, "Banana" => 20];`
    *   *Access:* `$prices["Apple"]` is 100.
*   **Multidimensional Arrays:**
    *   Arrays containing other arrays (e.g., a table with rows and columns).
*   **Iteration:** Use `foreach` for easy access:
    ```php
    foreach ($prices as $item => $val) {
        echo "$item costs $val";
    }
    ```

### 15. SQL Transaction Control (TCL)
*   **What is a Transaction?** A transaction is a single logical unit of work that contains one or more SQL statements (usually DML like INSERT/UPDATE).
*   **ACID Properties:**
    1.  **Atomicity:** All statements in the transaction must succeed, or none are applied ("All or nothing").
    2.  **Consistency:** The database remains in a valid state after the transaction.
    3.  **Isolation:** Transactions do not interfere with each other.
    4.  **Durability:** Once committed, changes are permanent even after a crash.
*   **Key Commands:**
    1.  **START TRANSACTION / BEGIN:** Marks the beginning of the unit.
    2.  **COMMIT:** Saves all changes permanently.
    3.  **ROLLBACK:** Undoes all changes since the last COMMIT or BEGIN.
    4.  **SAVEPOINT:** Creates a bookmark within a transaction to allow partial rollbacks.
*   **Importance:** Essential for applications where data accuracy is critical, such as banking (moving money from one account to another).
