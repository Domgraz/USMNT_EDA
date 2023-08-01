# USMNT_analysis

## Table of Contents:
* [General info](#general-info)
* [Techologies and Libraries](#technologies-and-libraries)
* [Data Source](#data-source)
* [Data Explanation](#data-explanation)
* [Calculated Fields](#calculated-fields)
* [Key Questions](#key-questions)

## General Info
With the rise of soccer in the US and many tournaments coming to the states over the next few years, culminating in the 2026 World Cup I wanted to examine the player pool for the US Men's National Team (USMNT) for the future. 


## Technologies and Libraries

* Python 3.9
* Pandas
* Matplotlib
* DuckDb
* Sci-Kit Learn


## Data Source
 The data that is included has been taken from Transfermarkt's USMNT extended squad page and may not currently be up to date.


## Data Explanation
Data from csv
* Player - USMNT player's first and last name
* Position - position on field played as listed
* Birthday - player's birthday in month-day-year
* Age - int of players age
* Club - current club the player plays for
* League - league the current club is affiliated with
* Market Value - current market value for player in int
* Highest Market Value - historical highest market value of player in int
* League Appearances - number of appearances for club in current season in int
* Goals Conceded - goals allowed for goalkeepers in int
* Clean Sheet - count of games a goal isn't conceded for the goalkeeper in int
* Yellow Cards - count of yelow cards awarded for player in int
* Red Cards - count of red cards awarded for player in int
* Starting Eleven % - percentage of games player started in int
* Club Minutes % - percentage of total minutes player has played for the club in int
* Club Goals - count of club goals for the season for the player in int
* Club Assists - count of club assists for the season in int
* Goal Participation % - percentage of involvement in goals for club in int
* Total Minutes - minutes played for club during the season in int
* US Caps - count of official USMNT appearances for player in int
* US Goals - count of historical  national team goals for player in int
* US Assists - count of historical national team assists for player in int
* US Total Minutes - historical total minutes player with USMNT for player

## Calculated Fields
These fields establish whats known as G/A p90 for soccer which is a player's goals and assists per 90 minutes played which is regular time in a game.

* Club GA = (Club Goals + Club Assists) / (Total Minutes / 90)
* US GA = (US Goals + US Assists) / (US Total Minutes / 90)

## Key Questions
* Who are the most valuable players in the player pool?
* Who are the youngest players to have a cap?
* Which league has the most USMNT players in it?
* Which league has the most value in terms of USMNT players?
* Who are the players with the best G/A per 90 for their club?
* Who are the players with the best G/A per 90 for the national team?
* Whos value is still on the rise vs falling?


        