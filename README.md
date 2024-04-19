# Human Resources Analysis Report
![](https://github.com/temee0/Human-Resources-Analytics-Report/blob/main/intro%20page%201.png)

## Introduction
This HR analytics project focuses on analyzing Employee data within a fictional company. Our goal is to uncover insights that answer key questions and guide data-driven decisions.  

By employing descriptive, diagnostic, and prescriptive analysis, we aim to summarize employee data, understand the work force composition, determine employee performance and job satisfaction level, and provide actionable recommendations for improvement.   

Through this analysis, we seek to make informed decisions regarding promotions and retrenchments, as well as implement strategies to improve overall performance and job satisfaction among employees.

**_Disclaimer_** :  _The dataset used in this analysis is sourced online and is entirely fictitious. Therefore, this report does not represent any specific company, institution, or country. Rather, it serves as a demonstration of data analysis skills, PowerBI visualization skills, and knowledge of the DAX language._

## Problem Statement
1. Distribution of employees across gender, age groups, and departments.
2. Evaluation of job satisfaction levels among employees.
3. Assessment of employee performance. 
4. Identification of employees eligible for promotion based on performance and tenure.
5. Total number of employees to be retrenched.
6. How to incentivise employees to increase job satifaction and employees perfomance.

## Analysis toolkit
### Microsoft powerBI:
- DAX
- Visual tools
- Modelling
- Page navigation
- Buttons
- Bookmarking
- Filters
- Tooltips

## Modelling
A one-to-one relationship has been automatically derived from these datasets and remains unchanged.

![](https://github.com/temee0/Human-Resources-Analytics-Report/blob/main/HR%20data%20model.jpg)

## Visualization
This report comprises of 3 pages 
- home page
- Action page
- Detail page
      
You can interact with the report [here]

## Home Page
![](https://github.com/temee0/Human-Resources-Analytics-Report/blob/main/home%20page.jpg)
- There are a total of 1470 employees.
- Among them, 588 are female and 882 are male.
- The number of employees to be retrenched is 117.
- 72 employees are due for promotion.
- The average length of service for employees is 7 years.
- 85% of employees reside within close or very close proximity to the workplace.

## Action Page 
![](https://github.com/temee0/Human-Resources-Analytics-Report/blob/main/Action%20page.jpg)
- The sum of monthly income of employees is $9,559,309.
- The total count of married employees is 673.
- The total count of single employees is 470.
- The total count of divorced employees is 327.
- The average monthly income for employees amounts to $6,403.
- The youngest and oldest employees are  18 and 60 respectively.
- The highest sum of monthly income is earned by employees aged 40, with an average monthly income of $7,701.

## Detail Page
![](https://github.com/temee0/Human-Resources-Analytics-Report/blob/main/Details%20page.jpg)
### Research and Development Department:   
- The total count of employees is 961.
- The number of employees to be retrenched are 74
- 47 employees are due for promotion
- Breakdown of performance ratings among employees:   
  **High rated**: 84%  
  **Low rated**: 16% 
- the job satisfaction levels of employee are distributed thus:  
  **High**: 366 Employees   
  **Medium**: 300 Employees  
  **Low**: 295 Employees  
- Number of distinct job roles within the department: 6.
- 271 employees are working overtime.

### Sales Department:
- The total count of employees is 446.
- The number of employees to be retrenched are 36.
- 23 employees are due for promotion.
- Breakdown of performance ratings among employees:  
  **High rated**: 86%   
  **Low rated**: 14% 
- the job satisfaction levels of employee are distributed thus:  
  **High**: 172 Employees   
  **Low**: 147 Employees  
  **Medium**: 127 Employees  
- Number of distinct job roles within the department: 3.
- 128 employees are working overtime.  
  
### Human Resources Department
- The total count of employees is 63.
- The number of employees to be retrenched are 7.
- 2 employees are due for promotion.
- Breakdown of performance ratings among employees:  
  **High rated**: 86%  
  **Low rated**: 14%
- The job satisfaction levels of employee are distributed thus:  
  **High**: 31 Employees   
  **Low**: 17 Employees  
  **Medium**: 15 Employees  
- Number of distinct job roles within the department: 2.
- 17 employees are working overtime.

## Conclusion
The total count of employees stands at 1470, comprising 882 male employees and 588 female employees. Among them, 46% are married, 32% are single, and 22% are divorced. These individuals are distributed across three departments: Research and Development, Sales, and Human Resources, encompassing a total of 11 job roles.

The total monthly income disbursed to employees amounts to $9,559,309, with an average income of $6,503.

A total of 117 employees have been identified for retrenchment, while 72 are due for promotion. The longest-serving employee has dedicated 40 years to the company. The company"s average lenght of service years is 7 years.

Regarding proximity to the workplace, an impressive 85% reside within close or very close proximity to the workplace, accounting for 1241 individuals. Consequently, 229 employees live further away.  

Employee performance ratings are notably high, with 85% of the workforce receiving high ratings. However, job satisfaction rating reveal disparities, with 459 employees reporting low satisfaction, 442 reporting medium satisfaction, and 567 reporting high satisfaction.

Furthermore, 28% of employees worked outside standard working hours (overtime).

## Recommendations  
The insight about employees' proximity to the workplace should be utilized and flexible work arrangements such as remote work or flexible hours for employees who live further away should be implemented. This can improve employee morale, reduce commuting stress, and enhance work-life balance.     

The disparities in job satisfaction ratings should be addressed by conducting thorough assessments to identify the root causes. Implement initiatives such as regular feedback sessions, recognition programs, and opportunities for professional development to improve overall job satisfaction and retention.  

The company needs to reduce its workforce by 117 employees due to financial reasons. Simultaneously, there are 72 employees who are due for promotion. it is important to promote employees alongside retrenchment to mitigate the fear and uncertainty among the remaining workforce. By promoting deserving employees, the company sends a message that there are still opportunities for growth and advancement within the organization. This helps to reassure employees about their job security and reduces anxiety about potential future layoffs. it's also important to handle the retrenchment process with sensitivity and transparency. Provide support services such as career counseling and job placement assistance to those affected.   

It is important to mitigate negative perceptions of overtime by ensuring that overtime work is fairly compensated and recognized. 

It is important to recognize and celebrate the dedication of the longest-serving employee who has contributed 40 years to the company. This as an opportunity to highlight the value of employee loyalty, and ensure the transfer of knowledge within the organization.  

## Data Transformation/Cleaning   
Data was efficiently cleaned and transformed using power query and the DAX langyage. Some of the applied steps are listed below:
- Using the power query editor to identify errors and make corrections
- Deleting duplicate rows using the power query editor.
- Identifying wrong data format and correcting them.
- The total number of employees was determined using the DAX countrow function  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Total Emp = COUNTROWS('HR Analytics Data')
  </kbd>
- Created a service year field using a calculated column,  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Service Year = COMBINEVALUES(" ",'HR Analytics Data'[YearsAtCompany],"Years")
  </kbd>
- Grouped employees' distance status as close, very close or very far using the Nested IF function  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 IF('HR Analytics Data'[DistanceFromHome]>19,"Very Far",IF('HR Analytics Data'[DistanceFromHome]>9,"Close","Very Close"))
  </kbd>
- Grouped employees' job satisfaction as high, low, or medium using the Nested IF function  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Job Satisfaction Rating = if('HR Analytics Data'[JobSatisfaction]=3,"medium",if('HR Analytics Data'[JobSatisfaction]<3,"high","low"))
  </kbd>  
- Employees' performance rating was grouped as high or low using the IF function  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Performance Rating = if('HR Analytics Data'[PerformanceRating]=3,"high rated","low rated")
 </kbd>
- I created a metric and a calculated column to identify employees to be retrenched using the DAX IF function  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Retreanchment Status = if('HR Analytics Data'[YearsAtCompany]>17,"will be retreanched","on service")
  </kbd>         
- I createed a metric and a calculated column to identify employees that are due for promotion using the DAX IF function <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Due For Promotion = if('HR Analytics Data'[YearsSinceLastPromotion]>9,"Due For Promotion","Not Due")
  </kbd>    
- I calculated the Average montly income uding the DAX average function  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Average Monthly Income = AVERAGE('HR Analytics Data'[MonthlyIncome])
  </kbd>     
- I calculated the Average Service years using the DAX average function  <kbd style="background-color: #B8AFAF; padding: 10px; border-radius: 5px;">
 Average service year = AVERAGE('HR Analytics Data'[YearsAtCompany])
  </kbd>     

