# Toman-Bike-Share-Analysis

![excel_to_powerbi_animated-diagram](assets/images/kaggle_to_powerbi.gif)

# Table of contents

- [Objective](#objective)
  - [User story](#user-story)
- [Data source](#data-source)
- [Stages](#stages)
- [Design](#design)
  - [Dashboard components](#dashboard-components-required)
- [Dashboard mockup](#dashboard-mockup)
- [Tools](#tools)
- [Development](#development)
- [Pseudocode](#pseudocode)
- [Data exploration notes](#data-exploration-notes)
- [Data cleaning](#data-cleaning)
  - [Transform the data](#transform-the-data)
  - [Create the SQL view](#create-the-sql-view)
- [Testing](#testing)
  - [Column count check](#column-count-check)
  - [Data type check](#data-type-check)
  - [Duplicate count check](#duplicate-count-check)
- [Visualisation](#visualisation)
  - [DAX measures](#dax-measures)
- [Analysis](#analysis)
  - [Validation](#validation)
  - [Discovery](#discovery)
- [Recommendations](#recommendations)
  - [Potential ROI](#potential-ROI)
  - [Action plan](#action-plan)
# Objective
# Development
# Design
# Visualization
# Analysis






# Development
### Pseudocode
   *  What's the general approach in creating this solution from start to finish?
   1. Get the data
   2. Explore the data in SQL server management studio
   3. Clean the data with SQL
   4. Do some touch ups with power query
   5. Visualize the data in Power BI
   6. Generate the findings based on the insights






We want to make sure all our data is join together for us to make it simple to use
so 
1. Used union to combine the two tables 2021 and 2022 in order to connect the two tables as one after checking them well and noticing that they both have the same kind of data with unique rows using union instead of union all to make sure we don't have any duplicated rows
created a CTE inoder to connect the newly combined table with the cost table
2. We first checked for what our we have in common for our tables g«found out that the yr column is common amoung all the table so we used it to cjoin the tables we use left join inorder to get all the records from our left table which is the cte is our main table and we want it to match with the cost table and bring back back all the rows from the left and match it
3.   Now just need to pick the columns that are needed for our project which are the date, season,the year,riders,the rider type,price and COGS

4.   Rounded the price column to two decimal places
5. The we noticed the cogs column had the time data type so we went ahead and changed it to decimal then later changed to money in power query
6. to get the revenue we did riders * price
7. for the profit we did riders * price - COGS
