# 🏦 C++ Bank Management System Project

A comprehensive console-based Bank Management System developed in **C++**. This project implements core Object-Oriented Programming principles, file handling, vector manipulation, role-based user permissions, and robust client/user data management.

---

## ✨ Features

### 1. 👥 Client Management
- **Add New Clients:** Allows adding multiple clients with automatic validation to ensure account numbers are unique.
- **Client List:** Displays a formatted table listing all registered bank clients along with their total account count.
- **Find Client:** Quick search functionality to locate specific clients using their Account Number.
- **Update Client Info:** Modify existing client details such as Pin Code, Full Name, Phone Number, and Account Balance.
- **Delete Client:** Soft/Hard deletion of client records from the system files.

### 2. 💸 Transactions Menu
- **Deposit:** Add funds securely to a client's account balance.
- **Withdraw:** Deduct funds with balance-check validation to prevent overdrafts.
- **Total Balances:** View the cumulative balance of all accounts in the system.

### 3. 🔐 User & Permissions Management (Multi-user System)
- **Manage Users:** Add, list, update, and delete system users.
- **Role-Based Access Control (RBAC):** Restricts access to specific system features (e.g., Client List, Add Client, Delete, Update, Transactions, and User Management) using bitwise permission enums.

---

## 🛠️ Technologies & Concepts Used
- **Language:** C++
- **File I/O:** Reading from and writing to text files (`<fstream>`) using custom record delimiters (`#//#`).
- **Data Structures:** `struct` for structuring Client and User records, and `vector` for in-memory data manipulation.
- **Standard Libraries:** `<iostream>`, `<vector>`, `<string>`, `<iomanip>`, `<fstream>`.

---

## 📂 File Structure & Data Formatting
- Client records are structured and saved line-by-line using a custom separator (`#//#'`):
  ```text
  AccountNumber#//#PinCode#//#FullName#//#Phone#//#Balance
