# Created And Manipulated Pandas DataFrames To Analyze School, Student's Budgets And Standardized Test Data.

# Background
As You are the new Chief Data Scientist for your city's school district. 
In this capacity, you'll be helping the school board and mayor make strategic decisions regarding future school budgets and priorities.
As a first task, you've been asked to analyze the district-wide standardized test results. You'll be given access to every student's math and reading scores, as well as various information on the schools they attend. Your task is to aggregate the data to showcase obvious trends in school performance.

# Repo Instructions

Created a new repository for this project called #pandas-challenge, Cloned the new repository to local by terminal.

Inside my local Git repository, created a folder for "PyCitySchools"

Added Jupyter notebook "(PyCitySchools_starter.ipynb)" to this folder. This is the main script to run this analysis.

A Resources folder that contains the CSV files(Raw Data) i have used. 

Also this folder that contains "pdf" file that has the results from the conducted analysis.

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
Used the scores above to create a DataFrame called "spending_summary".

Include the following metrics in the table:

Average math score, Average reading score, % passing math (the percentage of students who passed math), % passing reading (the percentage of students who passed reading), % overall passing (the percentage of students who passed math AND reading)

# Scores by School Size
Created the required code to bin the per_school_summary.
Used "pd.cut" on the "Total Students" column of the "per_school_summary" DataFrame.

Created a DataFrame called "size_summary" that breaks down school performance based on school size (small, medium, or large).

# Scores by School Type
Used the "per_school_summary" DataFrame from the previous step to create a new DataFrame called "type_summary".

This new DataFrame should show school performance based on the "School Type".

# Final Statement for Provided Data
# Summary of Analysis:
The analysis focused on evaluating the academic performance of schools based on various factors such as school type, size, and per student budget. It examined average math and reading scores, as well as the percentage of students passing math, reading, and overall. The data revealed significant differences between Charter and District schools, with Charter schools consistently performing better across all metrics. Additionally, the analysis explored the relationship between per student budget and academic performance, noting that higher budget allocation did not always correlate with better outcomes. This suggests that how factors beyond financial resources, such as teaching quality and school culture, may influence student achievements. Overall, the analysis highlights the importance of considering multiple factors when assessing school performance and emphasizes the need for further investigation into effective educational practices.

# Key Findings:
# Comparison of School Types:
I.
In every criterion, charter schools did better than district schools. Overall passing rates, percentages of children passing math and reading, and average math and reading scores were all higher in charter schools.

II.
The average math and reading scores for charter schools were 83.47 and 83.90, respectively, considerably higher than the average scores of 76.96 and 80.97 for district schools.

III.
Additionally, the passing percentages in arithmetic (93.62% vs. 66.55%) and reading (96.59% vs. 80.80%) were much better in Charter schools, leading to an overall passing rate of 90.43% compared to 53.67% for District schools.

# Budget per Student Analysis:
I.
The investigation also looked into how each student's budget affected their academic achievement. Unexpectedly, schools with smaller funds per student frequently fared better than those with larger budgets.

II.
91.33% was the highest overall passing percentage for schools in the lowest budget category (<$585), while 54.64% was the highest for schools in the highest budget group ($645–680).

III.
This shows that a number of variables, including school administration, resource distribution, and the caliber of instruction, are more important in predicting academic performance than financial constraints.

# Analysis Findings:
The research emphasizes how crucial school style and efficient resource use are in affecting student success. Charter schools routinely outperform District schools, while sometimes having smaller funding per student. This shows how important the instructional ideas and approaches used by these schools are.

The results also cast doubt on the idea that larger budgets equate to improved academic performance, emphasizing the need for a more complex understanding of the variables influencing school achievement outside of financial resources. This suggests that spending more on student support services, curriculum development, and teacher training might improve student accomplishment more than just raising funding levels.

# Conclusion
In conclusion, while financial resources are important for educational institutions, the analysis underscores the significance of other factors such as school type and teaching methodologies in driving academic excellence. Moreover, it highlights the need for further investigation into the specific practices and approaches employed by Charter schools that contribute to their superior performance compared to District schools.
