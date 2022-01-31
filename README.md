# School_District_Analysis

## Overview of the school district analysis

A school district asked for a snapshot of several key metrics by each school campus and by the district level. The main analysis focused on the performance of math and reading scores disaggregated several ways in preparation for a board meeting. However, after the school board reviewed the data, it was determined that the data from Thomas High School's 9th grade class was suspect of cheating. The school board asked for the data to be removed and analyzed again for a comparison.

## Process

1. Open Jupyter Notebook files from local directories using a development environment.
2. Read an external CSV file into a DataFrame.
3. Format a DataFrame column.
4. Determine data types of row values in a DataFrame.
5. Retrieve data from specific columns of a DataFrame.
6. Merge, filter, slice, and sort a DataFrame.
7. Apply the groupby() function to a DataFrame.
8. Use multiple methods to perform a function on a DataFrame.
9. Perform mathematical calculations on columns of a DataFrame or Series

## Results

#### How each of the seven school district metrics was affected by the changes in the data

Original Analysis 
![image](https://user-images.githubusercontent.com/95304774/151830696-065e4ba0-d56e-4539-99ee-876d7bd4a5cb.png)

The testing data of 461 9th graders at Thomas High School was turned into null data, which recalculated the percentages of passing math, passing reading, and the overall passing. The total count of students did not change as that was run on the count of the student ids, which was not turned into null data.

Adjusted Analysis 
<img width="921" alt="Screen Shot 2022-01-31 at 10 18 16 AM" src="https://user-images.githubusercontent.com/95304774/151831189-9a09eab5-dfad-42b2-bd29-532bc2c897a0.png">

When comparing the two charts, removing less than 500 test scores had a nominal impact on the almost 40,000 student data set. The change was less than a 1% difference and the numbers would still round to the same whole number.

#### How is the school summary affected?

In the original analysis, Thomas High School started with a 91% overall passing rate, which was a concern to the school board as being too high. After calculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly.

Original Analysis 
![image](https://user-images.githubusercontent.com/95304774/151832097-15d61c53-5f84-4f9b-ab98-7b49adb6e520.png)

Adjusted Analysis
![image](https://user-images.githubusercontent.com/95304774/151834392-5e48f360-006c-45ef-b002-29f569ae3287.png)

Removing the 9th grade students from the data set had a huge impact by dropping from 91% to 65% for the overall passing rate.

#### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

In the original analysis, Thomas High School ranked 2nd in the district raising red flags with the school board.

Original Analysis
![image](https://user-images.githubusercontent.com/95304774/151834994-f8082dd5-a434-4431-9d0f-0920faf64a09.png)

After adjusting the 9th grade data, Thomas High School ranked in the exact middle of 15 campuses at 8th from the bottom.

Adjusted Analysis
![image](https://user-images.githubusercontent.com/95304774/151835528-44d2f6dd-bc16-41c9-87da-5584b6ac6c3c.png)

#### How does replacing the ninth-grade scores affect the following:

###### Adjusted Averages using the Math and Reading Scores

In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. Now the scores have been replaced with null values and shows up in Python programming as NaN in the following charts.

![image](https://user-images.githubusercontent.com/95304774/151836244-a810b8f3-d305-4722-829e-6eb240e16310.png)

![image](https://user-images.githubusercontent.com/95304774/151836331-b5fa7808-d5ab-4941-a664-f14a4463f3de.png)

#### Scores by school spending

Thomas High School falls in the $630-$644/student spending range. However, the hundredths place was needed to see the nominal changes.

Original Analysis 
![image](https://user-images.githubusercontent.com/95304774/151836709-7befc282-e515-4851-91ef-a4a6a63a3131.png)

Adjusted Analysis
![image](https://user-images.githubusercontent.com/95304774/151836753-05b04668-d0bd-4547-a8d9-03881ea3d5d6.png)

There was very little spending impact by changing the 9th grade scores.

#### Scores by school size

Thomas High School is defined as a medium sized school. The hundredths place was needed to see the nominal changes.

Original Analysis
![image](https://user-images.githubusercontent.com/95304774/151837292-841d2823-04fd-4037-8b7e-6fc069ac3afc.png)

Adjusted Analysis 
![image](https://user-images.githubusercontent.com/95304774/151837388-a8115e9d-7087-4f54-9705-ce935888f01d.png)

There was very little impact by campus size due to changing the 9th grade scores.

#### Scores by school type

Thomas High School is a charter school type. The hundredths place was needed to see the nominal changes.

Original Analysis
![image](https://user-images.githubusercontent.com/95304774/151837577-5d6711c7-2533-4a37-bada-b38d2e68d257.png)

Adjusted Analysis 
![image](https://user-images.githubusercontent.com/95304774/151837635-fc131df2-59a3-4487-9ba6-4d3c4061c5d6.png)

There was very little impact by school type by changing the 9th grade scores.

#### summarize four changes to the school district analysis after reading and math scores have been replaced

1. The overall passing rate for Thomas High School changed dramatically from 91% to 65%.

2. Thomas High School's ranking dropped from 2nd to 8th in the district of 15 campuses.

3. Data at the grade level will now show as "NaN" in reports for the 9th grade students at Thomas High School

4. In addition to the overall passing rate, the campus math and reading averages and passing percentages all saw shifts.

The major changes will be seen at the lower views of the disaggregated data with minor impact to the larger data views.
















