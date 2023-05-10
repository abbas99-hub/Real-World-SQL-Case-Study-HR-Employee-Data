# Real-World-SQL-Case-Study-HR-Employee-Data
## Project Overview
This project aims to perform exploratory data analysis (EDA) on HR Analytics data using SQL and Python. The HR Analytics dataset contains employee information such as age, education level, job role, salary, etc., and the main objective of this project is to gain insights into employee attrition and identify the key factors that affect employee retention.
The HR Analytics Employee Attrition & Performance contains 1470 rows and 35 columns. The data source is located at Kaggle.

## Dataset Description
The HR Analytics dataset contains the following columns:

* Age: Employee's age
* Attrition: Employee's attrition status (Yes/No)
* BusinessTravel: Frequency of employee's business travel
* DailyRate: Daily rate of pay
* Department: Employee's department
* DistanceFromHome: Distance between employee's home and workplace
* Education: Employee's level of education
* EducationField: Field of study
* EmployeeCount: Number of employees
* EmployeeNumber: Employee identification number
* EnvironmentSatisfaction: Employee's satisfaction with the work environment
* Gender: Employee's gender
* HourlyRate: Hourly rate of pay
* JobInvolvement: Employee's level of job involvement
* JobLevel: Employee's job level
* JobRole: Employee's job role
* JobSatisfaction: Employee's job satisfaction
* MaritalStatus: Employee's marital status
* MonthlyIncome: Employee's monthly income
* MonthlyRate: Monthly rate of pay
* NumCompaniesWorked: Number of companies the employee has worked for
* Over18: Whether the employee is over 18 years old
* OverTime: Whether the employee works overtime
* PercentSalaryHike: Percentage of salary hike for the employee
* PerformanceRating: Employee's performance rating
* RelationshipSatisfaction: Employee's satisfaction with work relationships
* StandardHours: Standard number of working hours
* StockOptionLevel: Employee's stock option level
* TotalWorkingYears: Employee's total years of work experience
* TrainingTimesLastYear: Number of training times the employee had last year
* WorkLifeBalance: Employee's work-life balance
* YearsAtCompany: Number of years the employee has been with the company
* YearsInCurrentRole: Number of years the employee has been in the current role
* YearsSinceLastPromotion: Number of years since the employee's last promotion
* YearsWithCurrManager: Number of years the employee has been with the current manager

## SQL Queries
Use SQL queries to extract relevant data from the database.
Clean and preprocess the data as necessary to ensure that it is suitable for analysis.
Use SQL queries to perform various types of analysis on the data, such as calculating attrition rates by department or identifying factors that are correlated with higher levels of employee satisfaction.


## Project Steps
1. Data Preparation and Cleaning
The first step of the project is to prepare and clean the dataset for analysis. This involves removing duplicates, handling missing values, and transforming the data into a usable format.
I used Microsoft Excel to replace the numeric code used to represent some of the variables.

Step 1: In the Education column, I replaced

1 with “Below College”
2 with “College”
3 with “Bachelor”
4 with “Master”
5 with “Doctor”

Step 2: In the EnvironmentSatisfaction, I replaced:

1 with “Low”
2 with “Medium”
3 with “Satisfied”
4 with “Highly-Satisfied”

Step 3: In the JobInvolvement, I replaced:

1 with “Low”
2 with “Medium”
3 with “Involved”
4 with “Highly-Involved”

Step 4: In the JobSatisfaction, I replaced:

1 with “Low”
2 with “Medium”
3 with “Satisfied”
4 with “Highly-Satisfied”

Step 5: In the PerformanceRating, I replaced:

3 with “Satisfied”
4 with “Highly-Satisfied”

Step 6: In the RelationshipSatisfaction, I replaced:

1 with “Low”
2 with “Medium”
3 with “Satisfied”
4 with “Highly-Satisfied”

Step 7: In the WorkLifeBalance, I replaced:

1 with “Low”
2 with “Mid”
3 with “Good”
4 with “Very-Good”

2. Exploratory Data Analysis
Analyze the distribution of the variables in the dataset and identify any outliers or missing values that need to be addressed.
Create visualizations, such as histograms and box plots, to better understand the distribution of the variables.
Look for any patterns or trends in the data, such as correlations between variables, that could provide insights into the factors that affect employee attrition.

3. Data Visualization
Data visualization is an essential part of EDA. It helps to identify patterns and trends in the data that may not be apparent in summary statistics. In this step, we use Python's visualization libraries such as Matplotlib and Plotly to create visualizations such as bar graphs, pie charts, and scatter plots.

4. Insights and Recommendations

> - The dataset does not feature any missing or erroneous data values, and all features are of the correct data type. <br>
- The strongest positive correlations with the target features are: **Performance Rating**, **Monthly Rate**, **Num Companies Worked**, **Distance From Home**. 
- The strongest negative correlations with the target features are: **Total Working Years**, **Job Level**, **Years In Current Role**, and **Monthly Income**.
- The dataset is **imbalanced** with the majoriy of observations describing Currently Active Employees. <br>
- Several features (ie columns) are redundant for our analysis, namely: EmployeeCount, EmployeeNumber, StandardHours, and Over18. <br>

Other observations include: <br>
> - Single employees show the largest proportion of leavers, compared to Married and Divorced counterparts. <br>
- About 10% of leavers left when they reach their 2-year anniversary at the company. <br>
- Loyal employees with higher salaries and more responsbilities show lower proportion of leavers compared to their counterparts. <br>
- People who live further away from their work show higher proportion of leavers compared to their counterparts.<br>
- People who travel frequently show higher proportion of leavers compared to their counterparts.<br>
- People who have to work overtime show higher proportion of leavers compared to their counterparts.<br>
- Employee who work as Sales Representatives show a significant percentage of Leavers in the submitted dataset.<br>
- Employees that have already worked at several companies previously (already "bounced" between workplaces) show higher proportion of leavers compared to their counterparts.<br>
