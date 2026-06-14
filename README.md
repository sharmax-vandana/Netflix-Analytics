# Netflix-Analytics : [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1L5lle2eKn7sITaaWoTirFO19yHhpB9Lq?usp=sharing) https://nbviewer.org/github/sharmax-vandana/Netflix-Analytics/blob/main/Netflix_User_Analytics.ipynb
# 🎬 Netflix User Analytics

A machine learning project analyzing Netflix subscriber behaviour to predict **subscription renewal** and **monthly spending** using Decision Tree, KNN, and Linear Regression.

---

##  Repository Structure

```
Netflix-Analytics/
├── Dataset_2.csv                 # Netflix user dataset (750 records)
├── Netflix_User_Analytics.ipynb  # Main analysis notebook
└── README.md
```

---

##  Dataset

750 Netflix users with the following features:

| Column | Description |
|---|---|
| `UserID` | Unique user identifier |
| `Age` | User age |
| `Gender` | Male / Female |
| `SubscriptionType` | Basic / Premium / VIP |
| `WatchHoursPerWeek` | Hours watched per week |
| `DevicesUsed` | Number of devices used |
| `FavoriteGenre` | Action, Comedy, Drama, Sci-Fi, Horror, Romance |
| `AdClicks` | Number of advertisement clicks |
| `MonthlySpend` | Monthly spending (₹) |
| `SubscriptionRenewed` | Yes / No |

---

##  Notebook Outline

### Part A — Dataset Understanding
- Load & preview data
- Shape, columns, dtypes
- Missing value check

### Part B — Exploratory Data Analysis
- Average age, watch hours, monthly spend
- Subscription type distribution
- Renewal percentage breakdown

### Part C — Data Preparation
- Label encoding of categorical features
- Feature/target split for classification and regression
- Stratified 80/20 train-test split

### Part D — Decision Tree Classification
- Train model to predict `SubscriptionRenewed`
- Accuracy evaluation
- Confusion matrix with TP/TN/FP/FN interpretation

### Part E — K-Nearest Neighbors (KNN)
- KNN classifier with K = 5
- Accuracy comparison with Decision Tree

### Part F — Linear Regression
- Predict `MonthlySpend`
- MSE, RMSE, R² evaluation
- Actual vs Predicted scatter plot
- New user spend prediction

---

##  Tech Stack

- **Python 3**
- `pandas`, `numpy` — data handling
- `matplotlib`, `seaborn` — visualisation
- `scikit-learn` — ML models

---

##  How to Run

1. Clone the repo
   ```bash
   git clone https://github.com/sharmax-vandana/Netflix-Analytics.git
   cd Netflix-Analytics
   ```

2. Install dependencies
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. Launch the notebook
   ```bash
   jupyter notebook Netflix_User_Analytics.ipynb
   ```

> Make sure `Dataset_2.csv` is in the same directory as the notebook before running.

---

##  Key Findings

- **Subscription renewal** is a classification problem — predicted using Decision Tree & KNN
- **Monthly spending** is a regression problem — predicted using Linear Regression
- Features like `WatchHoursPerWeek`, `MonthlySpend`, and `SubscriptionType` are strong renewal indicators
- Model predictions can help Netflix target at-risk users with personalised retention campaigns
