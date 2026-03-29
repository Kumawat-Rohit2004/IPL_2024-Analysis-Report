# 🏏 IPL 2024 Season Analysis — Power BI Dashboard

> A comprehensive, interactive Power BI report covering all **74 matches**, **10 teams**, and **17,053 ball-by-ball deliveries** of the Indian Premier League 2024 season.

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Datasets](#-datasets)
- [Dashboard Features](#-dashboard-features)
- [Key Insights](#-key-insights)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Repository Structure](#-repository-structure)
- [License](#-license)

---

## 📌 Project Overview

This project transforms raw IPL 2024 cricket data into an interactive Power BI dashboard that enables fans, analysts, and enthusiasts to explore the season from multiple perspectives — from team win records down to individual ball-by-ball delivery patterns.

| Metric | Value |
|---|---|
| Total Matches | 74 |
| Total Deliveries | 17,053 |
| Total Runs (off bat) | 24,657 |
| Total Wickets | 883 |
| Teams | 10 |
| Venues | 10 |
| Datasets Used | 4 |

---

## 🗃️ Datasets

Four CSV files are used as data sources for this report:

### `ipl_2024_deliveries.csv` — 17,053 rows
Ball-by-ball delivery data for every match in the season.

| Column | Description |
|---|---|
| `match_id`, `season`, `match_no` | Match identifiers |
| `date`, `venue` | Match date and ground |
| `batting_team`, `bowling_team` | Teams involved |
| `innings`, `over` | Innings and over number |
| `striker`, `bowler` | Player names |
| `runs_of_bat`, `extras` | Runs scored |
| `wide`, `legbyes`, `byes`, `noballs` | Extra type breakdown |
| `wicket`, `wicket_type` | Dismissal info |
| `player_dismissed`, `fielder` | Dismissal details |

---

### `ipl2024_Matches_AutoRecovered_.csv` — 74 rows
Match-level summary with scores, results, toss details, and player awards.

| Column | Description |
|---|---|
| `id`, `date` | Match identifier and date |
| `team1`, `team2` | Competing teams |
| `toss_winner`, `decision` | Toss result and choice (Bat/Field) |
| `first_score`, `first_wkts` | First innings score and wickets |
| `second_score`, `second_wkts` | Second innings score and wickets |
| `winner`, `winning_margin` | Match result |
| `player_of_the_match` | POTM award |
| `most_runs`, `most_wkts` | Top performer each match |

---

### `ipl_players.csv`
Squad lists for all 10 IPL 2024 franchises, with one column per team.

**Teams covered:** CSK · DC · GT · KKR · LSG · MI · PBKS · RCB · RR · SRH

---

### `ipl_teams_owner.csv` — 10 rows
Franchise ownership and captaincy details.

| Column | Description |
|---|---|
| `Owner Name` | Franchise owner(s) |
| `Team Name` | Full team name |
| `Team Captain` | Captain for IPL 2024 |

---

## 📊 Dashboard Features

The `IPL_2024_Analysis.pbix` report includes the following pages and visuals:

- **Team Performance Overview** — season win/loss records across all 10 franchises
- **Batting Leaderboard** — top run scorers with runs, strike rates, and boundary stats
- **Bowling Leaderboard** — top wicket takers with wickets, economy, and bowling type
- **Ball-by-Ball Analysis** — over-by-over run flow and wicket fall using the full delivery dataset
- **Toss & Decision Analysis** — win rates split by toss choice (bat vs. field)
- **Player of the Match Tracker** — most impactful players across the tournament
- **Venue Breakdown** — scoring trends and results across all 10 stadiums
- **Team & Franchise Info** — ownership, captains, and squad context for all teams

---

## 🏆 Key Insights

### Team Win Tally

| Team | Wins | Notes |
|---|---|---|
| 🥇 Kolkata Knight Riders | 11 | **IPL 2024 Champions** |
| Rajasthan Royals | 9 | Runners-up |
| Sunrisers Hyderabad | 9 | |
| Chennai Super Kings | 7 | |
| Royal Challengers Bengaluru | 7 | |
| Lucknow Super Giants | 7 | |
| Delhi Capitals | 7 | |
| Punjab Kings | 5 | |
| Gujarat Titans | 5 | |
| Mumbai Indians | 4 | |

> 3 matches were abandoned due to rain/weather.

---

### 🏏 Top Run Scorers

| Rank | Batsman | Runs |
|---|---|---|
| 1 | Virat Kohli | 741 |
| 2 | Ruturaj Gaikwad | 583 |
| 3 | Riyan Parag | 573 |
| 4 | Travis Head | 567 |
| 5 | Sanju Samson | 531 |
| 6 | Sai Sudharsan | 527 |
| 7 | KL Rahul | 520 |
| 8 | Nicholas Pooran | 499 |
| 9 | Sunil Narine | 488 |
| 10 | Abhishek Sharma | 484 |

---

### 🎯 Top Wicket Takers

| Rank | Bowler | Wickets |
|---|---|---|
| 1 | Harshal Patel | 30 |
| 2 | Avesh Khan | 22 |
| 2 | Mukesh Kumar | 22 |
| 4 | Varun Chakaravarthy | 21 |
| 4 | Jasprit Bumrah | 21 |
| 6 | Harshit Rana | 20 |
| 6 | T Natarajan | 20 |
| 6 | Mitchell Starc | 20 |
| 6 | Arshdeep Singh | 20 |
| 10 | Yuzvendra Chahal | 19 |

---

### ⭐ Player of the Match Leaders

| Player | Awards |
|---|---|
| Abhishek Sharma | 3 |
| Sunil Narine | 3 |
| Travis Head | 3 |
| Sam Curran | 2 |
| Andre Russell | 2 |
| Sanju Samson | 2 |
| Virat Kohli | 2 |
| Mayank Yadav | 2 |
| Jos Buttler | 2 |
| Ravindra Jadeja | 2 |

---

### 🪙 Toss Trends

- **73% of teams elected to field first** after winning the toss (52 out of 71 decided matches)
- Only 19 teams chose to bat first — reflecting the strong T20 preference for chasing

---

### 🏟️ Venues

| Stadium | City |
|---|---|
| MA Chidambaram Stadium | Chennai |
| Narendra Modi Stadium | Ahmedabad |
| Ekana Cricket Stadium | Lucknow |
| M. Chinnaswamy Stadium | Bengaluru |
| Wankhede Stadium | Mumbai |
| Eden Gardens | Kolkata |
| Rajiv Gandhi International Stadium | Hyderabad |
| Arun Jaitley Stadium | Delhi |
| Sawai Mansingh Stadium | Jaipur |
| MYSICS, Mullanpur | Chandigarh |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design, data modelling, report publishing |
| **Power Query** | Data cleaning, transformation, and ETL |
| **DAX** | Custom measures, KPIs, and calculated columns |
| **CSV / Excel** | Raw data storage and source files |

---

## 🚀 Getting Started

**Prerequisites:** [Power BI Desktop](https://www.microsoft.com/en-us/power-bi/desktop) (free, Windows only)

1. **Clone or download** this repository to your local machine
2. Ensure all **CSV files are in the same folder** as the `.pbix` file
3. Open `IPL_2024_Analysis.pbix` in Power BI Desktop
4. If prompted, **update the data source path** to point to your local CSV files
5. Click **Home → Refresh** to load all data
6. Explore the report using slicers, filters, and cross-highlights

---

## 📁 Repository Structure

```
IPL-2024-Analysis/
│
├── IPL_2024_Analysis.pbix               ← Main Power BI report
├── ipl_2024_deliveries.csv              ← Ball-by-ball delivery data (17,053 rows)
├── ipl2024_Matches_AutoRecovered_.csv   ← Match-level summary (74 rows)
├── ipl_players.csv                      ← Team squad lists
├── ipl_teams_owner.csv                  ← Franchise ownership & captains
└── README.md                            ← Project documentation
```

---

## 📜 License

This project is intended for **educational and personal portfolio purposes only.**  
All cricket data belongs to the Board of Control for Cricket in India (BCCI) and the IPL.
