# 🏧 Simple ATM Management System in C++

A lightweight, console-based **ATM (Automated Teller Machine) System** developed in C++. This application allows authenticated users to manage their bank accounts through file-based data persistence, providing features such as quick withdrawals, custom withdrawals, deposits, and real-time balance checks.

---

## ✨ Features

* **🔐 User Authentication:** Secure login system validating Account Number and PIN against stored records.
* **⚡ Quick Withdraw:** Fast withdrawal presets (20, 50, 100, 200, 400, 600, 800, 1000).
* **💵 Normal Withdraw:** Custom withdrawal amounts (restricted to multiples of 5).
* **💰 Deposit System:** Easy account balance deposits with real-time file updates.
* **📊 Check Balance:** Instant display of the current account balance.
* **📁 File-Based Data Persistence:** Automatically reads and writes client records to a text file (`Clinet.txt`).

---

## 🛠️ Built With

* **Language:** C++ (C++11 or later recommended)
* **File I/O:** Standard Library Streams (`fstream`)
* **Data Structures:** `std::vector`, `struct`, `enum`

---

## 📂 File Format Specification

The system uses a custom text file database named **`Clinet.txt`**. Data records are separated by the `#//#` delimiter.

### Record Format:
`AccountNumber#//#PinCode#//#Name#//#Phone#//#AccountBalance`

### Sample `Clinet.txt`:
```text
A101#//#1234#//#John Doe#//#0501234567#//#5000.00
A102#//#4321#//#Jane Smith#//#0507654321#//#1200.50
```

---

## 🚀 How to Run

### 1. Prerequisites
Make sure you have a C++ compiler installed (e.g., `g++`, `clang`, or MSVC).

### 2. Prepare Data File
Create a file named `Clinet.txt` in the same directory as the executable with sample client data (like the sample above).




---

## 🎮 How to Use

1. **Login:** Enter a valid Account Number and PIN stored in `Clinet.txt`.
2. **Main Menu Options:**
   - **[1] Quick Withdraw:** Pick a predefined amount to withdraw instantly.
   - **[2] Normal Withdraw:** Enter a custom amount (must be a multiple of 5).
   - **[3] Deposit:** Enter an amount to add to your balance.
   - **[4] Check Balance:** View your current available funds.
   - **[5] Logout:** Log out and return to the login screen.

---

## 💡 Future Improvements
- [ ] Add encryption for PIN numbers inside the text file.
- [ ] Cross-platform screen clearing (`cls` for Windows / `clear` for Unix).
- [ ] Add input sanitation to handle invalid non-numeric inputs gracefully.
- [ ] Implement administrative features (e.g., Add New Client, Delete Client).
