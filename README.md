# 🛒 Integrated Retail Analytics for Store Optimization and Demand Forecasting

## 📌 Project Overview

This project focuses on applying **Data Analytics** and **Machine Learning** techniques to optimize retail store performance, forecast product demand, detect anomalies, segment stores, and provide actionable business recommendations. Using Walmart retail datasets, the project analyzes historical sales along with external factors such as promotions, holidays, fuel prices, CPI, unemployment, and store characteristics to support data-driven retail decision-making.

---

## 🎯 Project Objectives

- Detect anomalies in weekly sales data.
- Analyze seasonal trends and holiday effects.
- Perform data preprocessing and feature engineering.
- Segment stores using clustering techniques.
- Analyze department relationships for cross-selling opportunities.
- Forecast weekly sales using machine learning.
- Evaluate the impact of economic and promotional factors.
- Develop strategic recommendations for inventory and marketing optimization.

---

## 📂 Dataset Information

The project uses three datasets:

### 1. Sales Dataset
Contains weekly sales for each store and department.

**Features**
- Store
- Dept
- Date
- Weekly_Sales
- IsHoliday

---

### 2. Features Dataset

Contains external factors affecting sales.

**Features**
- Temperature
- Fuel_Price
- MarkDown1–MarkDown5
- CPI
- Unemployment
- IsHoliday

---

### 3. Stores Dataset

Contains store-specific information.

**Features**
- Store
- Type
- Size

---

## ⚙️ Project Workflow

### 1. Data Collection

- Imported three Walmart datasets
- Explored dataset structure
- Performed descriptive statistics

---

### 2. Data Wrangling

- Merged datasets
- Removed duplicate columns
- Checked missing values
- Verified data types
- Removed duplicates

---

### 3. Data Preprocessing

- Missing Value Treatment
- Outlier Detection & Capping (IQR Method)
- Categorical Encoding
- Feature Engineering
- Data Scaling
- Feature Selection
- Train-Test Split

---

### 4. Exploratory Data Analysis (EDA)

Visualizations performed:

- Sales Distribution
- Monthly Sales Trend
- Sales by Store Type
- Correlation Heatmap
- Pair Plot
- Holiday vs Non-Holiday Sales
- Fuel Price vs Sales
- Temperature vs Sales
- Markdown Analysis
- Store Size Analysis

---

### 5. Hypothesis Testing

- Holiday sales are higher than non-holiday sales.
- Larger stores generate higher revenue.
- Promotional markdowns increase sales.

---

## 🤖 Machine Learning Models

### Model 1 — K-Means Clustering

**Objective**

Segment stores based on operational and sales characteristics.

**Evaluation**

- Silhouette Score

---

### Model 2 — Department Correlation Analysis

Since customer-level transaction data was unavailable, department-wise sales correlation analysis was performed instead of traditional Market Basket Analysis.

**Objective**

Identify departments with similar demand patterns to support cross-selling strategies.

---

### Model 3 — XGBoost Regressor

**Objective**

Forecast weekly sales using historical sales, promotions, economic indicators, and store information.

**Evaluation Metrics**

- MAE
- RMSE
- R² Score

---

## 🔧 Feature Engineering

New features created:

- Total_MarkDown
- Has_MarkDown
- Year
- Month
- Week

---

## 📊 Model Explainability

SHAP (SHapley Additive Explanations) was used to interpret the XGBoost model and identify the most influential features affecting weekly sales.

Top important features include:

- Store
- Department
- Total_MarkDown
- Size
- Week
- Month
- Holiday Indicator

---

## 📈 Business Insights

- Holiday periods significantly increase weekly sales.
- Promotional markdowns positively influence demand.
- Larger stores generally generate higher revenue.
- Sales exhibit strong seasonal patterns.
- Store segmentation enables targeted inventory planning.
- Department correlation helps identify cross-selling opportunities.

---

## 💡 Strategic Recommendations

- Increase inventory before holidays and promotional events.
- Develop personalized marketing campaigns for different store segments.
- Optimize pricing and markdown strategies.
- Utilize demand forecasting for procurement planning.
- Monitor external economic factors while planning promotions.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- SHAP
- Google Colab

---

## 📁 Project Structure

```
Integrated-Retail-Analytics/
│
├── data/
│   ├── sales.csv
│   ├── features.csv
│   └── stores.csv
│
├── notebooks/
│   └── Integrated_Retail_Analytics.ipynb
│
├── images/
│   ├── eda_plots/
│   ├── clustering/
│   ├── shap/
│   └── forecasting/
│
├── report/
│   └── Capstone_Report.pdf
│
├── README.md
│
└── requirements.txt
```

---

## 📌 Results

- Successfully cleaned and integrated multiple retail datasets.
- Identified sales anomalies and seasonal demand patterns.
- Segmented stores using K-Means clustering.
- Performed department correlation analysis to infer cross-selling opportunities.
- Built an XGBoost model for accurate weekly sales forecasting.
- Explained model predictions using SHAP feature importance.

---

## 👨‍💻 Author

**Navjot Khatri**

Capstone Project: **Integrated Retail Analytics for Store Optimization and Demand Forecasting**

---

## ⭐ If you found this project helpful, consider giving it a star!
