# Final Lab Task 4

## Task Description:

- This task involved working with a single database containing two tables: EmployeeSalaries and EmployeeData. I performed a series of SELECT statements to extract and manipulate employee information.

## Step 1: Query Statements

### Objective: Perform queries on the EmployeeSalaries table.

- Problem 1: Consider a table named EmployeeSalaries that stores information about the salaries of employees.
- The table has the following fields:
  
```sql
CREATE DATABASE payroll;
USE payroll;

CREATE TABLE EmployeeSalaries (
    employee_id INT AUTO_INCREMENT PRIMARY KEY,
    employee_name VARCHAR(100),
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE
);
```
<img src="Images/emp_sal_tbl.png" width="600" height="300">

### Retrieve the employee_name and salary and arrange from the highest salary to lowest.

```sql
SELECT employee_name, salary FROM EmployeeSalaries ORDER BY salary DESC;
```
<img src="Images/emp_name_salary.png" width="400" height="150">

### Retrieve the department names along with the average salary for each department.

```sql
SELECT department, AVG(salary) AS average_salary FROM EmployeeSalaries GROUP BY department;
```
<img src="Images/depart_avg_sal.png" width="300" height="300">

## Step 2: Key Schema Statements

**Objective:** Perform queries on the `EmployeeData` table.

- Problem 2: Create a database named employeeDB and copy and paste the initial query.
- The `EmployeeData` table stores information about employees with the following schema:
  
```sql
CREATE DATABASE employeeDB;
USE employeeDB;

CREATE TABLE EmployeeData (
    employee_id INT AUTO_INCREMENT PRIMARY KEY,
    full_name VARCHAR(100),
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE,
    manager_id INT
);
```
<img src="Images/emp_data_tbl.png" width="600" height="500">

### Retrieve the employees along with their full names and salaries with highest paying employee to the lowest.

```sql
SELECT full_name, salary FROM EmployeeData ORDER BY salary DESC;
```
![image](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Final%20Lab%20Task%204/Images/select1.png)

### Retrieve the average salary from EmployeeData table, where the average salary exceeds $70,000.

```sql
SELECT AVG(salary) AS average_salary FROM EmployeeData HAVING average_salary > 70000;
```
![image](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Final%20Lab%20Task%204/Images/select2.png)

### Retrieve the full names of employees who earn a salary greater than $100,000.
```sql
SELECT full_name FROM EmployeeData WHERE salary > 100000;
```
![image](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Final%20Lab%20Task%204/Images/select3.png)

### Retrieve the number of employees from the EmployeeData table.

```sql
SELECT COUNT(employee_id) AS number_of_employees FROM EmployeeData;
```
![image](https://github.com/silerio06/EDM-Portfolio-Dave/blob/main/Final%20Lab%20Task%204/Images/select4.png)
