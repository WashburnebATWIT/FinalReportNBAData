# Exploring NBA Draft Picks (1989-2021): A Comprehensive Analysis

## Introduction

My project delves into the NBA Draft picks spanning from 1989 to 2021, aiming to address specific research questions that shed light on the performance and impact of players based on their draft positions. As both a fan of the NBA and a data science major, the project was particularly interesting; in a sense, I was providing similar analysis that front offices/scouting departments produce to prepare for drafting new players each year. The primary research questions include: 
1) How do first overall picks compare in performance metrics to other picks?
2) How do performance metrics differ by decade?
3) What colleges send the most players to the NBA and how do they influence a player's draft position?
4) What are the major contributors to a player's win shares?
5) Can a basic predictive model be established for a player's win shares based on their overall pick?

## Selection of Data
### Information

The dataset comprises comprehensive information on NBA Draft picks from 1989 to 2021, encompassing details such as the year, overall pick, and player-specific data. The source of the dataset is from basketball reference – one of the most reputable and comprehensive sources of NBA data. Furthermore, the specific data set was found on Kaggle and has a useability rating of 10.00 – confirming completeness, credibility, and compatibility. In terms of characteristics, the data set includes information about performance metrics, college affiliations, and draft pick details.

![Information in Data](graph/DataColumns.png)

### Data Cleaning 

In terms of any munging, imputation, or feature engineering, there was specific cleaning necessary to work with the data. Firstly, I had to handle null/missing data: for the numerical values, I changed all missing data to 0 (as the player never played in the NBA), and for the object values I simply dropped all missing data (as any player who did not go to college or did not play on a team would inherently provide no use to the data analysis). Furthermore, I added a data column for decade (based on when a player was drafted), and filtered data such as separating #1 overall picks from all other picks. 
