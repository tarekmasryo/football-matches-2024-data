# ⚽ Football Matches 2024/2025 (Top 5 Leagues + Champions League)

**Author:** [Tarek Masryo](https://github.com/tarekmasryo) · [Kaggle](https://www.kaggle.com/datasets/tarekmasryo/football-matches-20242025-top-5-leagues)  
**Version:** v1.0 (2025-09-01)  

**License:**  
• Match data (via [football-data.org API](https://www.football-data.org/)) — **CC BY-NC 4.0 (Attribution–NonCommercial)**  

---

## TL;DR

> Clean football dataset: **1,941 matches** across **6 competitions**, with detailed scores, referees, teams, and derived features (goal difference, total goals, outcomes, points).  
>  
> - One CSV (`football_matches_2024_2025.csv`)  
> - Includes FT/HT breakdowns  
> - Pre-computed features for direct analysis  

---

## Why this dataset exists
Football data is often scattered across multiple APIs and formats.  
This dataset provides a **single, analysis-ready CSV** that you can load in seconds to explore team/league performance, simulate tables, or train ML models on match outcomes.

---

## What’s inside
**Main file — `football_matches_2024_2025.csv` (1 row per match)**  

**Columns (23):**
- Competition info: competition_code, competition_name, season, stage, matchday  
- Match details: match_id, date_utc, status, referee, referee_id  
- Teams: home_team_id, home_team, away_team_id, away_team  
- Scores: fulltime_home, fulltime_away, halftime_home, halftime_away  
- Derived features: goal_difference, total_goals, match_outcome, home_points, away_points  

---

## Data Dictionary

| Column            | Description                                       |
|-------------------|---------------------------------------------------|
| competition_code  | Short code for competition (e.g., PL, CL)         |
| competition_name  | Full competition name                             |
| season            | Season year (2024/2025)                           |
| stage             | Competition stage (e.g., REGULAR_SEASON, GROUP)   |
| matchday          | Matchday number                                   |
| match_id          | Unique match identifier                           |
| date_utc          | Match date (UTC)                                  |
| status            | Match status (FINISHED, SCHEDULED, etc.)          |
| referee           | Referee name                                      |
| referee_id        | Referee identifier                                |
| home_team_id      | Home team ID                                      |
| home_team         | Home team name                                    |
| away_team_id      | Away team ID                                      |
| away_team         | Away team name                                    |
| fulltime_home     | Goals scored by home team (full-time)             |
| fulltime_away     | Goals scored by away team (full-time)             |
| halftime_home     | Goals scored by home team (half-time)             |
| halftime_away     | Goals scored by away team (half-time)             |
| goal_difference   | Goal difference (home - away)                     |
| total_goals       | Total goals in match                              |
| match_outcome     | Outcome (Home Win / Away Win / Draw)              |
| home_points       | Points for home team (3 win / 1 draw / 0 loss)    |
| away_points       | Points for away team (3 win / 1 draw / 0 loss)    |

---

## Quick start (pandas)

```python
import pandas as pd

df = pd.read_csv("football_matches_2024_2025.csv")
print(df.shape)

# Average goals per match
avg_goals = df["total_goals"].mean()
print("Avg goals per match:", round(avg_goals, 2))

# Home win rate
home_win_rate = (df["match_outcome"] == "Home Win").mean()
print("Home win rate:", round(home_win_rate, 3))
```

---

## 💡 Use Cases
- Predict match results or total goals  
- Build dashboards for league/club performance  
- Simulate league tables using outcomes and points  
- Analyze trends: goal averages, draw frequencies, home vs away win rates  
- Educational projects in **sports analytics** and **machine learning**  

---

## 📝 Changelog
- **v1.0 (2025-09-01):** Added 1,941 matches from 6 major competitions with derived features (goal diff, total goals, outcome, points).  

---

## 📜 License & Attribution
- Data collected via the [football-data.org API](https://www.football-data.org/)  
- Pre-processed and structured by **Tarek Elmasry**  
- Licensed under **CC BY-NC 4.0 (Attribution–NonCommercial)** → Free for open research & educational use  
- Commercial use is **not permitted**  
