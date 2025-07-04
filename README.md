# DSA-Project-documentation
## Project Title: Palmora Group HR Analysis

### Dataset description:
The Palmoria Group, a manufacturing company based in Nigeria, is embroiled in issues
bordering on gender inequality in its 3 regions. Cases like this can only spiral downwards,
revealing other issues like the gender pay gap, amongst other possible issues.
The CEO of Palmoria, Mr Ayodeji Chukwuma, is keen to address these issues before they
get out of hand. The CHRO, Mr Yunus Shofoluwe, has been assigned the task to identify
key areas within the business that could give rise to issues and address them immediately.
Mr Shofoluwe decided to recruit you as an HR Analytics expert to analyse the company’s
HR data and come up with recommendations for management’s attention. “Now, the
future of gender equality in Palmoria lies in your hands” – the exact words of Mr
Shofoluwe before he handed the data to you.
- Given file format: Excel workbook _xlsx & csv files

## Introduction
This report presents the findings of a data-driven analysis aimed at investigating gender inequality and the pay gap within Palmoria Group company. By analyzing employee demographic and salary data, the objective was to assess the extent of pay disparity between male and female employees, identify underlying patterns, and recommend strategies for promoting pay equity and workplace inclusivity

### Step-by-step Approach
#### Step 1: Extract, Transform and Load (ETL)
- Removes employees that are no long working with the company and departments that are indicated as NULL
- Assigned a generic gender to employees that are refused to disclose their gender
- Added columns by using conditional column: Rating_sort, Employee_Count
- Measure was used for quite number of calculations such:
- Average Rating by Gender = AVERAGE('Employee'[Rating])
  - Rating Count by Gender = COUNT('Employee'[Rating])
  - Average Salary by Gender = AVERAGE('Employee'[Salary])
  - Salary Count by Department and Region = COUNT('Employee'[Salary])
  - Employees Below Minimum Salary = COUNTX(FILTER('Employee', 'Employee'[Salary] < 90000), 'Employee'[Salary])
  - Bonus Amount = IF('Employee'[Rating] > 3, 'Employee'[Salary] * 0.1, 0)
  - Total Amount to be Paid = 'Employee'[Salary] + 'Bonus Amount
#### Step 2: Visualization
- Creating interactive dashboards with filters and slicers
- Designing pie charts, clustered column charts, line charts, bar graphs, and tables

### Insights and Interpretation
- In Kaduna region there is significant difference in the number of employees(male and female gender) that are working the company and this could be as a result of gender discrimination, occupational segregation, lack of female education 
- Kaduna region has the largest number of employees in the company
- In Abuja region there is almost the same number of male and female employees which could be as a result of Abuja being the capital city of Nigeria and it is expected to practice equality and equity, Abuja region accommodates all regions and respect both male and female gender
- In Lagos region there is a slight gender difference in the of number of employees and this could be as a result of differences in work experience and education attainment  
- Female employees are rated very good more than male employees and this could be as a result of female exceptionality in doing things
- Employees that are receiving below minimum salary in the company are more in Kaduna region, follow by Abuja region, then Lagos and this could be as a result of unemployment in the land
- Pay gap: male employees basic salary are higher than female employees and this could be as a result of job role/responsibilities, years of experience, certificate acquired e.t.c

### Recommendations
- Recruit and promote female employee into leadership roles to ensure diverse perspectives in decision-making and policy development
- Palmora Group should focus on transparent pay practices, fair hiring and promotion processes, and supportive policies for all employees. 
-	Regularly analyze salary data to identify and address any gender-based pay disparities. 
- Encourage open dialogue about gender equality and the pay gap, creating a safe space for employees to raise concerns and contribute to solutions
- Train employees and managers on unconscious bias and implement strategies to mitigate its effects in hiring and promotion decisions. 

### Conclusion
Analyzing gender inequality and gender pay gap issues in Palmora Group company will mitigate gender inequality and gender pay gap and create more equitable and inclusive work environment for all the employees






