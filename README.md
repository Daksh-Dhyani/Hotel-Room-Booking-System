# Hotel-Room-Booking-System
# 🏨 Hotel Room Booking System | DBMS Mini Project

## 📌 Project Overview

The **Hotel Room Booking System** is a database management system developed using **MySQL 8.0** to manage hotel operations efficiently. It provides a structured way to store and manage guest information, room categories, room availability, bookings, payments, and cancellations.

The project demonstrates how a relational database can replace manual record-keeping, reduce data redundancy, maintain data integrity, and simplify hotel booking operations.

## 🎯 Objectives

- Design a normalized relational database for hotel management.
- Maintain guest, room, booking, and payment records.
- Calculate booking amounts automatically based on room prices and the number of nights.
- Check room availability for specific dates.
- Prevent overlapping confirmed bookings for the same room.
- Track payments and outstanding balances.
- Generate booking summaries and revenue reports.
- Apply database constraints to maintain accurate and consistent records.

## 🛠️ Technologies Used

- **Database:** MySQL 8.0
- **Query Language:** SQL
- **Database Tool:** MySQL Workbench / MySQL Command Line Client
- **Database Design:** Entity-Relationship (ER) Model
- **Normalization:** Up to Third Normal Form (3NF)

## 📂 Project Modules

### 1. Guest Management
Stores guest details, including full name, phone number, email, city, and identity proof.

### 2. Room Type Management
Manages room categories such as Standard, Deluxe, and Suite, including their prices per night and capacity.

### 3. Room Management
Maintains room numbers, floor details, room categories, and room status, including Available, Booked, and Maintenance.

### 4. Booking Management
Records check-in and check-out dates, booking status, and total booking amounts. It also supports booking cancellations and date-overlap checks.

### 5. Payment Management
Records payments made through Cash, Card, or UPI and helps identify outstanding balances.

### 6. Reports and Queries
Generates useful information, including complete booking details, available rooms, revenue by room type, booking summaries, and pending payments.

## 🗄️ Database Structure

The project contains five main relational tables:

| Table | Purpose |
|---|---|
| `guests` | Stores guest information |
| `room_types` | Stores room categories, prices, and capacity |
| `rooms` | Stores individual room information |
| `bookings` | Stores reservation details and booking amounts |
| `payments` | Stores payment transactions |

### 🔗 Entity Relationships

- One room type can have multiple rooms.
- One guest can make multiple bookings.
- One room can be associated with multiple bookings over time.
- One booking can have multiple payment records.

## ⚙️ Key Features

- **Automated Bill Calculation:** Calculates the booking amount using the room's nightly price and the number of nights.
- **Double-Booking Prevention:** Uses a stored procedure to reject bookings that overlap with existing confirmed reservations.
- **Room Availability Search:** Identifies rooms available for a specified date range while excluding rooms under maintenance.
- **Payment Tracking:** Calculates the amount paid and the remaining balance for confirmed bookings.
- **Revenue Analysis:** Summarizes booking counts and revenue by room category.
- **Booking Summary View:** Provides consolidated information about confirmed bookings.
- **Booking Cancellation:** Updates the status of a reservation to Cancelled.
- **Data Integrity:** Uses primary keys, foreign keys, UNIQUE, NOT NULL, and CHECK constraints.

## 🧠 DBMS Concepts Demonstrated

This project applies the following database concepts:

- Relational Database Design
- Entity-Relationship (ER) Modelling
- Database Normalization up to 3NF
- Primary and Foreign Keys
- Integrity Constraints
- SQL DDL, DML, and DQL
- INNER JOIN and LEFT JOIN
- Aggregate Functions
- GROUP BY and HAVING
- Subqueries
- Database Views
- Triggers
- Stored Procedures
- Date Handling and Booking Validation

## 📊 Expected Outcomes

The system demonstrates how hotel booking data can be managed in a structured and reliable manner. It supports automatic bill calculation, room availability checks, reservation validation, payment tracking, and reporting.

The sample database also demonstrates successful booking operations, rejection of overlapping reservations, identification of pending payments, and validation of incorrect check-in and check-out dates.

## 🚀 Future Enhancements

The system can be extended with the following features:

- Web-based or desktop graphical user interface.
- User authentication and role-based access for hotel staff.
- Online room reservations.
- Payment gateway integration.
- Automatic room status updates during check-in and check-out.
- Room service and additional billing modules.
- Advanced dashboards for occupancy and revenue analysis.
- Email or SMS booking confirmations.

## 🎓 Learning Outcomes

Through this project, we gained practical experience in designing relational databases, applying normalization, maintaining referential integrity, writing SQL queries, creating triggers and stored procedures, and generating meaningful reports from structured data.

The project demonstrates the practical application of **Database Management System (DBMS)** concepts in a real-world hotel management scenario.

## 👨‍💻 Project Information

- **Project Name:** Hotel Room Booking System
- **Project Type:** DBMS Mini Project
- **Domain:** Hotel Management and Database Systems
- **Database:** MySQL 8.0
- **Purpose:** Academic project demonstrating relational database design and SQL operations

## 📄 Conclusion

The Hotel Room Booking System demonstrates how MySQL can be used to organize hotel data, simplify booking operations, automate billing calculations, prevent overlapping confirmed reservations, and maintain payment records.

It provides a practical foundation for developing a complete hotel management application with additional user-interface and online booking features.

---

⭐ **If you find this project useful, consider giving the repository a star!**
