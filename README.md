# 🎓 MarkMentor
### Smart Internal Marks Management & Academic Analytics Portal

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/PHP_8.x-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap" />
</p>

<p align="center">
  <strong>
    An enterprise-grade academic portal engineered to automate, audit,
    and visualize student evaluation matrices within university frameworks.
  </strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Academic%20Year-2025--2026-0F172A?style=flat-square" />
  <img src="https://img.shields.io/badge/Institution-DBATU-1E3A8A?style=flat-square" />
  <img src="https://img.shields.io/badge/Architecture-MVC-334155?style=flat-square" />
</p>

---

## 📖 Overview

**MarkMentor** is a smart academic marks management and analytics portal designed to replace manual registers and error-prone spreadsheets with a centralized, secure database environment.

Built using the **Laravel MVC architecture**, MarkMentor is designed around the assessment framework of **Dr. Babasaheb Ambedkar Technological University (DBATU)**.

The system provides:

- 📥 Automated academic data ingestion
- 🔐 Role-based access control
- 🧮 Automated marks calculation
- ⚠️ Pass/fail auditing
- 🏆 Student performance ranking
- 📊 Academic analytics
- 🔎 Transparent subject-wise performance tracking

---

## 🚀 Key Features

### ⚙️ Data Ingestion & Integrity

- **Automated CSV Bulk Ingestion**  
  Upload division-wide student records and subject marks through a single batch operation.

- **PRN Scientific Notation Recovery**  
  Prevents spreadsheet corruption where 12-digit Permanent Registration Numbers (PRNs) are converted into scientific notation such as `2.26E+11`.

- **Data Validation**  
  Validates imported academic records before storing them in the database.

---

### 📊 Academic Intelligence & Analytics

- **DBATU Evaluation Rule Engine**  
  Automatically calculates aggregate marks and applies university passing criteria.

- **🏆 Top Performers Podium**  
  Programmatically ranks students and highlights high-performing students across modules.

- **⚠️ Critical Failure Watchlist**  
  Automatically identifies students who fall below passing criteria, helping faculty take timely action.

- **📈 Performance Monitoring**  
  Provides structured academic information for monitoring student progress.

---

### 🔐 Role-Based Access Control (RBAC)

#### 👨‍🏫 Teacher Console

Provides faculty members with:

- CSV bulk import
- Student record management
- Mark editing
- Subject-wise analytics
- Cohort performance analysis
- Audit logs

#### 👨‍🎓 Student Portal

Provides students with an isolated, read-only academic profile containing:

- Subject-wise marks
- CA / MSE / ESE breakdown
- Total marks
- Pass/fail status
- Academic performance information

---

## 📐 Grading Matrix & Evaluation Rules

### Assessment Structure

| Component | Code | Maximum Marks | Weightage |
| :--- | :---: | :---: | :---: |
| **Continuous Assessment** | `CA` | 20 | 20% |
| **Mid-Semester Examination** | `MSE` | 20 | 20% |
| **End-Semester Examination** | `ESE` | 60 | 60% |
| **Aggregate Total** | **`TOTAL`** | **100** | **100%** |

### 🧮 Mathematical Evaluation Logic

$$
\text{Total Course Score} =
\text{CA} + \text{MSE} + \text{ESE}
$$

$$
\text{Result Status} =
\begin{cases}
\text{PASS} & \text{if ESE} \ge 20 \text{ and Total Course Score} \ge 40 \\
\text{FAIL} & \text{otherwise}
\end{cases}
$$

### ✅ Evaluation Summary

| Condition | Result |
| :--- | :---: |
| ESE ≥ 20 **and** Total ≥ 40 | 🟢 **PASS** |
| ESE < 20 | 🔴 **FAIL** |
| Total < 40 | 🔴 **FAIL** |


---

🛠️ Tech Stack

Layer	Technology

Backend Framework	PHP 8.x, Laravel MVC
Frontend & Templating	Laravel Blade, HTML5, CSS3, Bootstrap 5
Database	MySQL Relational Database Management System (RDBMS)
Security & Authentication	Laravel Native Auth, CSRF Middleware, Bcrypt Password Hashing
Version Control	Git & GitHub



---

### 🔐 Security

MarkMentor follows application-level security practices including:

- 🔑 Authentication & Authorization
- 🛡️ Role-Based Access Control
- 🔒 Bcrypt Password Hashing
- 🛡️ CSRF Protection
- 🚫 Restricted Student Access
- 📝 Audit Logging


---

### 📥 Data Processing Workflow

CSV File
   │
   ▼
Data Validation
   │
   ▼
PRN Normalization
   │
   ▼
Marks Processing
   │
   ▼
Database Storage
   │
   ▼
Evaluation Engine
   │
   ├──► PASS / FAIL
   ├──► Rankings
   ├──► Failure Watchlist
   └──► Academic Analytics


---

### ⚙️ Installation & Local Setup

Follow these steps to deploy MarkMentor locally.

1. Clone the Repository

git clone https://github.com/Ammara-cse/MarkMentor.git
cd MarkMentor

2. Install Backend & Frontend Dependencies

composer install
npm install

3. Configure Environment Variables

Duplicate the example environment file:

cp .env.example .env

Generate the Laravel application key:

php artisan key:generate

Open .env and configure the MySQL database:

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=markmentor_db
DB_USERNAME=root
DB_PASSWORD=

4. Run Migrations & Seeders

php artisan migrate --seed

5. Launch the Development Server

php artisan serve

Open your browser and navigate to:

http://127.0.0.1:8000


---

### 📁 Project Workflow

User Login
    │
    ├── Teacher
    │     │
    │     ├── Import CSV
    │     ├── Manage Marks
    │     ├── View Analytics
    │     └── Monitor Students
    │
    └── Student
          │
          ├── View Profile
          ├── View Subject Marks
          ├── View Total
          └── View Result Status


---

### 🎯 Project Objectives

MarkMentor aims to:

- Reduce dependency on manual academic registers.
- Minimize calculation and data-entry errors.
- Automate DBATU-based evaluation rules.
- Provide centralized academic records.
- Improve faculty monitoring of student performance.
- Provide students with transparent access to their marks.
- Enable data-driven academic analysis.


---

### 👥 Author & Academic Credits

Role	Details

Developer	Ammara Sirkhot
Project Guide	Prof. Pranali Bhosale
Head of Department	Dr. Arvind Kiwelekar
Department	Department of Computer Science and Engineering
Institution	Dr. Babasaheb Ambedkar Technological University (DBATU), Lonere, Raigad, Maharashtra
Academic Year	2025–2026



---

### 🏛️ Academic Context

Institution:
Dr. Babasaheb Ambedkar Technological University (DBATU)

Department:
Department of Computer Science and Engineering

Location:
Lonere, Raigad, Maharashtra

Academic Year:
2025–2026


---

### 🌟 Why MarkMentor?

> From manual marks management to intelligent academic analytics.



MarkMentor transforms fragmented academic records into a structured digital system that makes evaluation faster, more reliable, transparent, and easier to monitor.


---

### 📌 Project Status

MarkMentor is an academic software project developed to demonstrate practical implementation of:

- Laravel MVC
- Relational database design
- Authentication & authorization
- CSV data processing
- Automated evaluation logic
- Academic analytics
- Role-based dashboards


---

<p align="center">
  <strong>Built with 💻 by Ammara Sirkhot</strong>
</p><p align="center">
  <sub>Department of Computer Science & Engineering • DBATU • 2025–2026</sub>
</p>
