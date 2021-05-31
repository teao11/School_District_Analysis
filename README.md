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

<img width="924" alt="Screen Shot 2021-05-30 at 5 28 41 PM" src="https://user-images.githubusercontent.com/46773181/120125182-7ba56e00-c16c-11eb-91cb-11c31308709b.png">

Please see below for the district summary, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="924" alt="Screen Shot 2021-05-30 at 5 26 40 PM" src="https://user-images.githubusercontent.com/46773181/120125130-400aa400-c16c-11eb-9f63-93035a437e3c.png">

As we see above, the overall district was not terribly affected by the data issue. This could be due to the fact that the Thomas High School 9th grade makes up a very small % of the overall district population, and that there were few outliers within the 9th grade population that would cause the average to be shifted.

We do see the total students column reflect the fact that we have removed the 9th Grade class from Thomas High School.

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

<img width="459" alt="Screen Shot 2021-05-30 at 5 41 19 PM" src="https://user-images.githubusercontent.com/46773181/120125572-3eda7680-c16e-11eb-8598-aee3d6738d33.png">

Please see below for the reading summary by grade, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="463" alt="Screen Shot 2021-05-30 at 5 42 33 PM" src="https://user-images.githubusercontent.com/46773181/120125620-6b8e8e00-c16e-11eb-9eab-357b7c595f6b.png">

As we can see above, removing the 9th grade scores from Thomas High School will only affect this segment . Thomas High School 9th Grade scores have been replaced with NaN, as requested, so there is no mean score for this segment.

Please see below for the math summary by grade, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="461" alt="Screen Shot 2021-05-30 at 5 41 41 PM" src="https://user-images.githubusercontent.com/46773181/120125586-5580cd80-c16e-11eb-8881-27f76884a3f6.png">

Please see below for the math summary by grade, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="460" alt="Screen Shot 2021-05-30 at 5 42 47 PM" src="https://user-images.githubusercontent.com/46773181/120125629-73e6c900-c16e-11eb-8df0-2b8515e0bb1d.png">

Similar to the prior paragraph, removing the math scores and segmenting by grade ensures that only the Thomas High School grade scores will be affected! The 9th Grade scores for Thomas High School have been listed as NaN as requested.

Similar to the reading scores, removing the 9th grade scores from Thomas High School will only affect this segment. Thomas High School 9th Grade scores have been replaced with NaN, as requested, so there is no mean score for this segment again.

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

Please see below for the score summary by school type, **before** we addressed the issues with Thomas High School 9th Grade:

<img width="635" alt="Screen Shot 2021-05-30 at 5 05 54 PM" src="https://user-images.githubusercontent.com/46773181/120124423-4d725f00-c169-11eb-9b2c-4d5d0100993f.png">

Please see below for the score summary by school type, **after** we addressed the issues with Thomas High School 9th Grade:

<img width="635" alt="Screen Shot 2021-05-30 at 5 06 20 PM" src="https://user-images.githubusercontent.com/46773181/120124448-60852f00-c169-11eb-81a4-4bedae6e7d44.png">

Thomas High School is a Charter School, and so we would only expect to see changes to that segment in the dataframes above. However, we see a similar trend to the ones I have discussed prior to this -- the 9th grade class at Thomas High School represents such a small % of the entire charter school segment, that we see no an insignificant to no change after we replaced the Thomas High School 9th Grade scores.

## Summary

