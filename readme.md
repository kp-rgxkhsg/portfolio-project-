# IPL Data Analysis Project

This project is a comprehensive analysis of the Indian Premier League (IPL) cricket data from 2008 to 2020. It combines **match-level** and **ball-by-ball** datasets in a **SQL database** and performs various queries to derive insights about matches, teams, players, and performance trends.

---

## Datasets

The project uses two main tables:

### 1. `ipl_matches`
| Column | Description |
|--------|-------------|
| id | Unique match ID |
| city | City where the match was played |
| date | Match date |
| player_of_match | Player awarded 'Player of the Match' |
| venue | Match venue |
| neutral_venue | 1 if neutral venue, else 0 |
| team1 | Team 1 |
| team2 | Team 2 |
| toss_winner | Team that won the toss |
| toss_decision | Bat or field first |
| winner | Match winner |
| result | Win type (runs/wickets) |
| result_margin | Margin of victory |
| eliminator | Eliminator match flag |
| method | D/L method if used |
| umpire1 | First umpire |
| umpire2 | Second umpire |

### 2. `ipl_ball_by_ball`
| Column | Description |
|--------|-------------|
| id | Unique ball-by-ball record ID |
| inning | Inning number |
| over | Over number |
| ball | Ball number |
| batsman | Batsman on strike |
| non_striker | Non-striker batsman |
| bowler | Bowler |
| batsman_runs | Runs scored by batsman on this ball |
| extra_runs | Extra runs (wide, no-ball, etc.) |
| total_runs | Total runs (batsman + extras) |
| non_boundary | 1 if not a boundary |
| is_wicket | 1 if wicket fell |
| dismissal_kind | How the batsman was dismissed |
| player_dismissed | Player dismissed (if any) |
| fielder | Fielder involved (if any) |
| extras_type | Type of extra run |
| batting_team | Batting team |
| bowling_team | Bowling team |

---

## Project Goal

The project demonstrates:

- How to structure and query relational data in SQL.
- Aggregations, joins, window functions, and filtering to get **KPIs**.
- Player and team performance trends.
- Useful insights for analytics and visualization in Python or Power BI.

---

## Example Queries

Some example queries executed:

1. Count total matches and balls.
2. Top 10 run scorers.
3. Top 10 wicket takers.
4. Most wins by team.
5. Most toss wins.
6. Matches won batting first vs second.
7. Highest individual score.
8. Highest partnership runs.
9. Team scoring highest in a single match.
10. Total sixes per season.
11. Player with most Player of the Match awards.
12. Average runs per over per team.
13. Total extras by type.
14. Most economical bowler.
15. Matches played per city.
16. Venue with most matches.
17. Player with most dismissals (fielder).
18. Highest margin of victory (runs).
19. Highest margin of victory (wickets).
20. Matches where D/L method was applied.
21. Total centuries scored.
22. Total half-centuries scored.
23. Player scoring fastest 50.
24. Player scoring fastest 100.
25. Count of matches per season.
26. Most frequent match result (win by runs/wickets).
27. Number of tied matches.
28. Player with most sixes.
29. Player with most fours.
30. Top bowling figures in a match.

> Full SQL script is included in `ipl_queries.sql`.

---

## How to Use

1. Import the datasets (`matches.csv` and `ball_by_ball.csv`) into a MySQL database called `ipl`.
2. Run the SQL script `ipl_queries.sql` to create all queries.
3. Explore or export results for Python/Pandas analysis or Power BI visualization.
4. Each query has comments explaining the purpose.

---

## Tech Stack

- **SQL**: MySQL / Workbench
- **Python**: Pandas, Numpy, Matplotlib, Seaborn
- **BI Tools**: Power BI (optional)
- **Version Control**: GitHub

---

## Author

Priyanshu Kumar Priy  
Data Analyst Portfolio
