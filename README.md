# IPL Data Engineering Project

This project showcases a data engineering pipeline built to analyze and process IPL (Indian Premier League) cricket data. It includes data cleaning, transformation, and exploratory analysis using Azure Databricks and other data engineering tools. The analysis is based on match-level and delivery-level data.

## Project Structure

ipl-data-engineering-project/
├── data/                              # Directory for datasets
│   ├── deliveries.csv                 # IPL deliveries data
│   ├── matches.csv                    # IPL matches data
├── notebooks/                         # Directory for Jupyter/Databricks notebooks
│   └── ipl_data_analysis_notebook.ipynb # Analysis and data cleaning notebook
└── README.md                          # Project overview and instructions


## Project Objectives

- **Data Cleaning and Transformation**:
  - Handle missing values and inconsistencies in the raw datasets.
  - Transform the data into formats suitable for downstream analysis.

- **Exploratory Data Analysis (EDA)**:
  - Analyze match outcomes, team performance, player statistics, and trends across seasons.
  - Derive insights about batting, bowling, and team dynamics.

## Notable Features of the Project

1. **Schema Definition**:
   - **`matches_df` Schema**:
     - `id`: integer
     - `season`: string
     - `city`: strng
     - `date`: date
     - `match_type`: string
     - `player_of_match`: string
     - `venue`: stringi
     - `team1`: string
     - `team2`: string
     - `toss_winner`: string
     - `toss_decision`: string
     - `winner`: string
     - `result`: string
     - `result_margin`: integer
     - `target_runs`: integer
     - `target_overs`: integer
     - `super_over`: boolean
     - `method`: string
     - `umpire1`: string
     - `umpire2`: string


   - **`deliveries_df` Schema**:
     - `match_id`: integer
     - `inning`: integer
     - `batting_team`: string
     - `bowling_team`: string
     - `over`: integer
     - `ball`: integer
     - `batter`: string
     - `bowler`: string
     - `non_striker`: string
     - `batsman_runs`: integer
     - `extra_runs`: integer
     - `total_runs`: integer
     - `extras_type`: string
     - `is_wicket`: boolean
     - `player_dismissed`: string
     - `dismissal_kind`: string
     - `fielder`: string

2. **Data Cleaning**:
   - Managed missing values, particularly in columns like `result_margin` and `player_of_match`.
   - Ensured consistency in categorical fields such as team names.

3. **Analysis Highlights**:
   - Top-performing players for a team (Punjab Kings).
   - Team win/loss trends across different seasons.
   - Detailed match outcomes based on toss decisions.


---

This project is a demonstration of key data engineering concepts applied to IPL cricket data and is designed to showcase skills in data processing, analysis, and visualization. Feedback and suggestions are welcome!
