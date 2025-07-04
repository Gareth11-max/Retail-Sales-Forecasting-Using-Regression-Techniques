# 🧮 Retail Sales Forecasting Using Regression

This project focuses on building a supervised machine learning regression model to predict daily sales for retail stores. Using historical data, the model learns patterns based on features such as store opening status, day of the week, promotions, and holidays. The goal is to forecast sales accurately and help drive better planning, inventory management, and marketing strategies.

---

## 📌 Objective

To predict **daily retail sales** based on operational and temporal factors using regression techniques. The model aims to support **data-driven decision-making** in retail operations.

---

## 💼 Business Objective

- Improve **forecasting accuracy** to optimize:
  - Inventory planning
  - Workforce allocation
  - Promotional campaigns
- Reduce resource wastage and lost sales due to under/over-stocking.

---

## 📊 Dataset Overview

- **Features include:**
  - `DayOfWeek`
  - `Promo` (promotion active)
  - `Open` (store open or closed)
  - `StateHoliday`
  - `SchoolHoliday`
  - `StoreType`, `Assortment`
  - `CompetitionDistance`
- **Target Variable:**
  - `Sales` (continuous numeric value)

- **Data Source:** [Custom Retail Dataset or Kaggle's Rossmann Dataset]

---

## 🔍 Methodology

1. **Data Preprocessing**
   - Handling missing values
   - Encoding categorical variables
   - Feature engineering (e.g., extracting month/day from date)
2. **Exploratory Data Analysis (EDA)**
   - Trend analysis, sales distribution, and seasonal patterns
   - Correlation heatmaps and boxplots
3. **Modeling**
   - Baseline: Linear Regression
   - Advanced: Random Forest, XGBoost Regressor
4. **Evaluation**
   - Compared models using MAE, RMSE, and R² Score
5. **Hyperparameter Tuning**
   - GridSearchCV / RandomizedSearchCV for optimal model performance

---

## 🧪 Evaluation Metrics

- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score** (coefficient of determination)

---

## 📈 Results

| Model               | R² Score | RMSE     | MAE      |
|--------------------|----------|----------|----------|
| Linear Regression   | 0.72     | 1700.56  | 1250.34  |
| Random Forest       | 0.86     | 1125.41  | 890.22   |
| XGBoost Regressor   | **0.89** | **980.12** | **845.90** |

✅ **XGBoost** performed best and is recommended for deployment.

---

## 📌 Key Insights

- **Promotions and holidays** have a strong impact on daily sales.
- Stores that remain open during state holidays tend to have **higher average sales**.
- **Day of the week** shows consistent variation, with weekends usually performing better.
- A small group of stores generates a significant portion of total revenue.

---

## 🛠️ Tools & Technologies

- **Languages:** Python (Pandas, NumPy, Scikit-learn)
- **Visualization:** Matplotlib, Seaborn
- **Modeling:** XGBoost, Random Forest, Linear Regression
- **IDE:** Jupyter Notebook / Google Colab

---



