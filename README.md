# Medicine Management System

A lightweight, console-based **Medicine Management System** built in C++. This application utilizes Object-Oriented Programming (OOP) concepts alongside file handling mechanics to manage a medical store's inventory and streamline customer billing.

## Features

* **View Inventory:** Display all available medicines currently stored in the database.
* **Billing System:** Search for specific medicines, calculate total costs based on quantity, automatically apply a 12% tax rate, and generate/save receipt data.
* **Add Medicine:** Easily append new stock and medicines directly into the permanent inventory file.
* **Delete Medicine:** Efficiently remove expired or out-of-stock items from the record using an automated temporary file swapping mechanism.

## Concepts Used
This project showcases fundamental and intermediate features of the C++ programming language:
* **Object-Oriented Programming (OOP):** Uses classes (`med`, `med1`, `option`) to cleanly separate responsibilities and store related attributes.
* **Multiple Inheritance:** The `option` class inherits from both `med` and `med1` to combine capabilities into a single menu interface.
* **File Handling (`fstream`):** Implements `ifstream` and `ofstream` to read, write, and safely modify external data stores (`med.txt` and `billing.txt`).
* **Stream Manipulation:** Utilizes `getline()` and file buffers to accurately scan strings and modify specific text segments.

## How to Run

### Prerequisites

Make sure you have a C++ compiler installed (such as `g++` via GCC).

### Compilation

Open your terminal or command prompt and run the following command:

```bash
g++ main.cpp -o MedicineManagement
```

### Execution

Run the compiled executable:

* **Windows:**
```cmd
MedicineManagement.exe
```

## Sample Preview

```text
  ********************WELCOME TO THE MEDICAL STORE MANAGEMENT***********************
      Enter the choice:
  1. SHOW ALL THE MEDICINE AVAILABLE
  2. BILLING
  3. ADD MEDICINE
  4. DELETE MEDICINE
  5. EXIT

```

## Future Enhancements

* Add user authentication and login roles (Admin vs. Cashier).
* Implement real-time quantity updates (automatically decrementing stock counts upon billing).
* Transition from flat `.txt` files to structured files (like `.csv` or an SQLite database) for better relational tracking.
