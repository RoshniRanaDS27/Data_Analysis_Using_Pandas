# Created And Manipulated Pandas DataFrames To Analyze School, Student's Budgets And Standardized Test Data.

# Background
As You are the new Chief Data Scientist for your city's school district. 
In this capacity, you'll be helping the school board and mayor make strategic decisions regarding future school budgets and priorities.
As a first task, you've been asked to analyze the district-wide standardized test results. You'll be given access to every student's math and reading scores, as well as various information on the schools they attend. Your task is to aggregate the data to showcase obvious trends in school performance.

# Repo Instructions

Created a new repository for this project called # pandas-challenge, Cloned the new repository to local by terminal.

Inside my local Git repository, created a folder for "PyCitySchools"

Added Jupyter notebook "(PyCitySchools_starter.ipynb)" to this folder. This is the main script to run for analysis.

A Resources folder that contains the CSV files i have used. 

Also this folder that contains pdf file that has the results from the conducted analysis.

Pushed these changes to GitHub profile by bash terminal.

# Instructions
Using Pandas and Jupyter Notebook, created a report that includes the following data. Report is included a written description of at least two observable trends based on the data.

Check out the sample solution called "PyCitySchools_starter.ipynb" located in the "PyCitySchools" folder
to review the desired edges for this analysis.

# District Summary
Performed the necessary calculations and then created a high-level snapshot of the district's key metrics in a DataFrame.

Include the following:

Total number of unique schools, Total students, Total budget, Average math score, Average reading score, % passing math (the percentage of students who passed math), % passing reading (the percentage of students who passed reading), % overall passing (the percentage of students who passed math AND reading)

# School Summary
Performed the necessary calculations and then created a DataFrame that summarizes key metrics about each school.

Include the following:

School name, School type, Total students, Total school budget, Per student budget, Average math score, Average reading score, % passing math (the percentage of students who passed math), % passing reading (the percentage of students who passed reading), % overall passing (the percentage of students who passed math AND reading)

# Highest-Performing Schools (by % Overall Passing)
Sorted the schools by % Overall Passing in descending order and display the top 5 rows.
Saved the results in a DataFrame called "top_schools".

# Lowest-Performing Schools (by % Overall Passing)
Sorted the schools by % Overall Passing in ascending order and displaied the top 5 rows.
Saved the results in a DataFrame called "bottom_schools".

# Math Scores by Grade
Performed the necessary calculations to create a DataFrame that lists the average math score for students of each grade level (9th, 10th, 11th, 12th) at each school.

# Reading Scores by Grade
Created a DataFrame that lists the average reading score for students of each grade level (9th, 10th, 11th, 12th) at each school.

# Scores by School Spending
Created a table that breaks down school performance based on average spending ranges (per student).

Used required code to create four bins with reasonable cutoff values to group school spending.
Used pd.cut to categorize spending based on the bins.

Created the code to calculate mean scores per spending range
Used the scores above to create a DataFrame called spending_summary.

Include the following metrics in the table:

Average math score, Average reading score, % passing math (the percentage of students who passed math), % passing reading (the percentage of students who passed reading), % overall passing (the percentage of students who passed math AND reading)

# Scores by School Size
Created the required code to bin the per_school_summary.
Used pd.cut on the "Total Students" column of the per_school_summary DataFrame.

Created a DataFrame called size_summary that breaks down school performance based on school size (small, medium, or large).

# Scores by School Type
Used the per_school_summary DataFrame from the previous step to create a new DataFrame called type_summary.

This new DataFrame should show school performance based on the "School Type".
