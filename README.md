
# 🏏 IPL Prediction System using Streamlit

## 📌 Project Overview
This project is a **Web-based IPL Prediction System** built using **Streamlit**. It allows users to predict match winners and player performances based on historical IPL data. Additionally, it provides rich **visual analytics** on team performance, venue trends, and player statistics. The system leverages **Machine Learning** models trained on IPL datasets to make predictions.

---

## ✨ Features
### 1️⃣ Match Winner Prediction
- Predict the winning team based on:
    - Team 1 & Team 2
    - Venue
    - Toss Winner
    - Team Batting First
- Machine Learning Model: **Logistic Regression / Random Forest**

### 2️⃣ Player Performance Prediction
- Predict individual player performance (runs/wickets) based on:
    - Player Name
    - Opposition Team
    - Venue
    - Recent Form (last 5 matches)
- Machine Learning Model: **Regression Model (Linear Regression)**

### 3️⃣ IPL Data Dashboard
- Visual analysis of IPL history:
    - Team-wise Win Percentage
    - Venue-wise Winning Records
    - Top Players (Highest Run Scorers, Leading Wicket Takers)
    - Current Season Points Table (if integrated with live data)


## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/IPL_Prediction.git
cd IPL_Prediction
```

### 2️⃣ Install Dependencies
Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate       # For Windows
```

Install required libraries:
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Application
```bash
streamlit run app.py
```

---

## 📊 Sample Data
| Match ID | Team 1 | Team 2 | Venue | Toss Winner | Batting First | Winner |
|--|--|--|--|--|--|--|
| 1 | MI | CSK | Wankhede | MI | Yes | MI |
| 2 | RCB | KKR | Chinnaswamy | KKR | No | RCB |

| Player | Opposition | Venue | Last 5 Innings Runs | Predicted Runs |
|--|--|--|--|--|
| Virat Kohli | CSK | Chinnaswamy | 45, 60, 32, 55, 78 | 52 |

---

## 🧰 Tech Stack
| Component | Technology |
|--|--|
| Data Processing | pandas, numpy |
| Machine Learning | scikit-learn |
| Visualization | seaborn, matplotlib, plotly |
| Web Framework | Streamlit |

---

## 📊 Model Workflow
1. Load and preprocess IPL data (matches & player stats)
2. Train models:
    - Match Winner Model: Uses team, venue, toss, batting first as features.
    - Player Performance Model: Uses player, opposition, venue, recent form as features.
3. Save trained models using `joblib` or `pickle`.
4. Streamlit app:
    - Accepts user inputs via dropdown & text fields.
    - Uses pre-trained models to predict results.
    - Displays interactive plots using historical data.

---


## 🚀 Future Enhancements
✅ Live IPL data scraping for real-time analysis  
✅ Player comparison feature (batting average, strike rate, economy)  
✅ Historical head-to-head records  
✅ Prediction confidence scores  
✅ Team Strength Visualization (Batting vs Bowling)

