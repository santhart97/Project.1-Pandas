# Project.1-Pandas
Primer proyecto de Ironhack

# 1. Introduction
This was my first project in the Data Analytics bootcamp with Ironhack. It consisted in:
* I downloaded the global-shark-attacks .csv file compiled by Toby Jolly from kaggle. (https://www.kaggle.com/teajay/global-shark-attacks)
* The goal was to clean the data, and build a hypothesis that could be proved or disproved by analysing the data.
* I used the following libraries: Pandas, Numpy, Re, and Seaborn to vizualize the data.

# 2. Hypothesis
* My hypothesis is that, the average age of the victims in the 3 countries with the highest number of shark attacks would be around the same. 

# 3. Cleaning
* At first the data was very messy, the dataframe consisted of 25,723 rows and 24 columns. 
* The first step I used was to check if some of the rows were repeadet and get rid of them using, drop_duplicates(). I found that 19,411 rows were duplicates. Now I had 6,312 rows in the data.
* The second step was to see how many values were missing in the data using, isnull() and then dropping those values using, dropna().
* The data had many columns which were not useful or were repeated (eg. dates) so I dropped some columns, using .drop(columns=[]), and kept only the ones I felt were useful and gave a good understanding of the data as a whole.
* By the time the data was cleaned, I had a dataframe that consisted of 3,091 rows X 10 columns. A dataframe much smaller, tidier, easy to understand, and more readily representative of what I was looking for.

