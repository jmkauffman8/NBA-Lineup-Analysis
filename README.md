# NBA Lineup Analysis
Project that uses visualizations/variety of techniques to understand the best NBA lineups during the 2016-17 season and calculate the probability a given lineup is better than another

## Overview of NBA Lineup Analysis Project
This project uses lineup data from Cleaningtheglass.com to replicate analysis from the second edition of Chapter 32 of Mathletics in order to create a model that calculates the probability that one lineup is better than another.
In Basketball, simply swapping out two seemingly similarly skilled players can be the difference between a below average and an elite lineup. Figuring out a lineup that combines talent with chemistry is often what seperates the good coaches from the great, and Analytics has made this more possible than ever. For the 2016-2017 Atlanta Hawks, this statement rang particularly true, as simply subbing in Kent Bazemore for Thabo Sefalosha allowed the Hawks to field a lineup that was +30 stronger.

## Introduction

The NBA Lineup Analysis project is a data analysis project that focuses on analyzing the best NBA lineups during the 2016-17 season. The project aimed to use various visualization techniques and statistical models to understand the underlying factors that contribute to the success of a lineup. In particular, the project focused on replicating the analysis presented in Chapter 32 of Mathletics to create a model that calculates the probability that one lineup is better than another.

The project utilized data from Cleaningtheglass.com, which provides detailed lineup data for NBA games. The lineup data includes information such as player names, playing positions, playing time, and various statistics such as points, rebounds, and assists.

Data from Cleaningtheglass.com, downloaded in CSV form for the purposes of my analysis
<img width="496" alt="Screen Shot 2023-02-21 at 4 26 39 PM" src="https://user-images.githubusercontent.com/105028034/220472817-faed9a93-db25-4669-a7c3-1a9b24f7e693.png">

## Methodology

Methodology
The project began by exploring the lineup data and creating visualizations to gain insights into the nature of the data. I used R and the pandas library for data manipulation and cleaning. I created various graphs, including bar charts, scatter plots, and dot plots to visualize the relationships between different variables and identify any patterns.

Visualization examining lineups who played the most during the 2016-17 season
<img width="1087" alt="Screen Shot 2023-02-21 at 4 30 44 PM" src="https://user-images.githubusercontent.com/105028034/220473501-febd5f3c-9a4e-451a-be1e-bae09000660b.png">

Visualization examining lineups who had the best per-48 +/- during the 2016-17 season
<img width="1109" alt="Screen Shot 2023-02-21 at 4 31 37 PM" src="https://user-images.githubusercontent.com/105028034/220473648-dc04465e-bfb7-48a8-a8de-5dfda3403432.png">

Visualization examining lineups who had the worst per-48 +/- during the 2016-17 season
<img width="1067" alt="Screen Shot 2023-02-21 at 4 32 02 PM" src="https://user-images.githubusercontent.com/105028034/220473710-ff5f07b5-918c-479f-bcd3-f4f85b9085ad.png">

We also aimed to understand how lineup performance and their number of possessions was correlated, so I produced several visualizations examining this trend.

The first visualization examines each team's most effective lineup during the 2016-17 season
<img width="1102" alt="Screen Shot 2023-02-21 at 4 35 32 PM" src="https://user-images.githubusercontent.com/105028034/220474335-0d5a7f0c-11f2-40fc-b3e8-41419364bb6c.png">

The second visualization examines each team's least effective lineup during the 2016-17 season
<img width="1103" alt="Screen Shot 2023-02-21 at 4 36 15 PM" src="https://user-images.githubusercontent.com/105028034/220474441-fb57aedf-80bd-4d46-a9ab-dc4c74d91b1c.png">



I then used statistical models to understand the underlying factors that contribute to the success of a lineup. I used a logistic regression model to predict the probability that one lineup is better than another based on various factors such as playing positions, playing time, and statistics.

I evaluated the model's performance using various metrics, such as accuracy and Variance Difference. I also used feature importance plots to gain insights into which factors had the most significant impact on the model's predictions.

The standard deviation of the rating difference between the two lineups is given by the sum of the variances of the two random variables. More specifically, the variance of the difference of independent random variables is the sum of their variances. As the standard deviation is the square root of the variance, we can calculate the standard deviation of the rating difference between the two lineups.


## Results

The results of the analysis show that the difference in the ratings of the two lineups is essentially the same (0.00001 apart). Any variations can be attributed to two factors. Firstly, when conducting data cleaning, all possessions were generalized to take the league average of 14.8 seconds. In reality, the Atlanta Hawks took 14.3 seconds per possession. Secondly, the Mathletics dataset likely included playoffs, where the Hawks played six extra games.

Based on the analysis, the probability that the Tim Hardaway Jr. lineup is better than the Kent Bazemore lineup is 99.991%, according to both my analysis and Mathletics. This suggests that Mike Budenholzer, the former coach of the Hawks, may have made a mistake by playing this lineup so often and starting them for most of the season.

Mathletics' final analysis:

<img width="542" alt="Screen Shot 2023-02-21 at 4 47 30 PM" src="https://user-images.githubusercontent.com/105028034/220476292-08a582cc-fa47-4ee0-a738-6c39ca6532b8.png">

Versus my final analysis:

<img width="607" alt="Screen Shot 2023-02-21 at 4 48 01 PM" src="https://user-images.githubusercontent.com/105028034/220476356-36de7891-52c9-446f-b737-138ea7aeaa1e.png">

## Conclusion

In conclusion, this project demonstrates the potential of data analysis and statistical models in understanding the underlying factors that contribute to the success of a lineup in NBA games. By using various visualization techniques and statistical models, I was able to gain insights into the factors that contribute to a lineup's success and create a model that predicts the probability that one lineup is better than another. The insights gained from this project can be used to improve player performance and team strategy in the NBA.





