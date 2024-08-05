 <p align="center">
# Predicting NBA Game Point Spread
</p>


# MIDS-207-Final-Project

## Purpose

This project builds a pipeline to build models in an ML framework to predict game spread for NBA games. The baseline presentation for this project is located in the 'Baseline PPT: Predicting NBA Game Point Spread.pptx' file. The final presentation for this project is located in the [INSERT] file. Both presentations contain a more detailed overview of the motivation behind this project.

## Data

The data was sourced from Kaggle at https://www.kaggle.com/datasets/erichqiu/nba-odds-and-scores/data. This Kaggle page contains a data storage structure that is organized with three data files per season from the 2012-13 season to the 2018-19 season. The Kaggle page states that the data was compiled from "various sources." The three data files available for each season are detailed below:

1. 'raw_scores.txt': Contains information by team and game on points per quarter, points per overtime, total points/rebounds/assists/turnovers, FG%, FT%, FG3%. Each game has a unique ID, each team has a unique ID, and the game date is indicated. This file only contains regular season games.
2. 'vegas.txt': Contains betting odds by team and game from five sports books on three bets (moneyline, spread, and over/under), as well as averages across the five sports books, for regular season games. Each game has a unique ID and each team has a unique ID matching to the IDs in the Raw Scores data.
3. 'vegas_playoff.txt': Contains the same information as vegas.txt but for playoff games. Given that the Raw Scores data does not have playoff games, the information from this file type is excluded from our analysis.

Your data directory requires a sub-directory named 'NBA data - raw' containing sub-directories for each season named '2012-13' to '2018-19'.

## Pre-processing and EDA

We perform the data pre-processing and EDA in the 'Data_Processing.ipynb' file. This notebook compiles a game-level database of home and away team performances in the previous 5, 10, and 20 games using the 'raw_scores.txt' and 'vegas.txt' files. 

Game location is available from the Vegas data. 

Team performance features include win rate, average total points/rebounds/assists/turnovers, and average FG%/FT%/FG3% calculated using the Raw Scores data. These features are normalized by season and are used to make predictions on home team point spread for each game. These predictions are benchmarked against the actual game spread available in both data and the average home game spread available in the Vegas data.

Your data directory requires a sub-directory named 'NBA data - processed' in which the compiled training, validation, and test features and labels are exported.

## Modeling

[Specify where experiments are performed]. [Specify where final model is deployed].

## Results

## Contributions
