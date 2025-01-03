# Movies Project

## Files & Links

Kaggle Link: [Movies (IMDb, Earnings and more)](https://www.kaggle.com/datasets/delfinaoliva/movies)<br>
Tableau Link: <a href= "https://public.tableau.com/views/MoviesDashboard_17334967093890/Movies_Dashboard?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link"> Movies Dashboard </a><br>
Dataset file Link: <br>

## Project Objectives

I created a comprehensive project using tools as Excel and Python to treat the data, and Tableau to report and visualize it. The project objectives are as follow:

- Analyse a list of movies and determine which __Genre__ is most profitable, have look at the data related to __Actors__ and __Directors__. 
- Check any trend based on movies __released per year__ and highlight the ones with higher __IMDb Score__.
- Understand if we can predict the __Box Office__ results. For that, I will investigate the relationship between variables and develop a __predictive model__ to forecast the __Box Office__ results.

## Questions (KPIs)

1. Are the movies Box Office related to any of the other variables?
2. Having a bigger budget influences the Box Office?
3. Are the movies with more Awards more profitable?
4. Which genre is more profitable?
5. Which genre is more likely to get awards?

## Process

- Verified data for any duplicates and missing values.
- Made sure all data is consistant in terms of data types, data format and values.
- Created a new dataset with only __Actors__ information to join all the 3 variables into 1.
- Created new variables to add value to the dataset.
- Created __visual representation__ for multiple variables
- Did some Statistical Analysis using __T-Test__ and __Chi-Square Test__ techniques.
- Created 2 ML models (__Regression__ & __Classification__)
- Ran a __Features Importance__ technique to confirm all the Statistical and ML results.

## Dashboard

![Screenshot 2025-01-03 200550](https://github.com/user-attachments/assets/73b7a089-72d7-49c5-98ad-62aeae1383f7)

## Project Insights 

- The dataset has a total of 3907 movies (After cleaning duplicated)
- We only have movies from 1929 to 2016
- 68 movies did not have profit nor loss in earnings and 985 had a loss. That means 2,854 movies had profit
- 88% of the movies were released after 1990
- 28.6% of the movies have a budget between 20 and 50 Millions
- 2006 is the year with more movies released
- The biggest correlation happens between the __Box Office__ and __Earnings__, which means movies with higher __Box Office__ tend to be more profitable
- Movies with higher __Budget__ tend to have higher __Box Office__ and __Earnings__ (__Correlation__ and __Chi-Square Test__)
- The more nominations a movie has, higher is the chance to win an award
- Nominations and Awards are not related to the movie __Running time__, __Box Office__, __Earnings__ and __IMDb Score__
- Action is the most profitable __Genre__ with a total of $108.21B in __Earnings__. That makes an average of 114.87 millions per movie
- Even though __Action__ is the most profitable Genre, __Comedy__ is the Genre with more movies released (1002)
- __Drama__ is the Genre with more Nominations/Awards 
- __Action__, __Animation__ and __Adventure__ are the Genres generating more movies with higher Box Offices
- The Actor with more presences in movies is __Robert the Niro__ with a total of __53__ presences
- With the __T-Test__ we verified the movies with awards have higher __IMDb Score__
- In the end created a Random Forest Regressor model that confirmed all my previous analysis, with a result of 0.94 in R2, the model explains most of the variability
- To finalize the entire analysis, I ran a Features Importance technique based on the Random Forest Regressor model and concluded the variable __Earnings__ is the most important one when it comes to predict the __Box Office__

## Final Conclusion

Movies with higher __Budget__ tend to have an higher __Box Office__ and consequently are more profitable, which is pretty obvious, however, having higher __Box Office__ and __Earnings__ does not mean the movie will get more Golden Globes nominations and win more awards and that is surprising.
__Running time__ is also not related to Nominations and Awards, proving quality always stands over quantity.
Even though the results were easily predicted, it was really interesting to analyse this dataset and 
