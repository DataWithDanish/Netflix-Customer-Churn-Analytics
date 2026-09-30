# Netflix-Customer-Churn-Analytics
# 📊 Netflix Customer Churn Analytics

An end-to-end **Customer Churn Analytics & Predictive Risk Modeling** project built using Microsoft Excel. This project demonstrates practical Data Analyst and Data Science skills including data cleaning, exploratory data analysis, customer segmentation, KPI development, dashboarding, revenue-at-risk analysis, and predictive churn modeling.

> **Note:** This is a portfolio project using a customer churn dataset. It is not official Netflix corporate data.

---

## 📸 Dashboard Preview

![Customer Churn Dashboard](https://github.com/DataWithDanish/Netflix-Customer-Churn-Analytics/blob/5b70dfc8fb35c3ddbba727c9bc354029e6d05ecd/Screenshot%202026-10-01%20012505.png)

![Customer Churn Analysis](https://github.com/DataWithDanish/Netflix-Customer-Churn-Analytics/blob/5b70dfc8fb35c3ddbba727c9bc354029e6d05ecd/Screenshot%202026-10-01%20012628.png)

---

## 🎯 Project Objective

The objective of this project is to analyze customer behavior and identify factors associated with customer churn.

The analysis focuses on:

- Understanding overall customer churn
- Identifying high-risk customer segments
- Analyzing subscription-level churn
- Understanding customer engagement and recency
- Measuring revenue at risk
- Creating customer risk categories
- Building a predictive churn model
- Creating an executive-level dashboard for business decision-making

---

## 💼 Business Problem

Customer churn directly impacts recurring revenue.

The business needs to understand:

- Which customers are more likely to churn?
- Which subscription segments have higher churn?
- Which customer behaviors are associated with churn?
- How much revenue is potentially at risk?
- Which customers should be prioritized for retention?
- Can customer-level churn probability be estimated using historical data?

This project converts raw customer-level data into actionable analytical insights.

---

## 🛠️ Tools & Technologies

### Data Analysis
- Microsoft Excel
- Excel Tables
- Excel Formulas
- Conditional Formatting
- Data Validation
- Pivot-style analytical calculations
- Statistical analysis

### Data Science
- Python
- Pandas
- NumPy
- Scikit-learn
- Logistic Regression

### Visualization
- Excel Dashboard
- KPI Cards
- Bar Charts
- Doughnut Charts
- Conditional Formatting
- Risk Heatmaps

### Analytical Techniques
- Data Cleaning
- Exploratory Data Analysis
- Customer Segmentation
- Churn Analysis
- Revenue-at-Risk Analysis
- Feature Engineering
- Predictive Modeling
- Model Evaluation

---

## 📂 Dataset

The dataset contains **5,000 customer records** with **14 source fields**.

Key fields include:

| Field | Description |
|---|---|
| `customer_id` | Unique customer identifier |
| `age` | Customer age |
| `gender` | Customer gender |
| `subscription_type` | Subscription tier |
| `watch_hours` | Total watch hours |
| `last_login_days` | Days since last login |
| `region` | Customer region |
| `device` | Primary device |
| `monthly_fee` | Monthly subscription fee |
| `churned` | Customer churn indicator |
| `payment_method` | Payment method |
| `number_of_profiles` | Number of profiles |
| `avg_watch_time_per_day` | Average daily watch time |
| `favorite_genre` | Favorite content genre |

---

## 🔍 Data Analysis Process

The project follows a complete analytical workflow:

```text
Raw Customer Data
       ↓
Data Quality Checks
       ↓
Data Cleaning & Validation
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
Customer Segmentation
       ↓
Churn Analysis
       ↓
Revenue-at-Risk Analysis
       ↓
Predictive Modeling
       ↓
Risk Scoring
       ↓
Executive Dashboard
       ↓
Business Insights
```

---

## 🧹 Data Quality & Validation

The workbook includes an audit layer to validate:

- Missing values
- Duplicate customer IDs
- Invalid age values
- Negative watch hours
- Invalid login recency
- Invalid monthly fees
- Invalid churn flags
- Data completeness

This ensures the analytical results are based on validated data.

---

## 📊 Feature Engineering

Additional analytical fields were created using Excel formulas.

### Age Band

Customers are grouped into:

- 18–24
- 25–34
- 35–44
- 45–54
- 55–70

### Watch Band

Customers are categorized according to watch-hour engagement.

### Recency Band

Customers are categorized based on days since their last login.

### Engagement Band

Customer engagement is classified using:

- Watch hours
- Login recency

### Risk Band

Customers are categorized into:

- 🟢 Low
- 🟡 Medium
- 🟠 High
- 🔴 Critical

---

## 📈 Churn Analysis

Churn is analyzed across multiple business dimensions:

- Subscription Type
- Payment Method
- Region
- Device
- Favorite Genre
- Age Band

For each segment, the workbook calculates:

- Customer count
- Churned customers
- Churn rate
- Average watch hours
- Average login recency
- Revenue at risk

---

## 👥 Customer Segmentation

The project creates behavioral customer segments:

### 🏆 Champions

Highly engaged customers with recent activity and comparatively lower predicted risk.

### ⚠️ Engaged but At Risk

Highly engaged customers showing elevated predicted churn risk.

### 📉 Slipping

Customers with declining engagement and relatively stale login activity.

### 🔴 Dormant / High Risk

Low-engagement customers with significantly stale login activity.

---

## 💰 Revenue at Risk

A revenue-at-risk metric was created to connect customer analytics with business impact.

```text
Revenue at Risk
=
Monthly Fee × Churn Probability
```

This provides a more useful prioritization framework than simply counting churned customers.

A high-value customer with a high churn probability can therefore receive greater attention than a low-value customer with the same probability.

---

## 🤖 Predictive Modeling

A **Logistic Regression** model was developed to estimate customer churn probability.

The model uses customer characteristics and behavioral variables to estimate the probability that a customer may churn.

The model includes:

- Numerical feature standardization
- Categorical feature encoding
- Logistic Regression
- Probability scoring
- Risk classification

The model parameters are also transferred into Excel so that customer-level probabilities can be calculated transparently.

---

## 📐 Model Evaluation

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix

This allows the predictive model to be evaluated beyond simple accuracy.

---

## 📊 Excel Dashboard

The executive dashboard provides:

### KPI Metrics

- Total Customers
- Churned Customers
- Churn Rate
- Average Monthly Fee
- Revenue at Risk
- Critical Risk Customers

### Visual Analysis

- Churn Rate by Subscription
- Customer Risk Distribution
- Segment-level analysis
- Revenue exposure

The dashboard also includes a subscription filter for:

```text
All
Basic
Standard
Premium
```

---

## 📁 Project Structure

```text
Netflix-Customer-Churn-Analytics/
│
├── README.md
│
├── Netflix_Customer_Churn_Analytics_Portfolio.xlsx
│
├── data/
│   └── netflix_customer_churn.csv
│
└── screenshots/
    ├── dashboard.png
    ├── churn-analysis.png
    └── predictive-model.png
```

---

## 📑 Excel Workbook Structure

The Excel workbook contains the following analytical layers:

| Sheet | Purpose |
|---|---|
| `Dashboard` | Executive dashboard and KPIs |
| `Raw_Data` | Original customer dataset |
| `Analysis_Data` | Formula-driven analytical layer |
| `Churn_Analysis` | Dimension-level churn analysis |
| `Customer_Segments` | Behavioral segmentation |
| `Predictive_Model` | Logistic regression and model evaluation |
| `Data_Quality` | Data validation and audit checks |
| `Data_Dictionary` | Field definitions |
| `Analyst_Notes` | Interview insights and project explanation |

---

## 💡 Key Analytical Insights

The project demonstrates how raw customer data can be converted into:

```text
Customer Data
      ↓
Customer Behavior
      ↓
Churn Risk
      ↓
Revenue Exposure
      ↓
Retention Prioritization
```

Instead of only reporting historical churn, the project introduces a predictive layer to help identify customers who may require retention attention.

---

## 🎯 Business Applications

This analytical framework can support:

- Customer retention
- Subscription strategy
- Customer segmentation
- Revenue protection
- Retention campaign targeting
- Customer lifecycle management
- Risk-based prioritization
- Management reporting

---

## ⚠️ Limitations

- The dataset does not contain a time/date field, so true monthly churn trends and cohort retention analysis cannot be calculated.
- The dataset is used for portfolio/learning purposes.
- Model performance should be validated against future or production data before operational deployment.
- Correlation does not imply causation.
- Retention actions should ideally be validated through controlled experiments or additional business data.

---

## 🚀 What I Learned

Through this project, I practiced:

- Data Cleaning
- Data Validation
- Exploratory Data Analysis
- Feature Engineering
- Excel Formula Engineering
- Dashboard Development
- Customer Segmentation
- KPI Development
- Revenue-at-Risk Analysis
- Predictive Modeling
- Logistic Regression
- Model Evaluation
- Business Storytelling
- Data-driven Decision Support

---

## 👨‍💻 Author

**Danish**

Data Analyst | Data Science | Excel | Python | SQL | Data Visualization

GitHub: [@DataWithDanish](https://github.com/DataWithDanish)

---

## ⭐ Project

If you found this project useful, feel free to ⭐ the repository.
