# NBA player improvement prediction
## Background
National Basketball Association (NBA) is the best basketball league in the world with millions of fans worldwide. How players on a team perform is the most important factor that determines which team wins the championship. Players’ pay are largely based on their past performances. However, player performance change from season to season. Each year there are a number of players who improve dramatically over last year. Those players bring a lot of value, both competitively and economically, to the teams they belong to. Their importance is widely recognized by the NBA in that the player who improved the most over last season is awarded Most Improved Player Award. Therefore, it is advantageous for teams to accurately predict whether and how much a player will improve in the next season. For example, this information can be used to target players to acquire in trades or signings.<br>
## Problem statement
Use player performance data, biography data, and draft data to predict whether and how much a player will improve the next season.
## Data
Player performance data of every season since 1980 and player draft positions were used to build predictive models.<br>
Data were obtained from two Kaggle datasets, and also scrapped from [basketball-reference.com](basketball-reference.com)<br>
Data were combined and cleaned. In total, there were 13,378 samples and 24 selected independent features.
## Findings
Through exploratory data analysis, I found several factors such as age, games played, minutes played, last season's improvement, etc. that had significant impact on player improvement next season.<br>
I built multiple regression models using a modified approach in which weights were assigned to samples to compensate for their low representation in the dataset. Support vector machines model performed the best among all models, and reduced the prediction error by ~26% compared to the benchmark model.<br>
I also built multiple classification models. Voting model preformed the best and achieved ~67.5% accuracy in predicting whether a player will improve or not.
## File structure
1. Raw data can be found in data/raw/
2. Cleaned and modified data(with engineered features) can be found in data/
3. **Code and figures are in Jupyter Notebook form and can be found in notebooks/**
4. **Final report can be found in Final_report.pdf**
5. Presentation can be found in Presentation.pdf
<br>
Suggestions or discussions are welcome.
