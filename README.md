# 📚 Core Java Practicals & Assignments

A comprehensive repository containing all the practical assignments and code examples from my core Java training program. This project serves as a log of my learning journey, covering fundamental to advanced topics in Java.

-----

## 📝 Overview

This project is a collection of standalone Java programs, each designed to demonstrate a specific concept. The code is organized into packages, reflecting the topics covered during the coursework. The primary goal is to provide a clear, executable example for each fundamental principle of the Java language.

-----

## ✨ Key Concepts Covered

This repository includes practical implementations of the following topics:

| Category | Concepts Covered |
| :--- | :--- |
| **Object-Oriented Programming** | Classes, Objects, Inheritance, Polymorphism, Abstraction |
| **Core Fundamentals** | Data Types, Variables, Operators, Control Structures |
| **Data Structures** | Arrays, Strings, Collections Framework (List, Set, Map) |
| **Advanced Topics** | Exception Handling, Multithreading, Synchronization |
| **Database & Files** | Java Database Connectivity (JDBC), File I/O Streams |

-----

## 🚀 Getting Started

To run this project, you will need to set up your local environment by following these steps.

### **Prerequisites**

  * **Java Development Kit (JDK):** Version 8 or higher.
  * **IDE:** An IDE such as Eclipse or IntelliJ IDEA.
  * **Database:** A running instance of MySQL Server.

### **1. Clone the Repository**

Open your terminal or command prompt and run the following command:

```bash
git clone [your-repository-url]
```

*Replace `[your-repository-url]` with the actual URL of your GitHub repository.*

### **2. Import into Your IDE**

1.  Open your IDE (e.g., Eclipse).
2.  Select `File > Import...`.
3.  Choose "Existing Projects into Workspace" under the `General` category.
4.  Select the root directory of the cloned repository and click `Finish`.

### **3. Database Setup (for JDBC Practicals)**

The parts of this project that use JDBC require a MySQL database.

Run the following SQL script in your preferred MySQL client (like MySQL Workbench) to create the necessary database and a sample table.

```sql
-- 1. Create a new database for the project
CREATE DATABASE IF NOT EXISTS tns_practicals;

-- 2. Switch to using the new database
USE tns_practicals;

-- 3. Create a sample 'students' table for practice
CREATE TABLE IF NOT EXISTS students (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    student_name VARCHAR(255) NOT NULL,
    email VARCHAR(255) UNIQUE,
    enrollment_date DATE
);
```

**Important:** This project requires the **MySQL Connector/J** to communicate with the database. You must add the `mysql-connector-j-....jar` file to the project's **Build Path** in your IDE.

-----

## 📂 Project Structure

The code is organized into packages based on the topics taught. The package structure follows the standard Java convention for easy navigation:

`com.tnsif.day[number].[topic]`

This structure helps in easily locating the code corresponding to a specific concept.

-----

## 💡 Project Context

**Please Note:** This repository contains the project codebase as provided by my instructor. It has been uploaded to GitHub to demonstrate proficiency with version control using Git. As this is instructional material, it may include IDE-specific configuration files (`.classpath`, `.project`) and pre-compiled class files (`.class`) as they were part of the original distribution.
