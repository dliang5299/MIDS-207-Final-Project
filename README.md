# MIDS-207-Final-Project

## Purpose

## Data

The data was sourced from Kaggle at https://www.kaggle.com/datasets/erichqiu/nba-odds-and-scores/data. This Kaggle page contains a data storage structure that is organized with three data files per season from the 2012-13 season to the 2018-19 season. The Kaggle page states that the data was compiled from "various sources." The three data files available for each season are detailed below:

1. raw_scores.txt: Contains information by team and game on points per quarter, points per overtime, total points/rebounds/assists/turnovers, FG%, FT%, FG3%. Each game has a unique ID, each team has a unique ID, and the game date is indicated. This file only contains regular season games.
2. vegas.txt: Contains betting odds by team and game from five sports books on three bets (moneyline, spread, and over/under), as well as averages across the five sports books, for regular season games. Each game has a unique ID and each team has a unique ID matching to the IDs in the Raw Scores data.
3. vegas_playoff.txt: Contains the same information as vegas.txt but for playoff games. Given that the Raw Scores data does not have playoff games, the information from this file type is excluded from our analysis.

## Pre-processing

We perform the data pre-processing in [FILL IN HERE]. This [script/notebook] compiles a game-level database of home and away team performances in the previous 5, 10, and 20 games using the raw_scores.txt and vegas.txt files. Game location is available from the Vegas data. Team performance metrics include win rate, average total points/rebounds/assists/turnovers, and average FG%/FT%/FG3% calculated using the Raw Scores data. These features are normalized by season and are used to make predictions on home team point spread for each game. These predictions are benchmarked against the actual game spread available in both data and the average home game spread available in the Vegas data.

## Modeling

[Specify where experiments are performed]. [Specify where final model is deployed].

## Results

## Contributions
