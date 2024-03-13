# HR-Data-Analysis-using-SQL

### Introduction:

In the modern business landscape, Human Resources (HR) departments play a crucial role in managing the workforce of organizations. They handle various tasks such as recruitment, employee relations, training, and performance evaluation. Utilizing data effectively can provide valuable insights into employee dynamics, productivity, and organizational efficiency. This project aims to leverage Microsoft SQL Server to analyze HR data and derive meaningful conclusions to support strategic decision-making.
I have created a new database named "HR" within Microsoft SQL Server to manage and analyze employee data. I imported the provided HR data file into this database and utilize SQL queries to answer various questions about the workforce.

### Objective:

The objective of this project is to utilize SQL queries to extract valuable insights from HR data stored in a database. By addressing a series of analytical questions, we aim to understand various aspects of employee performance, satisfaction, attrition, and demographics. These insights will assist HR managers and organizational leaders in making informed decisions related to workforce management, employee engagement, and retention strategies.

### About the Dataset:

The dataset contains comprehensive information about employees within an organization, covering various aspects such as demographics, job attributes, performance indicators, and attrition status. This dataset is essential for HR professionals and organizational leaders to understand and manage their workforce effectively.

##### Here's a breakdown of the potential attributes based on the column names:

-  Employee Information: I found details like Employee Status: The data includes columns indicating whether employees are currently employed (CF_attrition Empolyee), their attrition status (Attrition which is the same as Column1), and potentially a reason for leaving (CF_attrition label for those who left).employee numbers, genders, job roles, marital statuses, and ages.
-  Work Details: This data includes information about departments, job levels, overtime status, training participation, and standard working hours.
-  Compensation: The data also contains details on employee compensation, including hourly rates, monthly income, monthly rates, and recent salary hike percentages.
-  Performance: There are columns related to employee performance, such as performance ratings and job satisfaction levels.
-  Work-Life Balance: The data provides insights into work-life balance with columns
-  Job Experience: I can analyze employee experience using details like total working years, years at the company, years in current roles, and years with current managers.
-  Company Information: The data includes information about departments, employee education fields, and business travel categories.
-  Other: There are additional details like the number of companies previously worked for by each employee, stock option levels, and relationship satisfaction levels.
- Employee Status: The data includes columns indicating whether employees are currently employed (CF_attrition Empolyee), their attrition status (Attrition which is the same as Column1), and potentially a reason for leaving (CF_attrition label for those who left).

 ###  Project Steps:

 - Database Creation: I have created an HR database within Microsoft SQL Server.
 - Data Import: I will import the HR data file into the newly created HR database.
 - Data Analysis: I will execute a series of SQL queries to answer specific questions about the employees in the organization. These queries will cover:

The tool used was Microsoft SQL Server.

Data was imported as a flat file (a CSV file) into Microsoft SQL Server

### Find the top 5 departments with the highest average monthly income
SELECT TOP 5 [Department], AVG([Monthly_Income]) AS Average_monthly_income
FROM [dbo].[HR Data CSV]
GROUP BY [Department]
ORDER BY AVERAGE_MONTHLY_INCOME DESC;


