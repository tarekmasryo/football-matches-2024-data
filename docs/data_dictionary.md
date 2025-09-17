# Data Dictionary — Football Matches 2024/2025

| Column            | Type   | Description                                    |
|-------------------|--------|------------------------------------------------|
| competition_code  | str    | Short code for competition (e.g., PL, CL)      |
| competition_name  | str    | Full competition name                          |
| season            | str    | Season year (2024/2025)                        |
| stage             | str    | Competition stage (e.g., REGULAR_SEASON)       |
| matchday          | int    | Matchday number                                |
| match_id          | int    | Unique match identifier                        |
| date_utc          | str    | Match date and time (UTC, ISO format)          |
| status            | str    | Match status (e.g., FINISHED, SCHEDULED)       |
| referee           | str    | Referee name                                   |
| referee_id        | int    | Referee identifier                             |
| home_team_id      | int    | Home team ID                                   |
| home_team         | str    | Home team name                                 |
| away_team_id      | int    | Away team ID                                   |
| away_team         | str    | Away team name                                 |
| fulltime_home     | int    | Home goals (full-time)                         |
| fulltime_away     | int    | Away goals (full-time)                         |
| halftime_home     | int    | Home goals (half-time)                         |
| halftime_away     | int    | Away goals (half-time)                         |
| goal_difference   | int    | Goal difference (home - away)                  |
| total_goals       | int    | Total goals scored in the match                |
| match_outcome     | str    | Outcome (Home Win / Away Win / Draw)           |
| home_points       | int    | Points awarded to home team (3/1/0)            |
| away_points       | int    | Points awarded to away team (3/1/0)            |
