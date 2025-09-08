# ⚽ Football Matches 2024/2025 Dataset

**Author:** [Tarek Masryo](https://github.com/tarekmasryo) · [Kaggle](https://www.kaggle.com/datasets/tarekmasryo/football-matches-20242025-top-5-leagues)  
**Version:** v1.0 (2025-09-01)  
**License:** CC0 (Public Domain, for open research & educational use)  

---

## 📌 TL;DR
Clean and structured dataset with **1,941 matches** from the 2024/2025 season:  
- 6 top competitions (Premier League, La Liga, Serie A, Bundesliga, Ligue 1, Champions League)  
- Match details: results, dates, venues, referees  
- Score breakdowns: full-time, half-time, extra-time, penalties  
- Derived features: goal difference, total goals, outcomes, points  

---

## ⚙️ Context
This dataset brings together all matches from the **2024/2025 season** across six of the biggest competitions in world football:

- Premier League (England)  
- La Liga (Spain)  
- Serie A (Italy)  
- Bundesliga (Germany)  
- Ligue 1 (France)  
- UEFA Champions League (Europe)  

It contains **1,941 matches** with structured fields, making it simple to explore results, build dashboards, or create machine learning models.

---

## 📂 File Included
- `football_matches_2024_2025.csv`  

Each row in the dataset represents a single match and includes:  
- Competition, season, stage, group, matchday  
- Teams (home & away)  
- Date (UTC + local time example)  
- Venue & referee  
- Scores: full-time, half-time, extra-time, penalties  

**Derived features:**  
- Goal difference  
- Total goals  
- Match outcome (Win/Draw/Loss)  
- Points awarded (3/1/0)  

---

## 🗄️ Data Dictionary

| Column            | Type   | Description                            |
|-------------------|--------|----------------------------------------|
| competition       | str    | Name of competition (e.g., Premier League) |
| season            | str    | Season year (2024/2025)                |
| stage             | str    | Competition stage (e.g., Group, Knockout) |
| group             | str    | Group name (if applicable)             |
| matchday          | int    | Matchday number                        |
| date_utc          | date   | Match date (UTC)                       |
| date_local        | date   | Match date (local time, example)       |
| venue             | str    | Stadium/venue name                     |
| referee           | str    | Referee name                           |
| home_team         | str    | Home team name                         |
| away_team         | str    | Away team name                         |
| home_ft           | int    | Home goals (full-time)                 |
| away_ft           | int    | Away goals (full-time)                 |
| home_ht           | int    | Home goals (half-time)                 |
| away_ht           | int    | Away goals (half-time)                 |
| home_et           | int    | Home goals (extra-time)                |
| away_et           | int    | Away goals (extra-time)                |
| home_pen          | int    | Home penalties scored                  |
| away_pen          | int    | Away penalties scored                  |
| goal_diff         | int    | Goal difference                        |
| total_goals       | int    | Sum of home and away goals             |
| outcome           | str    | W/D/L outcome for home team            |
| points_home       | int    | Points awarded to home team            |
| points_away       | int    | Points awarded to away team            |

---

## 💡 Inspiration
- Predict match results or total goals  
- Create visualizations and dashboards for league performance  
- Simulate league tables using points and outcomes  
- Explore trends across leagues, such as average goals or frequency of draws  
- Use as a foundation for football analytics or ML projects  

---

## 📜 License & Attribution
- Data collected via **football-data.org API**  
- Licensed under **CC0: Public Domain** → free for open research and educational use  
- Commercial use is **not permitted**
