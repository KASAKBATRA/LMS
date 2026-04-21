# Library Management System

## Project Overview

This project is a **Library Management System** developed as part of a technical assessment. It simulates a real-world library workflow with role-based access and multiple modules including transactions, maintenance, and reporting.

The system is designed to demonstrate **logical structuring, validation handling, and complete workflow implementation** rather than focusing on backend/database integration.

---

## 🛠️ Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Data Handling:** In-memory JavaScript objects (No external database)

---

## 👥 User Roles

### 🔑 Admin

* Full access to all modules:

  * Maintenance
  * Transactions
  * Reports

### 👤 User

* Limited access:

  * Transactions only (Book Issue, Return, Fine Payment)

---

## ⚙️ Features & Modules

### 🔐 1. Login System

* Role-based login (Admin/User)
* Password masking
* Input validation

---

### 📚 2. Book Availability

* Search by Book Name or Author
* Dropdown-based selection
* Validation for empty input
* Display results in tabular format
* Option to select and issue a book

---

### 📖 3. Book Issue

* Book selection with auto-filled author
* Membership selection
* Issue Date validation (≥ current date)
* Return Date auto-calculated (+15 days)
* Optional remarks
* Error handling for missing inputs

---

### 🔁 4. Return Book

* Auto-populated details (author, serial number, issue date)
* Editable return date
* Confirmation leads to fine calculation

---

### 💰 5. Fine Payment

* Automatic fine calculation (₹ per day overdue)
* Conditional checkbox for fine payment
* Works even when no fine is applicable
* Final confirmation completes transaction

---

### 🛠️ 6. Maintenance Module (Admin Only)

#### ➤ Membership Management

* Add Membership (all fields mandatory)
* Update Membership (extend or cancel)

#### ➤ Book Management

* Add Book/Movie (radio button selection)
* Update Book status

#### ➤ User Management

* Add new users
* Modify existing users
* Role and activation control

---

### 📊 7. Reports Module

* Master List of Books
* Master List of Movies
* Membership Records
* Active Issues
* Overdue Returns
* Issue Requests

---

### 🔄 8. Transactions Module

* Book Issue
* Return Book
* Pay Fine

---

## 🧠 Business Logic & Validation

* Mandatory field validation across forms
* Date constraints (no past issue date)
* Return date limits enforced
* Fine calculation based on overdue days
* Role-based access control
* Workflow integrity (Issue → Return → Fine)

---

## ⚠️ Note on Database

This project uses **in-memory data structures** for simplicity and faster execution.

> It can be easily extended to integrate with databases such as **MySQL, MongoDB, or Firebase** for persistent storage.

---

## ▶️ How to Run

1. Open the project folder
2. Run the file:

```bash
library_management_system.html
```

3. Open in any browser (Chrome recommended)

---

## 🔑 Demo Credentials

* **Admin Login**

  * ID: `adm`
  * Password: `adm`

* **User Login**

  * ID: `user`
  * Password: `user`

---

## 🎯 Objective Achieved

This project successfully demonstrates:

* End-to-end system workflow
* Clean UI navigation
* Strong validation logic
* Modular structure
* Real-world problem understanding

---

## 🙌 Conclusion

The system fulfills all the given requirements and provides a scalable foundation for a full-stack implementation in the future.

---
