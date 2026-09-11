# MarkMentor: Smart Internal Marks Management and Academic Analytics Portal

**MarkMentor** is an enterprise-grade web application engineered to optimize, automate, and safely audit student evaluation matrices within academic frameworks. Built using the **Laravel MVC framework**, **MySQL**, and **Bootstrap CSS**, it replaces manual ledgers and error-prone spreadsheets with a secure, centralized database system.

---

## 🌟 Key Features

* **Automated CSV Bulk Ingestion Engine:** Allows faculty members to upload batch student marks with built-in data sanitization.
* **PRN Scientific Notation Fix:** Solves data corruption issues where 12-digit university Permanent Registration Numbers (PRNs) get compressed into scientific notation (e.g., `2.26E+11`) by converting and restoring them accurately via regex parsing.
* **DBATU Grading Logic Automation:** Programmatically calculates assessment scores and verifies DBATU passing criteria:
  * Continuous Assessment (CA): Max 20 Marks
  * Mid-Semester Exam (MSE): Max 20 Marks
  * End-Semester Exam (ESE): Max 60 Marks
  * *Passing Threshold:* ESE $\ge$ 20 out of 60 and Cumulative Score $\ge$ 40%.
* **Real-Time Academic Analytics:**
  * **Top Performers Podium:** Displays high-achieving students in real time.
  * **Critical Failure Watchlist:** Automatically flags students falling below passing boundaries for academic intervention.
* **Role-Based Access Control (RBAC):**
  * **Teacher Console:** Bulk data uploads, mark entry adjustments, and analytics access.
  * **Student Portal:** Isolated profile view to check individual subject-wise progress and aggregate results securely.

---

## 🛠️ Tech Stack

* **Backend Framework:** PHP 8.x / Laravel (MVC Architecture)
* **Frontend:** HTML5, CSS3, Bootstrap CSS, Laravel Blade Engine
* **Database:** MySQL Relational Database
* **Version Control:** Git & GitHub

---

## 💻 Installation & Setup Guide

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/Ammara-cse/MarkMentor.git](https://github.com/Ammara-cse/MarkMentor.git)
   cd MarkMentor
