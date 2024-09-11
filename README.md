## Steps Taken
1. **Data Loading**: Imported CSV files into Power BI for `departments`, `employees`, and `dept_emp`.
2. **Data Cleaning**: Checked for and handled missing or incorrect data entries.
3. **Data Modeling**: Established relationships between tables in Power BI to ensure proper data connectivity.
## SQL Queries
- Query to find the average salary by department:
  ```sql
  SELECT d.dept_name, AVG(s.salary) AS avg_salary
  FROM departments d
  JOIN dept_emp de ON d.dept_no = de.dept_no
  JOIN salaries s ON de.emp_no = s.emp_no
  GROUP BY d.dept_name;
## Visualizations
1. **Total Number of Employees**: A card visual displaying the total count of employees.
2. **Average Salary by Department**: A bar chart showing average salaries across departments.
3. **Employee Distribution by Department**: A pie chart illustrating the employee count distribution across departments.
4. **Salary Trend Over Time**: A line chart depicting how salaries have changed over the years.
5. **Gender Distribution by Department**: A stacked bar chart showing the gender breakdown within each department.
## Instructions for Use
1. **Power BI**: Open the Power BI file and ensure all data connections are refreshed.
2. **SQL**: Use the included SQL scripts to run analyses on the database.
