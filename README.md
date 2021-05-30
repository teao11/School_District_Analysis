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

For Thomas High School, we see the following changes:
* Average Math Score: 83.4 to 83.3
* Average Reading Score: 83.8 to 83.9
* % Passing Math: 93.3 to 93.2
* % Passing Reading: 97.3 to 97.0
* Overall Passing %: 90.9 to 90.6

Overall, we saw very little shift in the statistics here. This suggests that the 9th grade class results were relatively in line with the overall Thomas High School results.

#### 3) How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

As we saw in the previous section, the overall passing percentage from Thomas High School fell slightly when we replaced the ninth graders' math and reading scores. The school still performs at a very high standard, and maintains its' second place standing in terms of overall passing percentage vs. other schools in the district.

In terms of **% passing reading**, replacing the ninth graders' results drops it below Griffin High School in terms of performance. When we look at **% passing math**, Thomas High School changes very little when comparing to other schools.

#### 4) How does replacing the ninth-grade scores affect the following: Math and reading scores by grade

Please see below for the reading summary by grade, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="456" alt="Screen Shot 2021-05-30 at 4 10 01 PM" src="https://user-images.githubusercontent.com/46773181/120123025-7ee72c80-c161-11eb-9a62-49df17cb9186.png">

Please see below for the reading summary by grade, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="456" alt="Screen Shot 2021-05-30 at 4 15 04 PM" src="https://user-images.githubusercontent.com/46773181/120123176-3c721f80-c162-11eb-815e-e7ec3322f01c.png">

As we can see above, removing the 9th grade scores from Thomas High School will only affect the 9th grade segment here. Thomas High School 9th Grade scores have been replaced with NaN, as requested!

Please see below for the math summary by grade, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="467" alt="Screen Shot 2021-05-30 at 4 11 57 PM" src="https://user-images.githubusercontent.com/46773181/120123092-c372c800-c161-11eb-83af-68586657414f.png">

Please see below for the math summary by grade, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="458" alt="Screen Shot 2021-05-30 at 4 15 04 PM" src="https://user-images.githubusercontent.com/46773181/120123306-e6ea4280-c162-11eb-9edf-0c21a30c4968.png">

Similar to the prior paragraph, removing the math scores and segmenting by grade ensures that only the Thomas High School grade scores will be affected! The 9th Grade scores for Thomas High School have been listed as NaN as requested.

Removing the 9th grade population from the denominator and grouping by school name has shifted the other Thomas High School grades up very slightly:
* 10th Grade: 83.1 to 84.3
* 11th Grade: 83.5 to 83.6
* 12th Grade: 83.5 to 83.8 

#### 5) How does replacing the ninth-grade scores affect the following: Scores by school spending

Please see below for the score summary by school spending, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="749" alt="Screen Shot 2021-05-30 at 4 23 41 PM" src="https://user-images.githubusercontent.com/46773181/120123391-7bed3b80-c163-11eb-8386-18f5ca3d5d3d.png">

Please see below for the score summary by school spending, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="710" alt="Screen Shot 2021-05-30 at 4 24 56 PM" src="https://user-images.githubusercontent.com/46773181/120123411-945d5600-c163-11eb-82ca-9f52caf1d6ff.png">

By looking at the school summary dataframe above, we see that Thomas High School falls into the $630-644 bucket, and changing the scores for the Thomas High School 9th Graders' should only affect this bucket. When comparing the two dataframes, we see that there was very insignificant to no change here.

This makes sense, as this bucket also contains 3 other schools that are far larger (2000+ students). Consequently, the 9th Grade Class at Thomas High School represents a very small portion of the $630-644 bucket and was unlikely to change the score summary for this bracket, unless the 9th grade class contained significant outliers.

#### 6) How does replacing the ninth-grade scores affect the following: Scores by school size

Please see below for the score summary by school size, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="677" alt="Screen Shot 2021-05-30 at 4 32 40 PM" src="https://user-images.githubusercontent.com/46773181/120123608-a8ee1e00-c164-11eb-949c-550eb959dac9.png">

Please see below for the score summary by school size, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="677" alt="Screen Shot 2021-05-30 at 4 52 58 PM" src="https://user-images.githubusercontent.com/46773181/120124109-801b5800-c167-11eb-81b8-cd3e0951583e.png">

Understanding that Thomas High School falls into the Medium (1000-2000) segment, we would only see change when comparing these two buckets. Again, there is very little to no change here.

This can be explained due to the size of the 9th Grade Class at Thomas High School (~450) representing an insignificant portion of the overall Medium (1000-2000) segment. Again, this suggests that The 9th Grade Class at Thomas High School was very consistent with the overall average scores within this Medium (1000-2000) segment.

#### 7) How does replacing the ninth-grade scores affect the following: Scores by school type


## Summary
