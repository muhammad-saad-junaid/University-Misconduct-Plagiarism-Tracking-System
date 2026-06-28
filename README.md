# University Misconduct & Plagiarism Tracking System

> Database Management Systems Project — COMSATS University Lahore (5th Semester)  
> **Course:** Database Systems (CSC270) | **Supervisor:** Prof. Modassir Ashfaq

---

## 📌 Overview
A fully database-driven backend system designed to systematically record, manage, and analyze cases of academic misconduct such as plagiarism, cheating, impersonation, and disruptive behavior across a university environment.

Built entirely using **SQL Server** — no frontend interface. All operations performed through DDL, DML, triggers, stored procedures, views, transactions, and role-based authorization.

---

## 🗄️ Database Design
- **Normalization:** 3NF — redundancy minimized, lookup tables used for consistency
- **Entities:** 9 major entities
- **Relationships:** Enforced via foreign keys with cascading actions
- **Business Rules:** Enforced through constraints and triggers

---

## 🏗️ Entities
| Entity | Purpose |
|--------|---------|
| Students | Student profile and enrollment data |
| Teachers | Faculty member records |
| Courses | Course catalog with department mapping |
| MisconductTypes | Standardized categories with severity levels (1–5) |
| MisconductReports | Core transactional table — connects all entities |
| Evidence | Supporting files per misconduct case |
| Appeals | Student appeal submissions with auto status updates |
| ActionLogs | Full audit trail — retained even after report deletion |
| MonthlyReports | Pre-aggregated statistics for admin reporting |

---

## ⚙️ Features Implemented
- **ACID-Compliant Transactions** — data consistency guaranteed
- **Triggers** — auto-update report status on appeal submission, auto-generate monthly summaries
- **Stored Procedures** — encapsulated business logic for reporting and case management
- **Role-Based Access Control** — separate permissions for Teachers and Students
- **Audit Logging** — every critical action recorded with timestamps
- **Indexes** — strategically placed for query performance
- **Views** — analytical views for repeat offender tracking and severity trends
- **Cascade Rules** — evidence and appeals cascade-delete with reports; logs preserved

---

## 🛠️ Tech Stack
| Component | Technology |
|-----------|-----------|
| Database | SQL Server |
| Query Language | T-SQL |
| Design | Relational Model, 3NF Normalization |
| Tools | SQL Server Management Studio (SSMS) |

---

## 👥 Authors
**Muhammad Saad Junaid** (FA23-BCE-107)  
Computer Engineering — COMSATS University Lahore  
🔗 [LinkedIn](https://linkedin.com/in/m-saad-junaid)
