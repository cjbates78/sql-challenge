# sql-challenge
Before You Begin
1. Create a new repository for this project called sql-challenge. Do not add this assignment to an existing repository.

2. Clone the new repository to your computer.

3. Inside your local Git repository, create a directory for this Challenge. Use a folder name that corresponds to the Challenge, such as EmployeeSQL.

4. Note that you’ll add your files to this folder and push the changes to GitHub.

#Files
Download the following files to help you get started:

Instructions
This Challenge is divided into three parts: data modeling, data engineering, and data analysis.

Data Modeling
Inspect the CSV files, and then sketch an Entity Relationship Diagram of the tables. To create the sketch, feel free to use a tool like QuickDBDLinks to an external site..

Data Engineering
1. Use the provided information to create a table schema for each of the six CSV files. Be sure to do the following:

    Remember to specify the data types, primary keys, foreign keys, and other constraints.

    For the primary keys, verify that the column is unique. Otherwise, create a composite keyLinks to an external site., which takes two primary keys to uniquely identify a row.

    Be sure to create the tables in the correct order to handle the foreign keys.

2. Import each CSV file into its corresponding SQL table.

Data Analysis
1. List the employee number, last name, first name, sex, and salary of each employee.

2. List the first name, last name, and hire date for the employees who were hired in 1986.

3. List the manager of each department along with their department number, department name, employee number, last name, and first name.

4. List the department number for each employee along with that employee’s employee number, last name, first name, and department name.

5. List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.

6. List each employee in the Sales department, including their employee number, last name, and first name.

7. List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.

8. List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

Created and Exported SQL schema file nad PNG from QuickDBD: https://www.quickdatabasediagrams.com/

Data would only import with VARCHAR fields, INT would not work 

Department data was imported with double quote, so I worked with Ask BCS and was able to run the following to fix it
UPDATE departments
SET dept_name= REPLACE(dept_name,'"','') 
and UPDATE departments
SET dept_name= REPLACE(dept_no,'"','')



