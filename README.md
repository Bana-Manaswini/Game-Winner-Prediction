# 🕹️ PUBG Game Winner Prediction

## 📘 Overview

PUBG Game Winner Prediction is a machine learning project aimed at predicting a player’s final placement (`winPlacePerc`) in a PUBG match using in-game performance statistics. By analyzing features like kills, distance traveled, healing items used, and damage dealt, this model helps uncover patterns that contribute to winning the game.

---

## 🎯 Objective

To build a regression model that accurately predicts the percentage rank (`winPlacePerc`) a player achieves in a PUBG match based on real-time gameplay metrics.

---

## 📂 Dataset Features

The dataset includes various player-level statistics:
- `kills`, `headshotKills`, `damageDealt`
- `walkDistance`, `rideDistance`, `swimDistance`
- `boosts`, `heals`, `weaponsAcquired`
- `matchType`, `maxPlace`, `numGroups`
- Target: `winPlacePerc` (Normalized rank from 0 to 1)

---

## 🔍 Project Workflow

### 1. Data Preprocessing
- Handled missing values and outliers
- Removed matches with irregular data
- Converted categorical features where needed

### 2. Feature Engineering
- Created combined features like:
  - `totalDistance = walk + ride + swim`
  - `healthItems = heals + boosts`
  - `killPerDistance = kills / totalDistance`
- Normalized skewed variables

### 3. Exploratory Data Analysis (EDA)
- Correlation heatmaps
- Feature distributions
- Match type filtering and analysis

### 4. Model Building
- Algorithms used:
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
- Evaluation Metrics:
  - MAE – Mean Absolute Error
  - RMSE – Root Mean Squared Error

### 5. Results & Insights
- XGBoost achieved the best prediction accuracy
- Key features: `kills`, `damageDealt`, `walkDistance`, `healthItems`
- Feature importance plots helped interpret model decisions

---

## 🛠️ Tech Stack

- Language: Python  
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost  
- Environment: Jupyter Notebook  

---

## 📊 Output

- Final model predicts `winPlacePerc` with low error.
- Visualizations show gameplay behavior linked to winning strategies.
- Insights can be used for in-game coaching and analytics.

---

## 💡 Applications

- eSports Analytics: Assist teams with performance optimization  
- Training Tools: Provide recommendations to players  
- Live Prediction: Real-time ranking forecasts for matches

---

## 📁 Repository Contents

- `PubgGamePrediction.ipynb` – Main notebook with full ML pipeline  
- (Optional) `dataset.csv` – Dataset if provided

---

## 👤 Author

Bana Manaswini
AI & Data Science Enthusiast  
GitHub: [https://github.com/Bana-Manaswini)

---

## 📬 Contact

For collaboration or questions:  
Email: manaswinireddybana@gmail.com


