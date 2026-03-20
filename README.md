# 🏫 School Store: Premium Inventory & Point of Sale (POS) System

A professional, high-performance Java desktop application designed for school store management. This system integrates real-time inventory tracking with a fast Point-of-Sale interface, ensuring accurate records and seamless transactions with a modern, adaptive UI.

---

## 🚀 How to Run the Project

1.  **Requirement**: Ensure you have **Java JDK** installed and a **PostgreSQL** instance running.
2.  **Database Setup**: Create a database in PostgreSQL and update the connection details in `DataManager.java`.
3.  **Download/Clone**: Extract the project folder to your local drive.
4.  **One-Click Run**: Double-click the file named **`RunProject.bat`** located in the root folder.
    * *This will automatically compile the source code and launch the application for you.*

---

## ✨ Key Features & Functionalities

### 1. 🎨 Modern Adaptive UI
* **Dual Theme Support**: Switch between **Light Mode** and **Dark Mode** via the Settings panel for better accessibility.
* **Role-Based Access**: Specialized views for **ADMIN** (Full Control) and **STUDENT/USER** (Purchase Only) roles.
* **Responsive Sidebar**: Navigation with hover effects and active-state tracking for a fluid user experience.

### 2. 🛒 Advanced Point of Sale (POS) & Order Queue
* **Hybrid Payment Logic**: Intelligent validation that separates "Cash Only" and "Online Only" items in the cart to prevent payment incompatibility.
* **Global Order Queue**: Orders are sent to a pending list for Admin approval, ensuring stock is only deducted upon verified payment.
* **Automated Receipting**: Generates professional, monospaced digital receipts upon order approval.
* **Visual Instructions**: Pop-up guides for GCash (Online) and Cashier (Physical) payment workflows.

### 3. 📦 Dynamic Inventory & Product Management
* **Live Stock Tracking**: Real-time background threads refresh stock levels every 5 seconds.
* **Low Stock Alerts**: Visual dashboard indicators highlight items with fewer than 10 units remaining.
* **Full CRUD**: Dedicated interface to Add, Update, or Delete products with immediate table synchronization.

### 4. 📊 Real-Time Analytics
* **Admin Dashboard**: Instant summaries of Total Products, Low Stock count, and Total Revenue.
* **Transaction Logs**: Comprehensive sales reports featuring product names, quantities, revenue, and exact timestamps.

---

## 🛡️ Smart Error Handling & Security
The system is built to be "human-proof" with the following safeguards:
* **Concurrency Management**: Uses `SwingWorker` for background data fetching to ensure the UI never freezes during database operations.
* **Input Validation**: Blocks non-numeric entries in price and quantity fields and prevents empty submissions.
* **Reference Tracking**: Generates unique 8-character UUID reference codes for every transaction to simplify order lookups.
* **Stock Guard**: Prevents adding items to the cart that exceed current physical inventory levels.

---

## 🛠️ Technical Overview
* **Language**: Java SE
* **UI Framework**: Java Swing (Custom-styled with `CardLayout` and `GridBagLayout`)
* **Database**: PostgreSQL (Persistent SQL Storage)
* **Architecture**: Robust Model-View-Controller (MVC) structure
* **Timer System**: Automated UI refresh cycles for multi-user synchronization.

---

### 📝 Developers' Note
This project was developed with a focus on **User Experience (UX)** and **Data Reliability**. It provides a stable, visually clear, and professional management tool for modern school environments.

**Created for Practical Research 2 / School Projects** 🎓
