# ⚽ Football Matches 2024/2025 (Top 5 Leagues + Champions League)

**Author:** [Tarek Masryo](https://github.com/tarekmasryo) · [Kaggle](https://www.kaggle.com/datasets/tarekmasryo/football-matches-20242025-top-5-leagues)  
**Version:** v1.0 (2025-09-01)  

**License:**  
• Match data (via [football-data.org API](https://www.football-data.org/)) — **CC BY-NC 4.0 (Attribution–NonCommercial)**  

---

## TL;DR

> Clean football dataset: **1,941 matches** across **6 competitions**, with detailed scores, venues, referees, and derived features (goal diff, total goals, outcomes, points).  
>  
> - One CSV (`football_matches_2024_2025.csv`)  
> - Includes FT/HT/ET/Pen breakdowns  
> - Pre-computed features for direct analysis  

---

## Why this dataset exists
Football data is often scattered across multiple APIs and formats.  
This dataset gives you a **single, analysis-ready CSV** that you can load in seconds to explore team/league performance, simulate tables, or train ML models on match outcomes.

---

## What’s inside
**Main file — `football_matches_2024_2025.csv` (1 row per match)**  

**Columns (24):**
- Competition, season, stage, group, matchday  
- Teams (home & away)  
- Scores: FT, HT, ET, Penalties  
- Date (UTC + local), venue, referee  
- Derived features: goal difference, total goals, outcome, points (home/away)  

---

## Data Dictionary

| Column        | Description                               |
|---------------|-------------------------------------------|
| competition   | Competition name (e.g., Premier League)   |
| season        | Season year (2024/2025)                   |
| stage         | Competition stage (Group/Knockout)        |
| group         | Group name (if applicable)                |
| matchday      | Matchday number                           |
| date_utc      | Match date (UTC)                          |
| date_local    | Local date                                |
| venue         | Stadium name                              |
| referee       | Referee name                              |
| home_team     | Home team                                 |
| away_team     | Away team                                 |
| home_ft       | Home goals (full-time)                    |
| away_ft       | Away goals (full-time)                    |
| home_ht       | Home goals (half-time)                    |
| away_ht       | Away goals (half-time)                    |
| home_et       | Home goals (extra-time)                   |
| away_et       | Away goals (extra-time)                   |
| home_pen      | Penalties scored by home team             |
| away_pen      | Penalties scored by away team             |
| goal_diff     | Goal difference                           |
| total_goals   | Total goals in match                      |
| outcome       | Match outcome (W/D/L for home team)       |
| points_home   | Points for home team                      |
| points_away   | Points for away team                      |

---

## Quick start (pandas)

```python
import pandas as pd

df = pd.read_csv("football_matches_2024_2025.csv")
print(df.shape)

# Average goals per match
avg_goals = df["total_goals"].mean()
print("Avg goals per match:", round(avg_goals, 2))

# Win rate of home teams
home_win_rate = (df["outcome"] == "W").mean()
print("Home win rate:", round(home_win_rate, 3))
```

---

## 💡 Use Cases
- Predict match results or total goals  
- Build dashboards for league/club performance  
- Simulate league tables using outcomes and points  
- Analyze trends: goal averages, draw frequencies, win rates  
- Educational projects in **sports analytics** and **machine learning**  

---

## 📝 Changelog
- **v1.0 (2025-09-01):** Added 1,941 matches from 6 major competitions with derived features (goal diff, total goals, outcome, points).  

---

## 📜 License & Attribution
- Data collected via the [football-data.org API](https://www.football-data.org/)  
- Licensed under **CC BY-NC 4.0 (Attribution–NonCommercial)** → Free for open research & educational use  
- Commercial use is **not permitted**  
