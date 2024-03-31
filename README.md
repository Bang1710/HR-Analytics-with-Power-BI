# 📝 HR Analytics with Power BI
## I. Description
In this Power BI case study, you will be exploring a dataset for a fictitious software company called Atlas Labs. This course focuses on helping you import, analyze and visualize Human Resources data in Power BI. Building on your existing knowledge of the platform, you'll learn how to effectively work with Power BI using example data.

You’ll carry out exploratory data analysis and will use DAX to help build powerful visualizations. You’ll finish your analysis by diving deeper into attrition and what factors impact attrition. This analysis will help the organization determine what action they will need to take to retain more employees.

We’ll finalize the case study by making design changes to our report that provides a clean, branded design.

## II. Dataset
### > Table ```Performance```

| Field                               | Description                                                | Datatype |
| ----------------------------------- | ---------------------------------------------------------- | -------- |
| PerformanceID                       | A unique ID that identifies an individual performance review | text     |
| EmployeeID                          | A unique ID that identifies an employee, connects to DimEmployee | text     |
| ReviewDate                          | Date an employee’s review took place                         | date     |
| EnvironmentSatisfaction             | Rating for employees' satisfaction with their environment, connects to DimSatisfiedLevel | number   |
| JobSatisfaction                     | Rating for employees' satisfaction with their job role, connects to DimSatisfiedLevel | number   |
| RelationshipSatisfaction            | Rating for employees' satisfaction with their relationships at work, connects to DimSatisfiedLevel | number   |
| WorkLifeBalance                     | Rating for employees' satisfaction with their work-life balance, connects to DimSatisfiedLevel | number   |
| SelfRating                          | Rating for employees' performance based on their own view, connects to DimRatingLevel | number   |
| ManagerRating                       | Rating for employees' performance based on their manager’s view, connects to DimRatingLevel | number   |
| TrainingOpportunitiesWithinYear     | Number of training opportunities offered in the last 12 months | number   |
| TrainingOpportunitiesTaken           | Number of training opportunities taken                       | number   |

### > Table ```Employee```

| Field                   | Description                                                | Datatype |
| ----------------------- | ---------------------------------------------------------- | -------- |
| EmployeeID              | A unique ID that identifies an employee                     | text     |
| FirstName               | First name of an employee                                   | text     |
| LastName                | Last name of an employee                                    | text     |
| Gender                  | Self-defined employee gender identity                       | text     |
| Age                     | Current age of an employee                                  | number   |
| BusinessTravel          | Frequency of business travel: Frequent Traveller, Some Travel, and No Travel | text     |
| Department              | Department an employee works in: Technology, HR, and Sales  | text     |
| DistanceFromHome        | Kilometer distance between an employee’s home and their office | number   |
| State                   | State where the employee lives                              | text     |
| Ethnicity               | Self-defined employee ethnicity                             | text     |
| Education               | Education level for employees, connects to DimEducationLevel | number   |
| EducationField          | Employee field of study                                     | text     |
| Job Role                | Current/latest employee job role                             | text     |
| MaritalStatus           | Current/latest employee marital status                      | text     |
| Salary                  | Current/latest employee salary                               | number   |
| StockOptionLevel        | The banding level for stock options that the employee has    | number   |
| Overtime                | "Yes" or "No" to indicate whether an employee is expected to work overtime in their role | text     |
| HireDate                | Date the employee joined the company                         | date     |
| Attrition               | "Yes" or "No" to indicate whether an employee has left the organization | text     |
| YearsAtCompany          | Number of years since the employee joined the organization   | number   |
| YearsInMostRecentRole   | Number of years the employee has been in their most recent role | number   |
| YearsSinceLastPromotion | Number of years since the employee last got promoted         | number   |
| YearsWithCurrManager    | Number of years the employee has been with their current manager | number   |

### > Table ```Satisfied Level```

| Field                               | Description                                                | Datatype |
| ----------------------------------- | ---------------------------------------------------------- | -------- |
| SatisfactionID                      | A unique ID that connects to EnvironmentSatisfaction, JobSatisfaction, RelationshipSatisfaction, and Work-Life Balance in FactPerformanceRating | text     |
| SatisfactionLevel                   | Provides meaning to the satisfaction level: Very Satisfied, Satisfied, Neutral, Dissatisfied, and Very Dissatisfied | number   |
| SatisfactionText                    | Text representation of the satisfaction level               | text     |

### > Table ```Rating Level```

| Field                               | Description                                                | Datatype |
| ----------------------------------- | ---------------------------------------------------------- | -------- |
| RatingID                            | A unique ID that connects to SelfRating and ManagerRating in FactPerformanceRating | text     |
| RatingLevel                         | Provides meaning to the rating level: Above and Beyond, Exceeds Expectation, Meets Expectation, Needs Improvement, and Unacceptable | number   |
| RatingText                          | Text representation of the rating level                      | text     |

### > Table ```Education Level```

| Field                               | Description                                                | Datatype |
| ----------------------------------- | ---------------------------------------------------------- | -------- |
| EducationLevelID                    | A unique ID that connects to Education in DimEmployee      | text     |
| EducationLevel                      | Provides meaning to the education level: Doctorate, Masters, Bachelors, High School, and No Formal Qualifications | number   |
| EducationText                       | Text representation of the education level                 | text     |



## III. Goals
+ Primary goal: Monitor key HR metrics on employees
+ Secondary goal: Understand what factors impact attrition

## IV. Key insights uncovered
+ Atlas Labs has employed over 1,470 people.
+ Atlas Labs currently employs over 1,200 people.
+ The largest department by far is Technology.
+ The attrition rate for employees leaving the organization is 16%
+ Majority of employees are between 20-29 years old.
+ Currently, Atlas Labs employ 2.7% more women than men.
+ Non-binary make up 8.5% of total employees.
+ White have the highest average salary
+ 'Mixed or multiple ethnic groups' have one of the lowest average salaries.

## V. Entity Relationship Diagram
![ERD](https://github.com/Bang1710/HR-Analytics-with-Power-BI/blob/main/ERD/ERD.png)
## VI. Dashboard
![Dashboard part 01](https://github.com/Bang1710/HR-Analytics-with-Power-BI/blob/main/Dashboard/DB1.png)
![Dashboard part 02](https://github.com/Bang1710/HR-Analytics-with-Power-BI/blob/main/Dashboard/DB2.png)
![Dashboard part 03](https://github.com/Bang1710/HR-Analytics-with-Power-BI/blob/main/Dashboard/DB3.png)
![Dashboard part 04](https://github.com/Bang1710/HR-Analytics-with-Power-BI/blob/main/Dashboard/DB4.png)
