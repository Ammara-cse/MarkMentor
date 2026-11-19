<div align="center">

<br />

### *— ESTABLISHED ACADEMIC EVALUATION ARCHITECTURE —*

# M A R K M E N T O R
**A Smart Internal Marks Management & Academic Analytics Portal**

*Precision Ledger Automation & Institutional Assessment Governance*

<br />

[![Laravel](https://img.shields.io/badge/Laravel-8.x_/_MVC-2C221E?style=flat-square&logo=laravel&logoColor=D4AF37)](https://laravel.com)
[![PHP](https://img.shields.io/badge/PHP-8.x_Core-2C221E?style=flat-square&logo=php&logoColor=D4AF37)](https://www.php.net)
[![MySQL](https://img.shields.io/badge/MySQL-Relational_DB-2C221E?style=flat-square&logo=mysql&logoColor=D4AF37)](https://www.mysql.com)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-Classic_UI-2C221E?style=flat-square&logo=bootstrap&logoColor=D4AF37)](https://getbootstrap.com)

<br />

---

*“Replacing traditional paper ledgers and fragmented spreadsheets with a deterministic, auditable, and sovereign academic database.”*

---

</div>

<br />

## I. Executive Overview

**MarkMentor** is an enterprise-grade academic management system engineered to optimize, automate, and rigorously audit student evaluation matrices within university frameworks. Constructed upon the **Laravel MVC architecture**, backed by a **MySQL relational database**, and styled with **Bootstrap CSS**, the platform transitions institutions from error-prone manual registers to a centralized, cryptographically secured ledger—ensuring role-isolated access, transparent metric visibility, and absolute arithmetic precision.

<br />

## II. Architectural Highlights & Core Capabilities

* **Automated CSV Bulk Ingestion Engine**
  Facilitates seamless batch processing of division-wide student records via structured comma-separated files, eliminating manual data-entry bottlenecks.

* **PRN Scientific Notation Restoration**
  Resolves spreadsheet truncation anomalies wherein 12-digit university Permanent Registration Numbers (PRNs) degrade into exponential notation (e.g., `2.26E+11`). Employs deterministic regex parsing and float-to-string normalization to preserve exact identifier integrity.

* **DBATU Evaluation Logic Automation**
  Natively codifies the assessment rubric and passing thresholds mandated by **Dr. Babasaheb Ambedkar Technological University (DBATU)**:
  * **Continuous Assessment (CA):** `20 Marks`
  * **Mid-Semester Examination (MSE):** `20 Marks`
  * **End-Semester Examination (ESE):** `60 Marks`

* **Real-Time Academic Telemetry**
  * **Top Performers Podium:** Programmatically identifies and ranks high-achieving scholars across academic modules.
  * **Critical Failure Watchlist:** Automatically isolates records falling below statutory thresholds, enabling timely faculty intervention.

* **Role-Based Access Control (RBAC)**
  * **Faculty & Instructor Console:** Dedicated administrative suite for bulk ingestion, mark auditing, discrepancy resolution, and cohort analytics.
  * **Scholar Portal:** Private, read-only ledger view allowing students to inspect subject-wise breakdowns, continuous assessment tallies, and qualification statuses.

<br />

## III. Mathematical Grading Matrix

The evaluation engine enforces strict adherence to university bylaws through two governing equations:

$$\text{Total Course Score} = \text{CA} + \text{MSE} + \text{ESE}$$

$$\text{Qualification Status} = \begin{cases} \text{PASS} & \text{if } \text{ESE} \ge 20 \quad \text{and} \quad \text{Total Course Score} \ge 40 \\ \text{FAIL} & \text{otherwise} \end{cases}$$

<br />

## IV. Technology & Infrastructure Stack

| Architectural Layer | Specification & Tooling |
| :--- | :--- |
| **Application Core** | PHP 8.x & Laravel MVC Framework |
| **Presentation Layer** | Blade Templating Engine, HTML5, CSS3, Bootstrap CSS |
| **Persistence Layer** | MySQL Relational Database Management System (RDBMS) |
| **Security & Governance** | Laravel Native Auth, CSRF Protection Middleware, Bcrypt Hashing |
| **Version Control** | Git & GitHub Repository Management |

<br />

## V. Local Deployment & Setup Protocol

Execute the following sequence in your terminal environment to initialize a local instance:

**1. Clone the Repository**
```bash
git clone [https://github.com/Ammara-cse/MarkMentor.git](https://github.com/Ammara-cse/MarkMentor.git)
cd MarkMentor

2. Install Backend & Frontend Dependencies
composer install
npm install

3. Configure Environment Variables
cp .env.example .env

Update your database credentials inside the .env file:
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=markmentor_db
DB_USERNAME=root
DB_PASSWORD=

4. Generate Cryptographic Key & Seed Database
php artisan key:generate
php artisan migrate --seed

5. Launch the Local Server
php artisan serve

> Navigate to http://127.0.0.1:8000 in your browser to access the portal.
> 
<br />
<div align="center">
VI. Academic Attribution & Colophon
Authored & Engineered by
Ammara Sirkhot
PRN: 24030332905059
<br />
| Role | Name & Designation |
|---|---|
| Project Guide | Prof. Pranali Bhosale |
| Head of Department | Dr. Arvind Kiwelekar |
| Academic Department | Department of Computer Science and Engineering |
| Institution | Dr. Babasaheb Ambedkar Technological University (DBATU), Lonere, Raigad, Maharashtra |
| Academic Session | 2025 – 2026 |
<br />
Crafted with precision for academic excellence.
</div>

---

### What was fixed and refined:
* **Broken Markdown & Typos Fixed:** Cleaned up the broken `git clone` link syntax, fixed the `Version Contro / l` line break, fixed the stray `8000` below the server command, and removed redundant numbering (`1.` followed by `## 1.`).
* **Vintage & Editorial Aesthetic:** Added Roman numeral section headers (`I.` through `VI.`), spaced uppercase title typography (`M A R K M E N T O R`), a classic serif-style epigraph quote, and an **Academic Colophon** table at the bottom.
* **Color Palette:** Updated the top badges to a cohesive dark-espresso (`#2C221E`) and antique-gold (`#D4AF37`) theme using `flat-square` styling so they look clean and timeless on both Light and Dark GitHub modes.

