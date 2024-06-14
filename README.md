# Python-challenge
![image](https://github.com/RoshniRanaDS/Data_Analysis_Using_Pandas/assets/161755928/b07ccb91-97f5-4461-9f47-5147386f5a3a) & ![image](https://github.com/RoshniRanaDS/Data_Analysis_Using_Pandas/assets/161755928/9b82848f-6a53-4432-986d-e058768ab3cb)


## Created And Manipulated Pandas DataFrames To Analyze School, Student's Budgets And Standardized Test Data.
![image](https://github.com/RoshniRanaDS/Data_Analysis_Using_Pandas/assets/161755928/c276f961-d746-4721-ac4c-0c75b1e51356)



# Background
As You are the new Chief **Data Scientist** for your city's school district. 
In this capacity, you'll be helping the **school board** and **mayor** make _strategic decisions_ regarding future school _budgets_ and _priorities_.
As a first task, you've been asked to **analyze** the district-wide _standardized test results_. You'll be given access to every student's **math** and **reading scores**, as well as various information on the schools they attend. Your task is to _aggregate_ the data to showcase obvious _trends_ in school performance.


## Repo Instructions
- [x] Created a new repository for this project called `pandas-challenge`, `Cloned` the new repository to local by `terminal`.  
- [x] Inside my local Git repository, created a folder for `"PyCitySchools"`  
- [x] Added `Jupyter notebook` _"(PyCitySchools_starter_Roshni.ipynb)"_ to this folder. This is the **main script** to run this analysis.  
- [x] A `Resources` folder that contains the _csv_ files(Raw Data) i have used.  
- [x] Also this folder that contains **"pdf"** file that has the results from the conducted analysis.  
- [x] Pushed these changes to `GitHub` profile by `bash terminal`.  

#
#
> [!NOTE]
> Useful information that users should know, even when skimming content.
#
## Instructions
Using `Pandas` and `Jupyter Notebook`, created a report that includes the following data. Report is included a written description of at least two observable trends based on the data.

Check out the sample solution called `"PyCitySchools_starter.ipynb"` located in the "PyCitySchools" folder
to review the desired edges for this analysis.

#
#
> [!IMPORTANT]
> Key information users need to know to achieve their goal.
#


## District Summary
Performed the necessary calculations and then created a `high-level` snapshot of the district's `key metrics` in a DataFrame.

Include the following:

- Total number of unique schools
- Total students, Total budget
- `Average` math score
- `Average` reading score
- `% passing` math (the percentage of students who passed math)
- `% passing` reading (the percentage of students who passed reading)
- `% overall passing` (the percentage of students who passed math AND reading)

## School Summary
Performed the necessary calculations and then created a `DataFrame` that summarizes `key metrics` about each school.

Include the following:

- School name
- School type
- Total students
- Total school `budget`
- Per student `budget`
- `Average` math score
- `Average` reading score
- `% passing math` (the percentage of students who passed math)
- `% passing reading` (the percentage of students who passed reading)
- `% overall passing` (the percentage of students who passed math AND reading)

## Highest-Performing Schools (by % Overall Passing)
`Sorted` the schools by `% Overall Passing` in `descending` order and display the top 5 rows.
Saved the results in a DataFrame called _"top_schools"_.

## Lowest-Performing Schools (by % Overall Passing)
Sorted the schools by `% Overall Passing` in `ascending` order and displaied the top 5 rows.
Saved the results in a DataFrame called _"bottom_schools"_.

## Math Scores by Grade
Performed the necessary calculations to create a `DataFrame` that lists the `average math` score for students of each `grade` level (9th, 10th, 11th, 12th) at each school.

## Reading Scores by Grade
Created a `DataFrame` that lists the `average` reading score for students of each `grade` level (9th, 10th, 11th, 12th) at each `school`.

## Scores by School Spending
- Created a `table` that breaks down school performance based on `average` spending ranges (per student).  
- Used required code to create four `bins` with reasonable cutoff values to `group` school spending.
#
![image](https://github.com/RoshniRanaDS/Data_Analysis_Using_Pandas/assets/161755928/f39b106b-c2ed-4347-af16-7f12ea2d085d)
#
- Used `pd.cut` to categorize spending based on the `bins`.    
- Created the following `code` to calculate `mean` scores per spending range
  
>spending_math_scores = school_spending_df.groupby(["Spending Ranges (Per Student)"])["Average Math Score"].mean()  
>spending_reading_scores = school_spending_df.groupby(["Spending Ranges (Per Student)"])["Average Reading Score"].mean()  
>spending_passing_math = school_spending_df.groupby(["Spending Ranges (Per Student)"])["% Passing Math"].mean()  
>spending_passing_reading = school_spending_df.groupby(["Spending Ranges (Per Student)"])["% Passing Reading"].mean()  
>overall_passing_spending = school_spending_df.groupby(["Spending Ranges (Per Student)"])["% Overall Passing"].mean()

- Used the scores above to create a `DataFrame` called "`spending_summary`".  

### Included the following metrics in the table:

- `Average` math score
- `Average` reading score  
- `% passing math` (the percentage of students who passed math)
- `% passing reading` (the percentage of students who passed reading)
- `% overall passing` (the percentage of students who passed math AND reading)

## Scores by School Size
- Created the required code to bin the `per_school_summary.`
#
  ![image](https://github.com/RoshniRanaDS/Data_Analysis_Using_Pandas/assets/161755928/3ff4b85c-ec3d-43cb-bf16-20f1c384fc67)
#
- Used "`pd.cut`" on the "Total Students" column of the "`per_school_summary`" DataFrame.  
- Created a DataFrame called "`size_summary`" that breaks down school performance based on `school` size (small, medium, or large).

## Scores by School Type
Used the "`per_school_summary`" DataFrame from the previous step to create a new DataFrame called "`type_summary`".

### This new `DataFrame` should show school performance based on the "`School Type`".
#
#
> [!IMPORTANT]
> Key information users need to know to achieve their goal.
# Final Statement for Provided Data
#
## Summary of Analysis:
The `analysis` focused on evaluating the `academic performance` of schools based on various factors such as school type, size, and per student budget. It examined average math and reading scores, as well as the percentage of students passing math, reading, and overall. The data revealed significant differences between Charter and District schools, with Charter schools consistently performing better across all metrics. Additionally, the analysis explored the relationship between per student budget and academic performance, noting that higher budget allocation did not always correlate with better outcomes. 

- This suggests that how factors beyond financial resources, such as teaching quality and school culture, may influence student achievements.  

### Overall, the analysis highlights the importance of considering multiple factors when assessing school performance and emphasizes the need for further investigation into effective educational practices.
#
#
> [!NOTE]
> Useful information that users should know, even when skimming content.
#

## Key Findings:
# Comparison of School Types:
I. In every criterion, charter schools did better than district schools. Overall passing rates, percentages of children passing math and reading, and average math and reading scores were all higher in charter schools.  
II. The `average` math and reading scores for charter schools were 83.47 and 83.90, respectively, considerably higher than the `average` scores of 76.96 and 80.97 for district schools.  
III.Additionally, the passing `percentages` in arithmetic (93.62% vs. 66.55%) and reading (96.59% vs. 80.80%) were much better in Charter schools, leading to an overall passing rate of 90.43% compared to 53.67% for District schools.  

# Budget per Student Analysis:
I.The investigation also looked into how each student's `budget` affected their academic achievement. Unexpectedly, schools with smaller funds per student frequently fared better than those with larger budgets.  
II.91.33% was the `highest` overall passing percentage for schools in the lowest budget category (<$585), while 54.64% was the highest for schools in the highest budget group ($645–680).  
III. This shows that a number of `variables`, including school administration, resource distribution, and the caliber of instruction, are more important in predicting academic performance than `financial constraints`.  

# Analysis Findings:
The research emphasizes how crucial school style and efficient resource use are in affecting student success. Charter schools routinely outperform District schools, while sometimes having smaller funding per student. This shows how important the instructional ideas and approaches used by these schools are.

The results also cast doubt on the idea that larger budgets equate to improved academic performance, emphasizing the need for a more complex understanding of the variables influencing school achievement outside of financial resources. This suggests that spending more on student support services, curriculum development, and teacher training might improve student accomplishment more than just raising funding levels.
#
#
> [!IMPORTANT]
> Key information users need to know to achieve their goal.
#
# Conclusion
In conclusion, while financial resources are important for educational institutions, the analysis underscores the significance of other factors such as school type and teaching methodologies in driving academic excellence. Moreover, it highlights the need for further investigation into the specific practices and approaches employed by Charter schools that contribute to their superior performance compared to District schools.
