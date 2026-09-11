# MarkMentor: Smart Internal Marks Management and Academic Analytics Portal

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap" />
</p>

**MarkMentor** is an enterprise-grade web application engineered to optimize, automate, and safely audit student evaluation matrices within academic frameworks. Developed using the **Laravel MVC framework**, **MySQL relational database**, and **Bootstrap CSS**, it replaces manual registers and standalone spreadsheets with a secure, centralized database environment that ensures real-time access control, transparent metric visibility, and absolute calculation precision.

---

## 🚀 Key Features

* **Automated CSV Bulk Ingestion Engine:** Allows instructors to upload division-wide student records in batch via CSV files.
* **PRN Scientific Notation Fix:** Solves data corruption where 12-digit university Permanent Registration Numbers (PRNs) get compressed into scientific notation (e.g., `2.26E+11`) by converting and restoring them accurately using regex parsing and float-to-string normalization.
* **DBATU Evaluation Logic Automation:** Automatically calculates assessment scores and verifies Dr. Babasaheb Ambedkar Technological University (DBATU) passing criteria:
  * **Continuous Assessment (CA):** Max 20 Marks
  * **Mid-Semester Examination (MSE):** Max 20 Marks
  * **End-Semester Examination (ESE):** Max 60 Marks
  * **Passing Rule:** ESE score $\ge$ 20/60 **AND** Aggregate Total $\ge$ 40%.
* **Real-Time Academic Analytics:**
  * 🏆 **Top Performers Podium:** Programmatically highlights high-achieving students across modules.
  * ⚠️ **Critical Failure Watchlist:** Automatically flags students falling below passing thresholds for immediate academic intervention.
* **Role-Based Access Control (RBAC):**
  * **Teacher Console:** Dashboard for bulk uploads, marks entry adjustment, analytics tracking, and record audits.
  * **Student Portal:** Isolated profile view to check individual subject-wise progress, continuous evaluation breakdowns, and pass/fail indicators securely.

---

## 📐 Grading Matrix & Rules

$$\text{Total Course Score} = \text{CA} + \text{MSE} + \text{ESE}$$

$$\text{Passing Flag} = \begin{cases} \text{PASS} & \text{if } \text{ESE} \ge 20 \text{ and } \text{Total Course Score} \ge 40 \\ \text{FAIL} & \text{otherwise} \end{cases}$$

---

## 🛠️ Tech Stack

* **Backend Framework:** PHP 8.x / Laravel MVC Framework
* **Frontend:** Blade Templating Engine, HTML5, CSS3, Bootstrap CSS
* **Database:** MySQL Relational Database Management System (RDBMS)
* **Authentication & Security:** Built-in Laravel Auth, CSRF Protection Middleware, Password Hashing
* **Version Contro
* l:** Git & GitHub

---

## ⚙️ Installation & Local Setup Guide

Follow these steps to set up the project on your local system:

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/Ammara-cse/MarkMentor.git](https://github.com/Ammara-cse/MarkMentor.git)
   cd MarkMentor

## 1. Install Composer Dependencies:<br>
   composer install

## 2.Install NPM Packages:<br>
npm install

## 3.Environment Configuration:<br>
Create a .env file by copying .env.example:
cp .env.example .env


## Configure your MySQL database settings in the .env file:<br>
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=markmentor_db
DB_USERNAME=root
DB_PASSWORD=

## 4.Generate Application Key:<br>
php artisan key:generate


## 5.Run Database Migrations and Seeders:<br>
php artisan migrate --seed


## 6.Start the Development Server:<br>
php artisan serve
Access the application in your browser at: http://127.0.0.1:8000

8000

---
# 👥 Authors & Academic Credits
### Sara Wadhaval (PRN: 24030332905055)<br>
### Ammara Sirkhot (PRN: 24030332905059)<br>
### Under the Guidance of: Prof. Pranali Bhosale<br>
### Head of Department: Dr. Arvind Kiwelekar<br>
# Department: Department of Computer Science and Engineering<br>
# University: Dr. Babasaheb Ambedkar Technological University (DBATU), Lonere, Raigad, Maharashtra, India.<br>
## Academic Year: 2025–2026
