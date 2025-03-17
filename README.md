# Employee Management System

## 📌 Overview

A simple Employee Management System using **Python** and **MySQL**. It helps you:

- Add employees
- Remove employees
- Promote employees
- Display all employees

The system automatically creates necessary tables if they don't exist.

---

## ⚙️ Setup Instructions

### **1️⃣ Install MySQL**
Make sure MySQL is installed and running. If not, download it from:
- [Download MySQL](https://dev.mysql.com/downloads/)

### **2️⃣ Install Python MySQL Connector**
Run this command:
```sh
pip install mysql-connector-python
```

### **3️⃣ Set Up the Database**
Open MySQL and create a database:
```sql
CREATE DATABASE emp;
USE emp;
```

### **4️⃣ Run the Script**
Execute:
```sh
python3 main.py
```
This will create the `employees` table if it doesn’t exist.

---

## 🎯 Features

✅ **Add Employees**: Store employee details (ID, Name, Position, Salary).  
✅ **Remove Employees**: Delete an employee record.  
✅ **Promote Employees**: Increase an employee’s salary.  
✅ **Display Employees**: View all employees with details.  
✅ **Data Stored in MySQL**

---

## 🚀 How to Use

Run the script, and a menu will appear:
```
Welcome to Employee Management Record
Press:
1 to Add Employee
2 to Remove Employee
3 to Promote Employee
4 to Display Employees
5 to Exit
```
Enter a number to perform an action.

---

## 🛠️ Database Structure

The `employees` table is structured as:
```sql
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    position VARCHAR(255) NOT NULL,
    salary FLOAT NOT NULL
);
