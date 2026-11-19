🎓 MarkMentor

Smart Internal Marks Management & Academic Analytics Portal

<p align="center">An academic management system designed to automate internal assessment, result evaluation, and student performance analytics.

<br/><img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel"/>
<img src="https://img.shields.io/badge/PHP_8.x-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"/>
<img src="https://img.shields.io/badge/Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap"/><br/><img src="https://img.shields.io/badge/Architecture-Laravel%20MVC-0F172A?style=flat-square" alt="Architecture"/>
<img src="https://img.shields.io/badge/Database-MySQL-0F172A?style=flat-square" alt="Database"/>
<img src="https://img.shields.io/badge/Status-Active-0F172A?style=flat-square" alt="Status"/></p>---

📌 Overview

MarkMentor is a role-based academic portal developed to replace manual mark registers and error-prone spreadsheets with a centralized database-driven system.

The system is designed around DBATU's internal assessment structure and provides automated result evaluation, role-based access, bulk mark ingestion, student performance analytics, and academic risk identification.

Core Objectives

- Centralize student academic records
- Automate internal mark calculations
- Apply predefined pass/fail rules consistently
- Reduce manual data-entry and calculation errors
- Provide teachers with actionable academic analytics
- Give students a transparent view of their academic performance

---

✨ Key Features

📥 1. Data Ingestion & Integrity

CSV Bulk Import

Import division-level student records and subject marks through a single CSV upload workflow.

PRN Scientific-Notation Recovery

Handles spreadsheet corruption where long PRNs may be converted into scientific notation.

Example:

Original PRN
22603032905059

Corrupted spreadsheet value
2.2603E+13

Recovered PRN
22603032905059

The ingestion layer validates and normalizes PRN values before storing them in the database.

---

📊 2. Academic Intelligence & Analytics

Automated Result Evaluation

MarkMentor calculates aggregate marks and applies the configured DBATU evaluation rules automatically.

Top Performers

Ranks students based on academic performance and highlights high-performing students.

Critical Failure Watchlist

Identifies students who do not satisfy the required passing criteria, allowing faculty to quickly identify students who may require academic support.

---

🔐 3. Role-Based Access Control

Role| Capabilities
Teacher| Import marks, edit records, view analytics, monitor students
Student| View personal marks, subject-wise performance and result status

The student interface is designed as a read-only academic profile, while teachers receive administrative and analytical capabilities.

---

📐 Evaluation Rules

Assessment Structure

Component| Code| Maximum Marks| Weightage
Continuous Assessment| "CA"| 20| 20%
Mid-Semester Examination| "MSE"| 20| 20%
End-Semester Examination| "ESE"| 60| 60%
Total| "TOTAL"| 100| 100%

Result Calculation

Total = CA + MSE + ESE

Pass Criteria

A student is considered PASS when:

ESE >= 20
AND
Total >= 40

Otherwise:

FAIL

This rule is implemented programmatically to ensure consistent evaluation across student records.

---

🏗️ System Architecture

                    ┌─────────────────────┐
                    │      User Layer     │
                    │ Teacher / Student   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Laravel Web Layer │
                    │ Routes / Controllers │
                    │       / Blade       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Business Logic    │
                    │ Evaluation / RBAC    │
                    │ Analytics / Import   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       MySQL         │
                    │ Relational Database  │
                    └─────────────────────┘

---

🛠️ Technology Stack

Layer| Technology
Backend| PHP 8.x
Framework| Laravel
Architecture| MVC
Frontend| HTML5, CSS3, Bootstrap 5
Templating| Laravel Blade
Database| MySQL
Authentication| Laravel Authentication
Security| CSRF Protection, Bcrypt Password Hashing
Data Import| CSV
Version Control| Git & GitHub

---

📁 Project Structure

MarkMentor/
│
├── app/
│   ├── Http/
│   ├── Models/
│   └── ...
│
├── database/
│   ├── migrations/
│   └── seeders/
│
├── resources/
│   └── views/
│
├── routes/
│   └── web.php
│
├── public/
│
├── .env.example
├── composer.json
├── package.json
└── README.md

---

⚙️ Installation & Local Setup

1. Clone the Repository

git clone https://github.com/Ammara-cse/MarkMentor.git
cd MarkMentor

2. Install Dependencies

composer install
npm install

3. Configure Environment

Create the environment file:

cp .env.example .env

Generate the Laravel application key:

php artisan key:generate

Configure your MySQL database inside ".env":

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=markmentor_db
DB_USERNAME=root
DB_PASSWORD=

4. Run Database Migrations

php artisan migrate --seed

5. Start the Development Server

php artisan serve

Open:

http://127.0.0.1:8000

---

🔒 Security Considerations

MarkMentor incorporates several application-level security mechanisms:

- Role-based access control
- CSRF protection through Laravel middleware
- Password hashing using Bcrypt
- Server-side validation
- Controlled student access to academic records
- Database-backed authentication

«Production deployment should additionally configure HTTPS, secure environment variables, database backups, rate limiting, and production-grade authentication policies.»

---

📈 Future Enhancements

Potential improvements include:

- 📱 Responsive mobile-first student portal
- 📊 Interactive performance dashboards
- 📈 Subject-wise performance trends
- 📧 Automated academic alerts
- 📄 PDF result generation
- 🔔 Faculty notification system
- 🧠 Predictive identification of academically at-risk students
- 📚 Multi-semester academic history
- ☁️ Cloud deployment and centralized hosting

---

🎯 Project Impact

MarkMentor demonstrates how a traditional academic workflow can be transformed into a centralized, automated and analytics-driven information system.

The project focuses on:

Manual Data → Structured Data → Automated Evaluation → Actionable Analytics

This reduces repetitive faculty work while improving consistency, visibility, and accessibility of academic information.

---

👩‍💻 Author

Ammara Sirkhot

Department of Computer Science & Engineering
Dr. Babasaheb Ambedkar Technological University (DBATU)
Lonere, Raigad, Maharashtra, India

Academic Year: 2025–2026

Project Guide

Prof. Pranali Bhosale

Head of Department

Dr. Arvind Kiwelekar

---

⭐ Acknowledgement

Developed as an academic project for exploring web application development, database management, role-based security, automation, and academic analytics using the Laravel ecosystem.

---

<p align="center">⭐ If you find this project useful, consider starring the repository!

MarkMentor — Making Academic Data Smarter.

</p>