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

# 4. Results
* To look if my hypothesis was true, I imported my cleaned data and visualized it.
* I first started by looking at the countries in which there have been attacks and plotted a pie chart, after a failed attempt, I chose to show the 10 countries with the most attacks to better represent the data using, nlargest(10).
* After that, I concentrated on the USA, because is the country with the most shark attacks. I created a variable, sharks_usa, to only focus on the attacks in that particular country.
* I created a new column, 'Ages', and used, .unique() function to get the specific values of the array. Then I dropped the empty values 'dropna()'.
* I used a histplot with a kde line to show the data for the USA. It showed a greater concentration of young victims of ages around 20. I then used the .mean() function to get the average, and the result corroborated with the graph, stating that the average age of victims is 28 years old.
* After I concentrated on the second country with the most victims, Australia. I followed the same steps as with the USA in cleaning and creating a 'Ages' column with unique values.
* This time I used a countplot. At first, because there are so many ages, it wasn't clean and the graph couldn't be read properly. Therefore I created a 'Range' column, with ages ranging by 10 years each.
* In the following countplot, it showed that most victims are around 20 to 30 years old, and after that age the number of victims gradually fell.
* I found the mean and the result was, again, 28 years old.
* Lastly, I looked at South Africa and I used the same methods as with the USA.
* The mean age for victims was 26 years old, only sligtly lower than with the other two countries.

# 5. Conclusions
* My hypothesis set out to prove that most of the victims of shark attacks were around the same age, and the data showed that, that was true. With the USA and Australia having exactly the same average age of 28 years old. South Africa's average age was only slightly lower with a mean of 26 years old.
* This results corroorate my hypothesis
