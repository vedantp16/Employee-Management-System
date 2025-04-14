# Employee Management System

## Overview
The **Employee Management System** is a console-based Java application designed to manage employee records. It allows users to perform CRUD (Create, Read, Update, Delete) operations and stores employee data in a MySQL database. This project demonstrates fundamental Java programming concepts, JDBC integration, and database management.

## Features
- Add a new employee to the system.
- View all employees.
- Update employee details by ID.
- Delete an employee record by ID.
- Store and retrieve data securely using MySQL.

## Technologies Used
- **Programming Language**: Java
- **Database**: MySQL
- **JDBC**: Java Database Connectivity for database integration

## Prerequisites
1. **Java Development Kit (JDK)**: Ensure JDK 8 or later is installed.
2. **MySQL Database**: A running instance of MySQL with a database named `employee_db`.
3. **IDE (Optional)**: IntelliJ IDEA, Eclipse, or any preferred Java IDE.

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/EmployeeManagementSystem.git
   ```
2. Navigate to the project directory and ensure all files are present.
3. Import the project into your IDE (optional).

## Database Setup
1. Create the database and table in MySQL:
   ```sql
   CREATE DATABASE employee_db;

   CREATE TABLE employees (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(50),
       department VARCHAR(50),
       salary DOUBLE
   );
   ```
2. Update the `DBConnection.java` file with your MySQL credentials:
   ```java
   private static final String URL = "jdbc:mysql://localhost:3306/employee_db";
   private static final String USER = "your_username";
   private static final String PASSWORD = "your_password";
   ```

## How to Run
1. Compile the Java files:
   ```bash
   javac *.java
   ```
2. Run the `Main` class to start the application:
   ```bash
   java Main
   ```

## Usage
- **Add Employee**: Input name, department, and salary details to add a new employee.
- **View Employees**: Displays a list of all employees in the database.
- **Update Employee**: Update an employee's details by entering their ID.
- **Delete Employee**: Remove an employee record by entering their ID.

## License
This project is licensed under the MIT License. Feel free to use, modify, and distribute it as needed.

---
Author: Vedant Pampattiwar
Contact:vedantpampattiwar2003@gmail.com
