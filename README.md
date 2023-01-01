# Pewlett-Hackard-Analysis #

## Overview of the analysis ##

### Background ###
  Pewlett Hackard is a large corporation that has identified the need to asses its future workforce needs given the approaching "silver tsunami". This play on words, although punny, poses a great threat to corporations as a large portions of their workforce are soon to retire. This population is known as the baby boomers.

### Purpose ###
  The purpose of this analysis is to determine the number of retiring employees per title and to identify employees who are eligible to participate in a mentorship program. The analysis will provide insights on how to prepare for the large amount of employees that will be retiring in the near future.
  Bobby, an HR Analyst for Pewlett Hackard, was tasked with two very important questions to answer in regards to the "silver tsunami":
  1. Which of the retiring population meets the criteria for a retirement package?
  2. Which positions are priority to be filled after positions become vacant from retiries?
  
  In order for Bobby to find answers to these questions, he will need to assess six CSV files and build a database to find relationships between data using primary and foreign keys. Below are the links to the six CSV files used in these findings:
  1. [departments.csv](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/Data/departments.csv)
  2. [dept_emp.csv](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/Data/dept_emp.csv)
  3. [dept_managers.csv](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/Data/dept_manager.csv)
  4. [employees](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/Data/employees.csv)
  5. [salaries](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/Data/salaries.csv)
  6. [titles.csv](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/Data/titles.csv)
  
### Flowchart ###
![EmployeeDB](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/EmployeeDB.png)
  
  A first step in building a database is to map out the flow or relationship between all your data files. In this case there are 6 CSV files that we will use to find patterns to answer our two questions. The relationships are identified by the lines connecting each of the tables. Those with a key are indicative of primary keys, meaning they are unique identifiers for that table. Those column names that are bolded are foreign keys, meaning they are primary key in another table.

## Results ##

* According to the unique_titles data, there are 90,398 employees who were born between 1952 and 1955 who are about to retire.
* According to the mentorship_eligiblty data, there are 1,940 employees who were born between January 1965 and December 1965 who are eligible to participate in a mentorship program
* The below screenshot shows that the highest number of retirees is those with the title "Staff" and the lowest is "Assistant Engineer"

![1](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/1.png)

* The below screenshot groups the number of employees (divided by title) who are eligible for the mentorship program.

![2](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/2.png)

***IN ADDITION TO THE 4 MAJOR POINTS ABOVE I WOULD LIKE TO ADD 2 ADDITIONAL FINDINGS***

#### Finding One - The Number of Retiring Employees by Title ####

This data CSV file was created using a relational database called PostgreSQL. The purpose of this file was to identify each occurance of a Pewlett Hackard employee who is retiring. Of those what is their employee number, title and dates of employment. This identifies both the count of employees potentially leaving the corporation and which job titles will need to be filled. For finding number one, Bobby has found that there are 133,776 employees who are in the retirement age and may plan on leaving the corporation. This is a large portion of their workforce and ensures that proper strategic planning will need to be performed for the corporation to maintain its standard level of business given the terminations.

#### Finding Two - The Employees Eligible for the Mentorship Program ####

This data CSV file was created using a relational database called PostgreSQL. The purpose of this file was to identify those employees in Pewlett Hackard that are not retiring and are in favorable positions to receive mentorship and ultimately transition into one of the vacancies left by those retiring. It simply is a transition of resources throughout the corporation. Finding number three, related to this CSV file, is that there are 1,550 current employees who qualify for mentorship and vertical move up the corporate latter. It should be realized that of the small 1,550 employees who are eligible for mentorship, this would only satisfy a small subset of those retiring. For this purpose these individuals should be considered for leadership positions.

## Summary ##

Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami.":

> 1. How many roles will need to be filled as the "silver tsunami" begins to make an impact?.

>> 90,398 roles are in urgent need to be filled out as soon as the workforce starts retiring at any given time.

> 2. Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

>> No, we have 1,940 employees who are eligible to participate in a mentorship program.
![Screenshot](images/Question2image.jpg)

***Additional Insights***

> 64% of employees holding senior titles are reaching retirement age. Therefore, the mentorship program will be a helpful way to transition new employees into Pewlett Hackard. Current data shows that 1940 employees who are retirement_ready employees are available to mentor the next generation of pewlett hackard employees. In sum, there is not a 1 to 1 ratio for the mentorship program, however there is a large enough buffer that it will be helpful.

> Another potential actionable insight is to mentor more than one new employee per eligile mentorship trainer. This could reduce the stress of not enough trainers and help teach the new employees team work and company culture.
![3](https://github.com/salvamike/Pewlett-Hackard-Analysis/blob/main/3.png)
