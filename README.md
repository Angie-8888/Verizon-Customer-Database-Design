Verizon Customer Management System
Description
This is a command-line Customer Management System for Verizon, created using Python and SQLite3. It supports core functionalities like adding/removing customers, managing services and equipment, tracking payments, and updating billing details. The project follows a simplified Model-View-Controller (MVC) structure to separate database logic from user interface operations.

File Structure
main.py – Handles user interaction, menus, and program flow.

database.py – Contains all database queries and logic.

Project2_database_design_angielee.docx – Explains the normalized relational database schema and design choices.

Project2_Software_Design_AngieLee.docx – Summarizes the software design and user flow architecture.

Features
✅ Add and remove customers
✅ Search for customers
✅ Track late payments
✅ Add/remove services and equipment
✅ Update costs for services/equipment
✅ Change billing amounts
✅ View all customer data

Database Schema
customers: customer_id (PK), customer_name, customer_number

locations: location_id (PK), customer_id (FK), address

services: service_id (PK), location_id (FK), service_type, cost_of_service

equipments: equipment_id (PK), location_id (FK), equipment_type, cost_of_equipment

payments: payment_id (PK), customer_id (FK), amount_due, last_payment_date, payment_status

This structure ensures data integrity and supports customers with multiple service locations.

How to Run
Make sure Python 3 is installed.

Open terminal or command prompt.

Run the program:

bash
Copy
Edit
python main.py
Author
Angie Lee

