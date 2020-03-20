# Predicting the NCAA Basketball Tournament
This repository holds the files from my final project in the General Assembly Part-Time Data Science course. My project was focused on predicting the results of the NCAA Men's Basketball Tournament alongside the Kaggle Competition. In the 'Notebooks' folder, you can find my original exploratory analysis, data wrangling, and modeling work. The 'raw data' folder contains the original data set that I started with. The 'derived data' folder contains the data sets that came out of the notebooks along the way. There is also a PDF of my final presentation.

#### -- Project Status: Completed

## Project Details
The purpose of this project is to create a predictive model to apply to basketball matchups and use that model to create a bracket for the NCAA's Men's Basketball Tournament.

### Methods Used
* Exploratory Analysis
* Data Visualization
* Predictive Modeling

### Technologies
* Python
* jupyter notebooks
* pandas, numpy
* matplotlib
* sklearn
  * Logistic Regression
  * Random Forest
  * XGBoost

### Project Problem and Hypothesis:
* Use historical data and team statistics to predict the outcome of the 2016 NCAA Men’s Basketball Tournament (without peeking)
* This is a classification problem: win or lose for a given matchup
* Win probabilities calculated for every potential matchup then used to create bracket
* Goal is to predict more games than by using seed alone

### Feature Creation:
* Using win and loss records, iterate through entire data set to create ELO scores for each team
* Using season level team stats, derive offensive and defensive efficiency stats
* Merge data, take differences between both teams to create feature set for modeling

### Modeling:
* LogisticRegression
* XGBClassifier
* DecisionTreeClassifier
* Random Forest

### Results:  
The Logistic Regression proved to have the best test score and was used for the final bracket prediction. The model ended up with 48 correctly predicted games in the tournament which beat out the "chalk bracket" which had 42 correctly predicted games. It does do better this time, but with so much variance in the college basketball tournament I wouldn't put my life savings on the results of the model.
