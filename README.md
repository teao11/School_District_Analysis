# School_District_Analysis

## Overview of the school district analysis:

<p>
The purpose of this analysis was to allow us to utilize the Pandas / Jupyter Notebook skills we had learnt throughout the Module 4 coursework in a real-life scenario.

In this challenge, we were tasked with helping Maria prepare summary statistics for the district education board. These statistics that we produced would then be used to drive budgeting decisions for the next fiscal period.

We first created an analysis based on complete data from the district, throughout the module coursework. However, Maria and the board were notified that there were data integrity issues with a small population within the data we were provided. These issues affected our results, and so we had to reconstruct the analysis after addressing the issues found with the 9th grade class at Thomas High School.

My report below outlines the results from both my analysis, and compares the results (pre and post data cleanup) for the board.
</p>

## Results

#### 1) How is the district summary affected

_Please note: We had rounded our % to contain no decimal points in our coursework, and the dataframe columns were slightly different in terms of column order. I have made the challenge dataframes consistent with this format, for ease of comparison._

Please see below for the district summary, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="924" alt="Screen Shot 2021-05-30 at 3 37 38 PM" src="https://user-images.githubusercontent.com/46773181/120122325-fd8d9b00-c15c-11eb-9d17-7192358161f9.png">

Please see below for the district summary, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="924" alt="Screen Shot 2021-05-30 at 3 32 36 PM" src="https://user-images.githubusercontent.com/46773181/120122219-57419580-c15c-11eb-93f8-922e0f0ba307.png">

As we see above, the overall district was not terribly affected by the data issue. This could be due to the fact that the Thomas High School 9th grade makes up a very small % of the overall district population, and that there were few outliers within the 9th grade population that would cause the average to be shifted.

#### 2) How is the school summary affected

Please see below for the school summary, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="890" alt="Screen Shot 2021-05-30 at 3 44 56 PM" src="https://user-images.githubusercontent.com/46773181/120122546-5578d180-c15e-11eb-9e96-bc40ecc5bcc3.png">

Please see below for the district summary, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="890" alt="Screen Shot 2021-05-30 at 3 50 40 PM" src="https://user-images.githubusercontent.com/46773181/120122633-d59f3700-c15e-11eb-9e11-27b139b24774.png">

As this analysis segments by school, there is absolutely no change between the rows, except for the row containing Thomas High School.



#### 3) How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?


#### 4) How does replacing the ninth-grade scores affect the following: Math and reading scores by grade


#### 5) How does replacing the ninth-grade scores affect the following: Scores by school spending


#### 6) How does replacing the ninth-grade scores affect the following: Scores by school size


#### 7) How does replacing the ninth-grade scores affect the following: Scores by school type


## Summary
