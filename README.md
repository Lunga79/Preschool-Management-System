# Preschool-Management-System
A web based Preschool management designed to enhance school administration and public engagement through online admissions, recruitment and job applications,event calendar management and school gallery, supported by administrative dashboard for managing and publishing information.

# Little Stars Preschool Management System

## 1. Project Overview
The **Little Stars Preschool Management System** is a web-based application developed using html, css, php and MySQL. The system provides an online platform for managing preschool information, student admissions, job postings, and administrative content.

Parents can:
- Apply for admission
- View school events
- Explore the gallery
- Apply for employment opportunities

Administrators have a secure interface to manage dynamic website content.

---

## 2. Objectives
The primary objectives of this project are:
- Develop a dynamic school website using server-side scripting
- Implement a database-driven content management system
- Provide online admission and job application functionality
- Integrate email notifications using SMTP
- Implement session-based authentication for administrative access

---

## 3. System Features

### 3.1 Public Interface
**Home Page**
- Background video display
- Keyword-based search navigation

**About Page**
- Institutional information, mission, and vision

**Gallery Page**
- Categorized image display
- Lightbox image preview functionality

**Calendar Page**
- Dynamic event listing retrieved from the database

**Careers Page**
- Dynamic job listings with application links

**Student Admission Application**
- Parent and child information capture
- Proof-of-payment upload
- Database storage
- Email notification to administrator

**Job Application System**
- Upload of CV, identification, and certificates
- Database storage of application records
- Email notification with file attachments

### 3.2 Administrative Interface
The administrative panel includes:
- Secure login using PHP sessions
- Dashboard for system management
- Calendar event management (Create and Delete)
- Gallery image upload and removal
- Job posting management (Create and Delete)

> Access to administrative functionality is restricted to authenticated users.

---

## 4. Technology Stack
The system was developed using the following technologies:
- **PHP** (Core PHP)
- **MySQL** (Relational Database Management System)
- **HTML5**
- **CSS3**
- **JavaScript**
- **PHPMailer** (SMTP-based email handling)
- **Gmail SMTP server**

---

## 5. System Architecture
The application follows a client-server architecture:
- **Client-side:** HTML, CSS, JavaScript
- **Server-side:** PHP
- **Database Layer:** MySQL
- **Email Service:** PHPMailer integrated with Gmail SMTP

Dynamic content is retrieved from and stored in the database using SQL queries.

---

## 6. Database Configuration
The system requires a MySQL database named:

- preschool

The following tables are required:
- admin
- calendar
- gallery
- jobs
- applications
- job_applications

Database connection settings are configured in:  
- config.php

---

## 7. Installation and Setup

### Step 1: Install a Local Server Environment
Install and start:
- **XAMPP** or **WAMP**
- **Apache**
- **MySQL**

### Step 2: Deploy the Project
Place the project folder inside the server directory:  
- htdocs

### Step 3: Configure the Database
1. Create a database named preschool
2. Import the corresponding SQL file
3. Verify database credentials in config.php

### Step 4: Configure Email Credentials
In the following files:
- apply.php
- apply-jobs.php

Replace placeholder email credentials with valid Gmail SMTP credentials and an application-specific password. **Do not commit email passwords to version control.**

---

## 8. File Storage Directories
The application uses the following directories for file uploads:
- uploads/ – Gallery images and admission receipts
- job_uploads/ – CVs, identification documents, and certificates

> Ensure these directories have appropriate write permissions.

-----

## 9. Security Considerations
This system implements basic session-based authentication for administrative access. Recommended enhancements for production deployment:
- Password hashing using password_hash() and password_verify()
- Full implementation of prepared statements for all SQL queries
- Server-side input validation and sanitization
- CSRF protection mechanisms
- Secure file upload validation
- Proper logout functionality with session destruction

---

## 10. Future Enhancements
Potential improvements include:
- Parent and staff user accounts
- Role-based access control
- Enhanced user interface design
- Online payment integration
- Deployment to a live hosting environment
- Advanced security hardening

---

## 11. Intended Use
This project was developed for **educational and demonstration purposes**. It serves as a practical implementation of dynamic web development using PHP and MySQL.

