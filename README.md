# Nba-Mvp-Prediction-data-analysis-and-model
* on resume. I like basketball, I like data analysis. So why not combine the two?  This is a project I made that takes an NBA stats dataset from Kaggle and uses it to find the correlations between a players season and their Mvp votes 


*to run this you will have to download this dataset from kaggle: https://www.kaggle.com/datasets/robertsunderhaft/nba-player-season-statistics-with-mvp-win-share

Heres how it works: 

First, we must import the dataset which will be using, which is a dataset containing NBA player stats from the 1982-2021 season.

Now we have a table of the stats of every single NBA player's individual season. We can create a True/False column titled "mvp" based on if the player recieved the highest 
amount of award shares (the percentage of MVP votes) in their season.

We need to add an MVP column based on the player by season, with the most Award Shares (MVP vote percentage). 1 iff all 1st place, 0 of no votes period.

Then we narrow Dataset by Setting Guidlines:
- All MVPs must have played more than 20 games
- Must have averaged more than 10 minutes a game
- Scored more than 5 pts per game
we can do this because anyone who does not qualify will historically never even get considered for a vote

we can model different stats and their correlation to winning MVP
First, looking at Value Over Replacement (VORP) to Award Shares
Looking at a specific players stats in a Radar Chart, in this case, the MVP Nikola Jokic (2021-2023 season)

we get the top 20 factors correlated with the MVP variable
Create a new correlation matrix for these factors
[image](https://github.com/user-attachments/assets/5511a61f-4c21-4f0e-9566-1667c2904155)

now we add Season, Player, and Award Share data back for the purpose of training
The data will be trained on the data from NBA seasons 1982-2021 and will predict the 2022 MVP voting

we use a Mean Squared Error to test how accurate our model is, a lower score is preferable
output: 0.004953966787615027
we then Backtest model for all years

Do same for RandomnForrest Reggresion model
Mean squared Error: 0.0015574997776201462

- I would like to acknowledge DataScientist David Yoo. He is a data scientist that tackled a similar project and has a great medium article about it
https://towardsdatascience.com/predicting-the-next-nba-mvp-using-machine-learning-62615bfcff75
