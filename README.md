# MIDS-207-Final-Project

## Data

The data was sourced from Kaggle at https://www.kaggle.com/datasets/erichqiu/nba-odds-and-scores/data. This Kaggle page contains a data storage structure that is organized with three data files per season from the 2012-13 season to the 2018-19 season. The Kaggle page states that the data was compiled from "various sources." The three data files available for each season are detailed below:

1. raw_scores.txt: Contains information by team and game on points per quarter, points per overtime, total points/rebounds/assists/turnovers, FG%, FT%, FG3%. Each game has a unique ID, each team has a unique ID, and the game date is indicated. This file only contains regular season games.
2. vegas.txt: Contains betting odds from five sports books on three bets (moneyline, spread, and over/under), as well as averages across the five sports books, for regular season games.
3. vegas_playoff.txt: Contains the same information as vegas.txt but for playoff games. Given that the Raw Scores data does not have playoff games, the information from this file type is excluded from our analysis.
