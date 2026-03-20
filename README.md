# 🏫 School Store: Premium Inventory & Point of Sale (POS) System

A professional, high-performance Java desktop application designed for modern school store management. This system features a completely refactored backend, transitioning from local storage to a cloud-ready **PostgreSQL** architecture for real-time data synchronization and enterprise-grade reliability.

---

## 🚀 Getting Started

1. **Requirements**: Ensure you have **Java JDK 17+** installed and a **PostgreSQL** (or Supabase) instance running.
2. **Database Setup**: 
   * Create a new database in PostgreSQL.
   * Check Datamanager For The Schema
   * Update your connection strings (Host, User, Password) in `src/data/DataManager.java`.
3. **Download/Clone**: Clone this repository to your local machine.
4. **One-Click Launch**: Double-click **`RunProject.bat`** in the root folder.
   * *This script handles automated compilation and launches the application instantly.*

---

## ✨ Advanced Features & Refactored Logic

### 1. ⚡ High-Performance Architecture (New)
* **Lazy Loading & Page Caching**: The UI now uses a smart caching system. Pages are only initialized upon first click, significantly reducing initial RAM usage and startup time.
* **Asynchronous Processing**: Integrated `SwingWorker` for all database operations. All data fetching runs on background threads, ensuring the **UI never freezes**—even during heavy inventory refreshes.
* **Ultra-Light Production Code**: The codebase has been stripped of all internal comments and redundant logic to provide a clean, high-speed execution environment.

### 2. 🎨 Modern Adaptive UI
* **Dual Theme Engine**: Seamlessly switch between **Light Mode** and **Dark Mode** via Settings.
* **Maroon & White Aesthetic**: A professional color palette designed for high-school and institutional branding.
* **Role-Based Access**: Specialized views for **ADMIN** (Inventory & Reports) and **STUDENT/USER** (Storefront & Purchases).

### 3. 🛒 Smart Point of Sale (POS)
* **Hybrid Payment Validation**: Automatically detects and separates "Cash Only" vs. "Online/GCash" items to prevent payment errors.
* **Live Stock Guard**: Real-time verification prevents users from adding items to their cart that exceed current physical inventory levels.
* **Global Order Queue**: Orders are sent to a pending list for Admin verification, ensuring inventory is only deducted once payment is confirmed.

### 4. 📦 Dynamic Inventory Management
* **PostgreSQL Integration**: Full persistent storage with support for concurrent multi-user connections.
* **Live Background Sync**: Background threads refresh stock levels every 5 seconds to ensure data accuracy across multiple terminals.
* **Visual Analytics**: Dashboard indicators for Total Revenue, Low Stock Alerts (<10 units), and Total Product count.

---

## 🛠️ Technical Stack

* **Language**: Java SE (Swing Framework)
* **Database**: PostgreSQL / Supabase (Cloud-Ready)
* **Layout Management**: `CardLayout` & `GridBagLayout` for responsive-style desktop behavior.
* **Design Tools**: Assets and UI components designed via **Adobe Photoshop**.
* **Security**: UUID-based transaction tracking and non-case/space sensitive authentication logic.

---

## 🛡️ Error Handling & Reliability
* **Human-Proof Validation**: Strict input masks for prices and quantities.
* **Reference Tracking**: Every transaction generates a unique 8-character reference code for easy auditing.
* **Auto-Sync**: Automated UI refresh cycles ensure all users see the same inventory levels in real-time.

---

### 📝 Developer's Note
This project was developed with a heavy focus on **User Experience (UX)** and **Backend Efficiency**. By moving to a PostgreSQL structure and implementing background threading, the system provides a stable, professional-grade management tool for school environments.

**Created for Practical Research 2 / School Projects** 🎓
