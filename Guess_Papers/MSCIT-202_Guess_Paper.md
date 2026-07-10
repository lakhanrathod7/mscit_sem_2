# BAOU M.Sc. IT Semester 2 - Guess Paper (August 2026)
## MSCIT-202: Web Application Development – LAMP

**Time: 3 Hours | Max Marks: 70**

---

### Section A: Long Answer Questions (Attempt any 3 - 30 Marks)
1. Define Open Source Software (OSS). Discuss the advantages and disadvantages of OSS compared to proprietary software.
2. Explain the Linux file system hierarchy (FHS) and discuss how to manage file permissions using `chmod`.
3. List and explain different datatypes available in MySQL. Discuss DDL and DML sub-languages with examples.
4. Explain database manipulation operations (Insert, Select, Update, Delete) in PHP with suitable database connectivity code.
5. Give a detailed comparison of HTTP methods GET and POST. Discuss when to use each with examples.

---

### Section B: Short Answer Questions (Attempt any 4 - 20 Marks)
1. Differentiate between Open-source and Closed-source software.
2. Explain the syntax of the `foreach` loop in PHP with an example.
3. What is an associative array? Explain how to store and access data in it using PHP.
4. Define: (1) Referential Integrity (2) Primary Key.
5. Write a short note on state management using Sessions and Cookies in PHP.
6. Explain the role of the Apache web server in the LAMP stack.

---

### Section C: Part A - MCQs (10 Marks)
1. Which command is used to change file permissions in Linux?
   A. chown B. chmod C. chgrp D. change
2. Which symbol is used to declare a variable in PHP?
   A. % B. @ C. $ D. &
3. Which function is used to remove spaces from a string?
   A. trim() B. cut() C. remove() D. del()
4. What does the 'A' in LAMP stand for?
   A. Android B. Apple C. Apache D. Amazon
5. Which SQL statement is used to retrieve data?
   A. INSERT B. SELECT C. UPDATE D. DELETE
6. Which PHP function is used to start a session?
   A. session_start() B. start_session() C. begin_session() D. session_init()
7. Default port for MySQL is:
   A. 80 B. 443 C. 3306 D. 21
8. Which operator is used for string concatenation in PHP?
   A. + B. . C. & D. *
9. `chmod 777` gives what permissions to everyone?
   A. Read only B. Write only C. Full permissions D. No permissions
10. Which command shows the current working directory in Linux?
    A. cd B. ls C. pwd D. dir

---

### Section C: Part B - True or False (10 Marks)
1. PHP stands for Hypertext Preprocessor.
2. Linux is a closed-source operating system.
3. `die()` function combines `echo` and `exit`.
4. Create Table is a DML statement.
5. Variables in PHP are case-sensitive.
6. The `explode()` function splits a string into an array.
7. `#` is used for multi-line comments in PHP.
8. MySQL is an RDBMS.
9. `$_POST` data is visible in the URL.
10. In LAMP, 'L' stands for Linux.

---
---

# TOPPER'S SOLUTIONS (DETAILED EXAM FORMAT)

## SECTION A: LONG ANSWERS (10 MARKS EACH)

### Q1. Open Source Software (OSS)
**Definition:**
Open Source Software is software whose source code is released under a license that allows users to study, change, and distribute the software to anyone and for any purpose. It is developed in a collaborative, decentralized manner.

**Advantages of OSS:**
1.  **Transparency:** Anyone can inspect the code for bugs or security holes.
2.  **Cost-Effectiveness:** Most OSS is free to use, eliminating licensing fees like those for Windows or Oracle.
3.  **Reliability:** Peer-review by a global community ensures that bugs are found and patched quickly.
4.  **No Vendor Lock-in:** Users are not tied to a single company for support or updates.
5.  **Flexibility:** Developers can customize the software to meet specific business needs.

