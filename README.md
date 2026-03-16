# 🏫 School Store: Premium Inventory & Point of Sale (POS) System

A professional, high-performance Java desktop application designed for school store management. This system integrates real-time inventory tracking with a fast Point-of-Sale interface, ensuring accurate records and seamless transactions.

---

## 🚀 How to Run the Project

1.  **Requirement**: Ensure you have **Java JDK** installed on your computer.
2.  **Download/Clone**: Extract the project folder to your local drive.
3.  **One-Click Run**: Double-click the file named **`RunProject.bat`** located in the root folder.
    *   *This will automatically compile the source code and launch the application for you.*

---

## ✨ Key Features & Functionalities

### 1. 📦 Dynamic Inventory Management
*   **Real-time Search**: Instantly filter products as you type using the dedicated search bar.
*   **Status Dashboard**: Visual indicators (Green for Good Stock, Red for Low Stock) appear when selecting items.
*   **Full CRUD**: Easily Add, Update, or Remove products from the system.

### 2. 🛒 High-Accuracy Point of Sale (POS)
*   **Live Stock Verification**: The system prevents you from selling items that exceed current inventory levels.
*   **Real-time Dropdown**: The product selector shows available stock counts that update live as you add items to your cart.
*   **Automated Calculations**: Instantly computes subtotals and Grand Totals with currency formatting (₱).

### 3. 📊 Sales Reporting
*   **Transaction Logs**: Every sale is recorded with the product name, quantity, total price, and an exact timestamp.
*   **Persistent Storage**: Postgresql That Saves on real time via sql on the database!
---

## 🛡️ Smart Error Handling
The system is built to be "human-proof" with the following safeguards:
*   **Numeric Validation**: Blocks invalid inputs (characters/emojis) in price and quantity fields.
*   **Data Integrity**: Prevents the use of reserved characters (like commas) that could disrupt data storage.
*   **Stock Guard**: Automatically warns and blocks transactions if the requested quantity exceeds physical stock.

---

## 🛠️ Technical Overview
*   **Language**: Java SE
*   **UI Framework**: Java Swing (Custom-styled with Hover Effects)
*   **Data Handler**: Professional File I/O Management
*   **Design Pattern**: Robust Model-View-Controller (MVC) structure
*   **Database**:Postgresql

---

### 📝 Developers' Note
This project was developed with a focus on **User Experience (UX)** and **Data Reliability**. It is a perfect solution for small to medium scale school projects requiring a stable and visually clear management tool.

**Created for Practical Research 2 / School Projects** 🎓
