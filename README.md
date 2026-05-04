Final Project – PHP Framework Migration
 Overview

This project is a rebuilt version of an existing PHP web application, now implemented using a modern PHP framework instead of native PHP.

The goal is to apply structured development practices (MVC architecture) and improve scalability, maintainability, and organization.

 Objectives
Understand how PHP frameworks structure applications
Compare native PHP vs framework-based development
Implement clean MVC architecture
Use routing, controllers, models, and views
Build a maintainable and scalable web system
 Project Description

This system replicates the original application with the same core features:

Login & Logout
Session-based Authentication
Role-Based Access Control
Subject Management
Program Management
User Management
Change Password

 This is a full rebuild, not just copying old PHP files.

 Tech Stack
PHP Framework (e.g., Laravel / CodeIgniter / Symfony / CakePHP)
MySQL Database
HTML, CSS (Bootstrap optional)
 Database Structure

Database Name: school

Tables
subject
subject_id
code
title
unit
program
program_id
code
title
years
users
id
username
password
account_type
created_on
created_by
updated_on
updated_by
Rules
Username must be unique
Passwords must be hashed
Use prepared queries or ORM
Maintain audit fields properly
 Features
1. Authentication
Login & Logout
Session handling
Redirect unauthenticated users
2. Home Page
Displays username & role
Navigation based on role
Links:
Subjects
Programs
Users (Admin only)
Change Password
Logout
3. Subject Management
List subjects
Add subject
Edit subject

Validation:

Code: required
Title: required
Unit: numeric, > 0
4. Program Management
List programs
Add program
Edit program

Validation:

Code: required
Title: required
Years: numeric
5. User Management (Admin Only)
List users
Add user
Edit user

Validation:

Username: required & unique
Account type: valid
Password: hashed
Confirm password required
6. Change Password
Enter current password
Enter new password
Confirm password
Save hashed password
 Access Control
Guest
 No access to protected pages
 Redirect to login
Admin
Full access
 Manage users
Staff
 Manage subjects & programs
 Cannot access user management
Teacher / Student
 View only (subjects & programs)
 No edit access

 Access control must be enforced server-side.

 Framework Requirements

Your project must properly use:

Routing
Controllers
Models (or ORM)
Views/Templates
Session handling
Validation tools

 Do NOT just copy old PHP files into the framework.

 Development Steps
Create a new framework project
Configure database connection
Create models:
User
Subject
Program
Create controllers:
Auth
Home
Subjects
Programs
Users
Password
Create views:
Login
Dashboard
CRUD pages
Configure routes
Implement authentication & authorization
Test all features
 System Pages
Login Page
Home/Dashboard
Subject List / Add / Edit
Program List / Add / Edit
User List / Add / Edit
Change Password
 UI Expectations
Clean and readable forms
Clear navigation
Organized tables
Visible success/error messages
Consistent layout
 Presentation Details

Date: April 22, 2026
Time: 3:00 PM
Location: F612

 Presentation Requirements

You must:

Run the system successfully
Explain the framework used
Demonstrate:
Login/Logout
Subject Management
Program Management
User Management
Change Password
Explain:
Project structure
Routing
Controllers, Models, Views
 Important Notes
The system must be fully functional
Non-working projects may receive deductions
Prepare:
Database setup
Framework dependencies
Working environment

Summary

This project demonstrates how to transform a basic PHP application into a modern, framework-based system using proper architecture and best practices.
