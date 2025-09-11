# Data Dictionary — Football Matches 2024/2025

| Column        | Type | Description |
|---------------|------|-------------|
| competition   | str  | Name of competition (e.g., Premier League) |
| season        | str  | Season year (2024/2025) |
| stage         | str  | Competition stage (e.g., Group, Knockout) |
| group         | str  | Group name (if applicable) |
| matchday      | int  | Matchday number |
| date_utc      | date | Match date (UTC) |
| date_local    | date | Match date (local time, example) |
| venue         | str  | Stadium/venue name |
| referee       | str  | Referee name |
| home_team     | str  | Home team name |
| away_team     | str  | Away team name |
| home_ft       | int  | Home goals (full-time) |
| away_ft       | int  | Away goals (full-time) |
| home_ht       | int  | Home goals (half-time) |
| away_ht       | int  | Away goals (half-time) |
| home_et       | int  | Home goals (extra-time) |
| away_et       | int  | Away goals (extra-time) |
| home_pen      | int  | Home penalties scored |
| away_pen      | int  | Away penalties scored |
| goal_diff     | int  | Goal difference |
| total_goals   | int  | Sum of home and away goals |
| outcome       | str  | W/D/L outcome for home team |
| points_home   | int  | Points awarded to home team |
| points_away   | int  | Points awarded to away team |
