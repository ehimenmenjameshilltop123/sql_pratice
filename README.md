# 🧑‍💼 Employee SQL Practice with PostgreSQL & pgAdmin

This project contains SQL queries and exercises I completed while practicing data analysis with PostgreSQL and pgAdmin.

## 📋 Project Summary

- Created an `employees` table with sample data
- Imported data from a CSV file into PostgreSQL using pgAdmin
- Wrote SQL queries to analyze and filter employee records

## 🛠️ Tools Used

- PostgreSQL
- pgAdmin
- SQL
- Google Sheets / Notepad (for CSV prep)

## 📂 Dataset Fields

| Column Name | Description          |
|-------------|----------------------|
| id          | Employee ID (integer) |
| name        | Full Name (text)      |
| department  | Department Name (text) |
| salary      | Salary in NGN/USD (integer) |
| hire_date   | Date Hired (date)     |

## 💻 Sample SQL Queries

```sql
-- View all employees
SELECT * FROM employees;

-- Average salary per department
SELECT department, AVG(salary) AS avg_salary
FROM employees
GROUP BY department;

-- Employees hired before 2020
SELECT * FROM employees
WHERE hire_date < '2020-01-01';

