# Library Management System

### Student Details
- **Name:** Tapabrata Bakuli
- **Enrollment Number:** 12024052017060
- **Department:** CSE(IOTCSBT)
- **Year/Semester:** 2nd Year / 4th Sem
- **Institute:** Institute of Engineering and Management (IEM)

---

## 1. Problem Statement
The manual management of library resources is prone to errors, inefficient tracking, and data redundancy. This project implements an automated **Library Management System** in Java to streamline the process of cataloging books, managing users (Students and Librarians), and tracking borrowing transactions. It ensures data integrity and provides an interactive interface for real-time library operations.

## 2. Target User
- **Librarians:** For administrative control, adding books, and monitoring overall history.
- **Students:** For searching, borrowing, and returning books within specified limits.

## 3. Core Features
- **Dynamic Inventory:** Add and search books by title or ISBN.
- **User Management:** Categorized users (Student/Librarian) with distinct permissions.
- **Borrowing Logic:** Automated issue/return system with validation checks.
- **Transaction History:** Persistent logs of all library activities with timestamps.
- **Input Validation:** Robust menu-driven interface with error handling for user inputs.

## 4. OOP Concepts Used
- **Encapsulation:** Used private fields in `Book` and `User` with public getters/setters to protect data integrity.
- **Inheritance:** `Student` and `Librarian` classes inherit common attributes from the abstract `User` class.
- **Polymorphism:** Overridden the `getMaxBorrowLimit()` method to provide different borrowing rules for different user types.
- **Abstraction:** The `User` class is abstract, ensuring no generic user can be created without a specific type.
- **Composition:** The `Library` class manages collections of `Book`, `User`, and `Transaction` objects.

## 5. Architecture Description
The system follows a modular architecture:
- **Models:** `Book`, `User`, `Student`, `Librarian`, and `Transaction` represent the data layer.
- **Service Layer:** `Library.java` contains the business logic for issuing/returning books and searching.
- **Controller/Main:** `Main.java` handles the user interaction loop and input processing.

## 6. Project Structure
The repository is organized as follows:
- **`src/`**: Contains the Java source code (`.java` files).
- **`docs/`**: Includes the project proposal and related documentation.
- **`report/`**: Contains the final project report in PDF format.
- **`slides/`**: Includes the presentation slides for the project.
- **`com/`**: This directory is generated after compilation (contains `.class` files).

## 7. How to Run Instructions
1. Ensure you have **Java JDK 8+** installed.
2. Open your terminal in the project root directory.
3. Compile the source code:
   ```bash
   javac src/com/library/*.java -d .
   ```
4. Run the application:
   ```bash
   java com.library.Main
   ```

---

## Submission Details (IEM_Gurukul)
- **Organization:** IEM_Gurukul
- **Classroom:** Term-II Project Submission
- **Deadline:** 29 March (11:59 PM)
