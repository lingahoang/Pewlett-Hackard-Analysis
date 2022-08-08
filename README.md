# Pewlett-Hackard-Analysis

## Overview
In this project, we are helping Bobby to analyze on given data using PostgreSQL to generate result. The assignment was to determine the number of retiring employees per title and identify employees who are eligible to participate in a mentorship program. This analysis is helping Bobby's manager to prepare for the "silver tsunami" as the result will tell us the number of current employees will reach the retirement age. 

## Result

### Deliverable 1: The Number of Retiring Employees by Title
To retrieve the number of retiring employees by title, here are some information that we generated below:

- Retirement Titles table for employees who are born between January 1, 1952 and December 31, 1955.

![retirement_titles](https://user-images.githubusercontent.com/107448172/183279198-15fc1ab1-c2ce-494a-aed4-aada2c2a7eb5.png)

In this table, we inner joined the employees table and titles table, which is given data, into this table that included employees number, first and last name, their title, their from date which is start date and to date which mean their up-to-date. All of the employees that are born betwen January 1, 1952 and December 31, 1955, are either still with the company which has to date as 9999-01-01 or their end date already. But as we can see, this table collected all data of all employees with their previous title before into this analysis.

- Unique Titles table that contains the employees' number, first and last name, and most recent title.

![unique_titles](https://user-images.githubusercontent.com/107448172/183279199-5d48b326-167e-4c7a-9578-cc7f849b01f3.png)

In this table, we excluded the employees that already left the company, so we won't be able to see a name that repeated twice.

- Retiring Titles table that contains the number of titles filled by employees who are retiring. 

![retiring_titles](https://user-images.githubusercontent.com/107448172/183279203-2278a5df-a271-4909-b65c-5b5f25d52afa.png)

In this table, you can see we did a count of total employees per titles, which tell us there will be 25,916 senior engineers will retire, then senior staffs, followed by engineers, staffs, with about 4,000 technique leaders and assistant engineers with only 2 managers will soon be retiring. 

### Deliverable 2: The Employees Eligible for the Mentorship Program

Since this deliverable will need a few columns from the employees table, the department employees table and the titles table. We performed a join to retrieve employee number, first and last name, and birth date, from date and to date and title columns and put into this list. We also only need employees that was hired between January 1, 1965 and December 31, 1965 that are still working with the company. Those listed below will be able to join the mentorship program. 

![mentorship_eligibility](https://user-images.githubusercontent.com/107448172/183280637-dd28d1a3-4b09-43b5-9b5f-5c3750f887ae.png)

## Summary

Based on the number of retiring employees by title, there are total of 72,458 employees in the company will be retiring soon. There will also 1,549 employees that will be qualify for the mentorship program. This time, Pewlett Hackard is not ready for the silver tsunami hit since they still need at least 70,000 new position to fill those empty seats.




