# 🏏 T20 Cricket Team Performance Analysis System

A **data-driven cricket performance evaluation system** built using **Python, Pandas, Seaborn, and Streamlit**.

This project analyzes **T20 cricket match-level datasets** to evaluate player performance in a structured and unbiased way.  
It supports both **single match datasets and multiple match datasets**.

The project was first developed as a **Jupyter Notebook for data analysis**, and later converted into an **interactive Streamlit web application**.

---

# 🚀 Project Motivation

In many **local tournaments, school matches, and gully cricket**, performance evaluation is usually done manually.

This leads to several problems:

- Player contributions are judged subjectively
- Awards like **Best Batsman / Best Bowler** may not always be fairly decided
- Player consistency across matches is difficult to evaluate
- Bowling performance is often judged only by wickets
- Team contribution analysis is rarely structured

This project solves these problems by providing a **data-driven cricket analytics system**.

---

# 🎯 Project Objectives

The main objectives of this project are:

- Build a **structured performance analysis system**
- Evaluate **batting and bowling performance**
- Compare **players across matches**
- Analyze **team contribution by roles**
- Measure **player consistency**
- Create **fair statistical summaries for team evaluation**

---

# 🛠️ Tech Stack

### Programming Language
- Python

### Libraries Used
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Streamlit

### Development Environment
- Jupyter Notebook
- Streamlit Web App

---

# 📂 Dataset Structure

The system accepts **structured match-level datasets**.

### Required Columns

| Column | Description |
|------|------|
| Match_No | Match identifier |
| Player_Name | Player name |
| Role | batsman / bowler / all-rounder |
| Batting_Position | Player batting order |
| Batting_Start_Over | Over when player started batting |
| Out_Over | Over when player got out |
| Balls_Played | Total balls faced |
| Runs_Scored | Total runs scored |
| Overs_Bowled | Overs bowled |
| Runs_Given | Runs conceded |
| Wickets_Taken | Wickets taken |

---

# 🔎 Project Workflow

```
Raw Match Dataset
        ↓
Data Validation
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Performance Analysis
        ↓
Statistical Comparison
        ↓
Interactive Visualizations
```

---

# 🧹 Data Validation

The system performs automatic validation before analysis.

Validation rules include:

- `Match_No` cannot be missing
- `Player_Name` cannot be missing
- Numeric columns must contain valid numbers
- Batting data cannot exist without proper entry
- Bowling data cannot exist if overs bowled = 0

If validation fails, the system **stops execution and displays an error**.

---

# ⚙️ Feature Engineering

The system calculates additional performance metrics.

### Strike Rate

```
Strike Rate = (Runs Scored / Balls Played) × 100
```

### Economy Rate

Overs are converted into **real overs format** before calculating economy.

```
Economy Rate = Runs Given / Overs Bowled
```

### Player Out Detection

```
Was_Out = Out_Over > 0
```

---

# 📊 Analytical Modules

The system performs several analytical evaluations.

### Batting Analysis

- Difference between individual runs scored
- Team total runs per match
- Player runs in each match
- Strike rate comparison between batsmen and all-rounders
- Total runs contribution by roles

---

### Bowling Analysis

- Difference between individual wickets taken
- Team total wickets per match
- Player wickets per match
- Economy rate comparison between bowlers and all-rounders
- Total wickets contribution by roles

---

### Match Dynamics Analysis

The system analyzes wicket distribution across match phases.

| Phase | Overs |
|------|------|
| Powerplay | 1 – 6 |
| Middle Overs | 7 – 15 |
| Death Overs | 16 – 20 |

This helps identify **when most wickets fall during matches**.

---

### Player Consistency Analysis

Consistency is calculated using the formula:

```
Consistency Score = Mean Performance ÷ (Standard Deviation + 1)
```

This helps identify players who perform **consistently across matches**.

---

# 📈 Visual Representations

The Streamlit app generates visualizations using **Seaborn and Matplotlib**.

### Bar Charts

- Individual runs comparison
- Individual wickets comparison
- Strike rate comparison
- Economy rate comparison
- Batting consistency
- Bowling consistency
- Phase-wise wickets
- Average runs by batting position

### Pie Charts

- Runs contribution by player
- Wickets contribution by player
- Runs contribution by role
- Wickets contribution by role

---

# 🌐 Streamlit Application

An interactive **Streamlit dashboard** was built to make the analysis accessible.

### Features

- Upload **single match dataset**
- Upload **multiple match datasets**
- Automatic **data validation**
- Automated **performance analytics**
- Interactive **player comparisons**
- Dynamic **visual dashboards**

---

# 📁 Project Structure

```
Python Data Analysis Projects
│
└── T20-Cricket Team Performance Analysis Project
      │
      ├── T20_Cricket_Team_Performance_Analysis.ipynb
      │
      ├── Streamlit-version
      │      └── app.py
      │
      ├── template.csv
      ├── RCB_IPL2024_FirstMatch.csv
      ├── RCB_IPL2024_Match2_vs_PBKS.csv
      └── RCB_IPL2024_Match3_vs_GT.csv
```

---

# ▶️ How to Run This Project

### Clone the repository

```
git clone https://github.com/Pranay-256/DATA-SCIENCE-PROJECTS.git
```

### Install required libraries

```
pip install pandas numpy matplotlib seaborn streamlit
```

### Run the Streamlit application

```
streamlit run app.py
```

---

# 🎯 Skills Demonstrated

- Data Cleaning
- Data Validation
- Exploratory Data Analysis
- Feature Engineering
- Sports Data Analytics
- Statistical Analysis
- Interactive Dashboard Development
- Streamlit Application Development

---

# 👨‍💻 Author

**Pranay Jha**

Aspiring **Data Analyst / Data Scientist**

---

⭐ If you found this project useful, consider giving the repository a **star**.
