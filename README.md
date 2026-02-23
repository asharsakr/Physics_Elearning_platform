# Physics E-Learning Management System (DBMS Project)

## Project Overview

Developed in response to the shift toward digital education post-COVID-19, this Database Management System is designed to streamline the workflow for Physics teachers. The platform manages educational content, student progress, and communication between teachers, assistants, parents, and students.

The system's core logic ensures academic integrity by gatekeeping advanced lessons until students pass assessment milestones with a required percentage.

## Tech Stack
Framework: ASP.NET Razor Pages

Database: SQL Server (Relational Schema)

Logic: C# (Session management, Validation, and Authentication)

Frontend: HTML5, CSS3, JavaScript (integrated with Razor syntax)
## Key Features

### For Students

* **Structured Learning:** Access to materials categorized by secondary school year (1st, 2nd, and 3rd).
* **Automated Gatekeeping:** Students must pass an assessment test to unlock subsequent lectures.
* **Progress Tracking:** Personal dashboard to view quiz grades and performance statistics.
* **Interaction:** Dedicated section for student-to-student communication and a practice question bank.

### For Teachers & Assistants

* **Content Management:** Upload PDF summaries and video lectures.
* **Assessment Engine:** Create complex quizzes using a tiered question bank (categorized by difficulty and chapter).
* **User Oversight:** Teachers can manage (add/delete/update) students and assistants.
* **Status Monitoring:** Assistants can update student statuses (continuing vs. quitting).

###  For Parents

* **Performance Monitoring:** Direct access to view their child’s quiz grades and attendance.
* **Direct Communication:** Integrated contact page to reach out to teachers.

---

##  Database Design

### Entity-Relationship (ER) Highlights

The system is built on a robust relational schema involving 10+ entities including `Teacher`, `Student`, `Questions`, `Quizzes`, `Multimedia`, and `Progress`.

**Key Relationships:**

* **Many-to-Many ():** Questions to Quizzes, Multimedia to Students, and Assistants to Quizzes.
* **One-to-Many ():** Teacher to Students/Assistants/Progress, and Parent to Progress records.
* **One-to-One ():** Student to Parent and Student to Progress.

### Schema Preview

The database handles complex attributes such as:

* **Questions:** Difficulty levels (1–30) and chapter mapping.
* **Progress:** Tracks specific metrics like "watched videos," "attendance," and "practice counts."

---

##  Technical Implementation & Team

This project was a collaborative effort , focusing on back-end logic, session management, and database integration.

| Name | Role / Focus |
| --- | --- |
| **Ashar Salama** | Back-end Session management, Authentication/Validation, and Password Security. |
| **Nada Mohamed** | Multimedia handling (PDFs/Videos), User Management UI, and Grade display. |
| **Dolagy George** | Progress logic, Quiz/Question database integration, and Multimedia support. |