**Disadvantages of OSS:**
1.  **Learning Curve:** Some tools (like Linux command line) require more technical knowledge than proprietary alternatives.
2.  **Lack of Formal Support:** There is no dedicated "help desk" for free software; support comes from community forums.
3.  **Security Risks:** While peer-review helps, the fact that code is public also means hackers can study it for vulnerabilities.
4.  **Compatibility:** Some proprietary hardware or file formats might not work perfectly with OSS.

---

### Q2. Linux File System & Permissions
**Linux File System Hierarchy (FHS):**
Linux follows a tree-like structure starting from the root directory (`/`).
*   `/bin`: Essential command binaries (like `ls`, `cp`).
*   `/etc`: System configuration files.
*   `/home`: Personal directories for users.
*   `/root`: Home directory for the System Administrator.
*   `/var`: Variable data files (logs, databases).
*   `/tmp`: Temporary files.

**Managing Permissions with `chmod`:**
Linux assigns three types of permissions to three categories of users.
*   **Permissions:** `r` (Read=4), `w` (Write=2), `x` (Execute=1).
*   **Categories:** `u` (User/Owner), `g` (Group), `o` (Others).

**Using Numeric Method:**
Total value = Sum of permissions. (e.g., Read + Write = 4+2 = 6).
*   `chmod 755 file`:
    *   **7** (4+2+1): Owner has full access.
    *   **5** (4+0+1): Group has Read and Execute.
    *   **5** (4+0+1): Others have Read and Execute.

---

### Q3. MySQL Datatypes and Sub-languages
**Common MySQL Datatypes:**
1.  **Numeric:** `INT` (integers), `DECIMAL(P, D)` (precise fixed-point for money).
2.  **String:** `CHAR` (fixed length), `VARCHAR` (variable length), `TEXT` (large text blocks).
3.  **Date/Time:** `DATE` (YYYY-MM-DD), `DATETIME` (YYYY-MM-DD HH:MM:SS).

**SQL Sub-languages:**
*   **1. DDL (Data Definition Language):** Used to define the structure of the database.
    *   *Commands:* `CREATE`, `ALTER`, `DROP`.
    *   *Example:* `CREATE TABLE Users (id INT, name VARCHAR(50));`
*   **2. DML (Data Manipulation Language):** Used to manage data within the tables.
    *   *Commands:* `INSERT`, `UPDATE`, `DELETE`, `SELECT`.
    *   *Example:* `UPDATE Users SET name='Amit' WHERE id=1;`

---

## SECTION B: SHORT ANSWERS (5 MARKS EACH)

### Q2. `foreach` loop in PHP
The `foreach` loop is specifically designed to iterate through array elements.
**Syntax:**
```php
foreach ($array as $value) {
    // code to be executed
}
```
**Example:**
```php
$names = ["John", "Sneha", "Rahul"];
foreach ($names as $n) {
    echo "Name is: $n <br>";
}
```

### Q3. Associative Arrays
An associative array uses **named keys** that you assign to them, instead of numeric indexes.
**Example:**
```php
$salary = ["Amit" => 50000, "Sita" => 60000];
echo "Amit's salary is: " . $salary['Amit'];
```
These are highly useful for representing database records where keys match column names.

### Q5. Sessions vs Cookies
*   **Cookies:** Stored on the **Client's browser**. Used for tracking and non-sensitive data like theme preferences. They have an expiration date.
*   **Sessions:** Stored on the **Server**. Much more secure. Used for sensitive data like login IDs. A session ID is stored in a cookie on the client to link the user to the server data.

---

## SECTION C: OBJECTIVE ANSWERS

### Part A: MCQs
1.  **B.** chmod
2.  **C.** $
3.  **A.** trim()
4.  **C.** Apache
5.  **B.** SELECT
6.  **A.** session_start()
7.  **C.** 3306
8.  **B.** . (Dot)
9.  **C.** Full permissions
10. **C.** pwd

### Part B: True or False
1.  **True**
2.  **False** (Open Source)
3.  **True**
4.  **False** (It is DDL)
5.  **True**
6.  **True**
7.  **False** (`/* */` is for multi-line)
8.  **True**
9.  **False** (POST data is hidden)
10. **True**
