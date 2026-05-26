# 🎓 School Performance Analytics Dashboard Template

A highly premium, data-driven, and customizable web application built to audit and visualize student enrollees, GAD (Gender and Development) profiles, cohort retention rates, facilities capacity, and staffing distributions for basic and secondary education levels.

This repository is a **reusable template**. Any school can instantly download it, run the setup wizard, configure their offered academic tiers, and deploy a tailored analytics dashboard in minutes!

---

## ✨ Features

- **🎓 Multi-Tier Grade Level Flexibility**: Choose which tiers your school offers (Kindergarten, Elementary, JHS, and/or SHS) during first-time setup or system settings. The entire dashboard dynamically hides/shows cards, tables, charts, and pages based on active tiers!
- **⚡ Executive Key Performance Indicators**: Live monitoring of Total BOSY Enrollment, Repeater Rates, Dropout Rates, Seat Sufficiency, Floor Area per Student, and Student-to-Teacher workload ratios.
- **📊 Vibrant Interactive Visualization**: Responsive, semantic high-contrast Chart.js charts covering multi-grade enrollees, longitudinal trend step-curves, facility functional distributions, and HR staffing charts.
- **👩‍🎓 Premium Student Portal View**: A glassmorphic landing board for students to access school announcements, explore Senior High track curriculum mappings (Academic & TVL), and see learning resources.
- **🏢 Real-time Classroom & Seats Inventory**: Manage floor areas, functional capacities, and grade-level seat shortages dynamically.
- **🛡️ Dynamic Cohort Persistence Heatmaps**: Diagnostic cohort retention tracking over 6 years with built-in rule engines offering actionable DepEd standard recommendations.
- **📋 Official Summary Report Exports**: Standard DepEd header layout, automated GAD breakdown charts, data-driven narrative analysis, and authorized signature blocks, exportable to print or PDF in one click.

---

## 🛠️ Technology Stack

- **Core**: HTML5, Vanilla JavaScript, PHP 7.4+
- **Styling**: Vanilla CSS3 (curated theme palette, glassmorphism, responsive grids)
- **Database**: MariaDB / MySQL
- **Dependencies**: Chart.js (v4), Bootstrap Icons, SweetAlert2

---

## 🚀 Installation & Setup

Deploying this template locally or on a server is straightforward:

### 1. Prerequisites
- **Local Server**: Install [XAMPP](https://www.apachefriends.org/) (includes PHP and MariaDB/MySQL).

### 2. Codebase Deployment
1. Clone this repository into your XAMPP local root directory (`htdocs`):
   ```bash
   git clone https://github.com/your-username/school-performance-dashboard.git
   ```
2. Open XAMPP Control Panel and start **Apache** and **MySQL**.

### 3. Database Initialization
1. Open your browser and navigate to [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
2. Create a new database named `school_dashboard_db` (or any custom name).
3. Select the database, click the **Import** tab, choose the clean SQL seed file located under:
   ```filepath
   database/database_template.sql
   ```
4. Click **Import** to seed the tables and baseline configurations.

### 4. Configuration
1. Open `config/db_connect.php` in a text editor.
2. Under the database settings block, update `DB_NAME`, `DB_USER`, and `DB_PASS` to match your local setup:
   ```php
   define('DB_HOST', 'localhost');
   define('DB_USER', 'root');
   define('DB_PASS', '');
   define('DB_NAME', 'school_dashboard_db');
   ```

### 5. Launch the Setup Wizard! 🚀
1. Open your browser and visit:
   ```url
   http://localhost/school-performance-dashboard-template/
   ```
2. The system will detect that setup is incomplete and redirect you to the **Setup Wizard (`setup.php`)**.
3. Fill out your school information (Name, School ID, Division, Tagline, Logo, Address, and offered Grade Levels).
4. Save and launch your tailored school performance dashboard!

---

## 👥 Default Credentials

For local testing and administration:
- **Username**: `admin`
- **Password**: `admin123` (configured under pre-seeded users in `users` table)

---

## 🤝 Contributing

Contributions, bug fixes, and feature expansions are welcome! Feel free to open a Pull Request or report an issue in the GitHub issue tracker.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
