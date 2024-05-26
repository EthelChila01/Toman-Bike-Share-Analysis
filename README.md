# Toman-Bike-Share-Analysis
# Table of contents
# Objective
# Development
# Design
# Visualization
# Analysis

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
