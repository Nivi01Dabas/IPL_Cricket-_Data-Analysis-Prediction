# IPL_Cricket-_Data-Analysis-Prediction
# 🏏 IPL Data Science Project

A complete end-to-end Data Science & Machine Learning project on IPL cricket data
using Python, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn.
## 👨‍💻 Project By
- **Name:** Nivya Dabas
- **Topic:** IPL Cricket Data Analysis & Prediction
- **Language:** Python 3.11
- **Type:** Data Science + Machine Learning
- 
## 📁 Project Structure

ipl_project/
│
├── 📄 ipl_analysis.py          → Main analysis + ML models
├── 📄 ipl_etl_pipeline.py      → ETL Pipeline
├── 📄 requirements.txt         → All libraries
├── 📄 README.md                → Project info (this file)
│
├── 📂 data/
│   ├── ipl_raw_data.json       → Raw API data
│   └── ipl_clean_data.csv      → Clean data (auto-generate)
│
├── 📂 outputs/
│   ├── eda_analysis.png        → EDA charts (auto-generate)
│   ├── player_performance.png  → Player charts (auto-generate)
│   ├── score_prediction.png    → Score model (auto-generate)
│   └── match_winner_prediction.png → Winner model (auto-generate)
│
├── 📂 models/
│   └── ipl_model.pkl           → Trained ML model (auto-generate)
│
├── 📂 database/
│   └── ipl_data.db             → SQLite database (auto-generate)
│
└── 📂 logs/
    └── etl_pipeline.log        → Pipeline logs (auto-generate)


## 🔧 Setup — Step by Step

### Step 1 — Python Install Karo
```
https://python.org/downloads
Python 3.11 download karo
"Add Python to PATH" tick karo
```

### Step 2 — Virtual Environment Banao
```bash
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac/Linux
```

### Step 3 — Libraries Install Karo
```bash
pip install -r requirements.txt
```

### Step 4 — API Key Lo (Free)
```
https://www.cricapi.com/ pe sign up karo
API key copy karo
ipl_etl_pipeline.py mein daalo:
API_KEY = "apni_key_yahan"
```

---

## 🚀 Project Kaise Chalaye

### ETL Pipeline pehle chalao:
```bash

python ipl_etl_pipeline.py
```

### Phir Main Analysis chalao:
```bash
python ipl_analysis.py
```

---

## 📊 Project Mein Kya Kya Hai

| Step | Kya Karta Hai |
|------|--------------|
| 1 | **Data Fetch** — CricAPI se live IPL data lena |
| 2 | **ETL Pipeline** — Data clean + transform + database mein save |
| 3 | **EDA** — Charts se data samajhna |
| 4 | **Player Analysis** — Batsmen & bowlers ki performance |
| 5 | **Score Prediction** — Linear Regression se score predict |
| 6 | **Winner Prediction** — Random Forest se match winner predict |

---

## 🤖 ML Models

### 1. Score Prediction — Linear Regression
- **Input Features:** Fours, Sixes, Balls Faced, Overs Bowled
- **Target:** Team 1 Score
- **Result:** MAE ~22 runs, R² Score

### 2. Match Winner — Random Forest Classifier
- **Input Features:** Team1, Team2, Venue, Toss Winner, Toss Decision, Scores
- **Target:** Match Winner
- **Result:** ~57% Accuracy

---

## 🔄 ETL Pipeline Details

```
EXTRACT   → CricAPI / CSV / Sample Data se data lao
    ↓
TRANSFORM → Nulls fill, duplicates remove, features banao
    ↓
LOAD      → CSV + SQLite Database mein save karo
```

### Features jo ETL banata hai:
- strike_rate     — Batsman ka strike rate
- economy_rate    — Bowler ki economy
- score_diff      — Dono teams ke scores ka fark
- toss_advantage  — Toss jeeta toh match bhi jeeta?
- is_high_score   — 180+ score flag
- total_boundaries — Fours + Sixes

---

## 📈 Output Charts

| Chart | Kya Dikhata Hai |
|-------|----------------|
| eda_analysis.png | Team wins, score distribution, toss decisions |
| player_performance.png | Top batsmen, bowlers, economy rates |
| score_prediction.png | Actual vs Predicted scores |
| match_winner_prediction.png | Feature importance, confusion matrix |

---

## 📦 Libraries Used

| Library | Kaam |
|---------|------|
| numpy | Mathematical calculations |
| pandas | Data manipulation |
| matplotlib | Charts & graphs |
| seaborn | Beautiful visualizations |
| scikit-learn | ML models |
| requests | API calls |
| sqlite3 | Database |
| logging | Pipeline logs |

---

## 💡 Aage Kya Kar Sakte Ho

- Streamlit dashboard banana
- XGBoost ya Neural Network try karna
- Ball-by-ball data add karna
- Player auction price prediction
- Live match score integration

---

## 🙋 API Reference

- CricAPI: https://www.cricapi.com/
- Endpoint: GET /v1/matches

---

## ✅ Project Status

- [x] ETL Pipeline
- [x] EDA Analysis
- [x] Player Performance Analysis
- [x] Score Prediction Model
- [x] Match Winner Prediction Model
- [ ] Streamlit Dashboard (Coming Soon)
- [ ] XGBoost Model (Coming Soon)
