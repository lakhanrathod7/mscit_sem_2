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

### Q1. Open Source Software (OSS) - Definition & Analysis
**Definition:**
Open Source Software (OSS) is software with its source code made available with a license in which the copyright holder provides the rights to study, change, and distribute the software to anyone and for any purpose.

**Advantages of OSS:**
1.  **Transparency & Trust:** Since the code is open, anyone can verify that the software does what it claims and doesn't contain hidden malware.
2.  **Rapid Innovation:** A global community of developers can contribute features and fix bugs much faster than a single company.
3.  **Cost Savings:** Most OSS is free of licensing fees, which significantly reduces the Total Cost of Ownership (TCO).
4.  **Security:** "Linus's Law" states that "given enough eyeballs, all bugs are shallow." High visibility leads to faster security patching.
5.  **No Vendor Lock-in:** Organizations are not dependent on a single vendor's roadmap or pricing structure.

**Disadvantages of OSS:**
1.  **Support Challenges:** No centralized technical support. Businesses must rely on community forums or hire third-party experts.
2.  **Ease of Use:** Many open-source tools are developed by techies for techies and may lack the polished user interface of commercial products.
3.  **Hidden Costs:** Training staff to use new OSS and the cost of integration can sometimes exceed the savings on licenses.
4.  **Compliance Risks:** Organizations must be careful to follow the specific terms of OSS licenses (like GPL or MIT) to avoid legal issues.

---

### Q4. Database Operations in PHP (CRUD)
To perform database operations in PHP, we typically use the `mysqli` extension or `PDO`. Below is the technical breakdown using `mysqli`.

**1. Database Connectivity:**
```php
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "myDB";

// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);

// Check connection
if ($conn->connect_error) {
  die("Connection failed: " . $conn->connect_error);
}
```

**2. INSERT Operation:**
Used to add new records to a table.
```php
$sql = "INSERT INTO Students (firstname, lastname) VALUES ('John', 'Doe')";
if ($conn->query($sql) === TRUE) { echo "New record created"; }
```

**3. SELECT Operation:**
Used to retrieve data.
```php
$sql = "SELECT id, firstname FROM Students";
$result = $conn->query($sql);
if ($result->num_rows > 0) {
  while($row = $result->fetch_assoc()) {
    echo "id: " . $row["id"]. " - Name: " . $row["firstname"]. "<br>";
  }
}
```

**4. UPDATE & DELETE:**
```php
// Update
$sql = "UPDATE Students SET lastname='Smith' WHERE id=1";
// Delete
$sql = "DELETE FROM Students WHERE id=1";
```

---

### Q5. HTTP GET vs POST Comparison
| Feature | GET Method | POST Method |
| :--- | :--- | :--- |
| **Data Location** | Appended to the URL in query strings. | Sent in the HTTP request body. |
| **Visibility** | Data is visible to everyone in the URL. | Data is not visible in the URL. |
| **Data Size** | Limited (~2048 characters). | No fixed limit (large files allowed). |
| **Security** | Low (Never use for passwords). | Higher (Mandatory for sensitive data). |
| **Caching** | Can be cached and bookmarked. | Cannot be cached or bookmarked. |
| **History** | Stored in browser history. | Not stored in browser history. |

**When to use:** Use **GET** for idempotent actions like searching or filtering where state doesn't change. Use **POST** for actions that modify data, such as submitting a form or uploading a file.

---

## SECTION B: SHORT ANSWERS (5 MARKS EACH)

### Q4. Referential Integrity & Primary Key
1.  **Primary Key:** A column or group of columns that uniquely identifies each row in a table. It cannot contain NULL values and must be unique across all rows.
2.  **Referential Integrity:** A set of rules that ensures that the relationship between tables remains consistent. It ensures that a Foreign Key in one table must always point to a valid Primary Key in another table, preventing "orphan" records.

### Q6. Role of Apache in LAMP
Apache is the **Web Server** component of the LAMP stack.
*   **Request Handling:** It listens for incoming HTTP requests from browsers.
*   **Processing:** It passes PHP requests to the PHP interpreter.
*   **Delivery:** It sends the processed HTML output back to the client's browser.
*   **Security:** It manages access control via `.htaccess` files and SSL/TLS for encryption.

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
9.  **False** (Data is hidden in body)
10. **True**
