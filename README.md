# sql-challenge

This is a research project on employees of the corporation from the 1980s and 1990s. All that remain of the database of employees from that period are six CSV files.  In this assignment I designed the tables to hold data in the CSVs, imported the CSVs into a SQL database, and answered questions about the data. In other words, you will perform:

Data Engineering
Inspected csv files looking for column names, potential or absence of primary keys and identified data types. Note: TIMESTAMP was used as the data type for the date fields. Using [http://www.quickdatabasediagrams.com an ERD was drawn up. An entity Relationship Diagram (ERD) is a snapshot of data structures. An ERD shows entities (tables) and relationships (primary and foreign keys) between tables within that database. Attributes (data types) are also shown. The code to create the tables was exported and modified to use the SERIAL method for creating auto incrementing primary keys in the Postgres SQL dialect.

Tables were created in the order departments, titles, employees, dept_emp, dept_managers, salaries to ensure any new primary keys were created before being referenced as a foreign key in another table – leading to a run error. 3 new primary keys were created for dept_emp, dept_managers, salaries in order to comply with the first normal form (all rows in a table must be unique). A .png picture of the ERD and a .sql file of the table creation code is uploaded as part of this submission.

The data was uploaded (in the same order as table creation) from the .csv files and checked for accuracy.
 
Data Analysis
SQL queries were created and run for the following questions:
1. List the following details of each employee: employee number, last name, first name, sex, and salary.
2. List first name, last name, and hire date for employees who were hired in 1986.
3. List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.
4. List the department of each employee with the following information: employee number, last name, first name, and department name.
5. List first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."
6. List all employees in the Sales department, including their employee number, last name, first name, and department name.
7. List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.

The queries are saved in the accompanying Data_Analysis.sql file.

John Russell
May 22nd, 2021
