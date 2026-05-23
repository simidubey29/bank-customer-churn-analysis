# Bank Customer Churn Analysis Using SQL & Python
SQL and Python-based analysis of 10,000+ bank customers. Explores churn behavior, customer demographics, balance trends, salary insights, and business intelligence using real-world banking data.

## Overview

This project analyzes a real-world banking customer dataset containing over 10,000 customer records. Using SQL queries and Python, the project explores customer demographics, account balances, credit scores, salary patterns, and customer churn behavior to generate meaningful business insights.

The analysis combines SQL-based querying with Python data analysis and visualization techniques to understand factors influencing customer retention and banking performance.

---

## Live Notebook

View the complete interactive analysis on Kaggle:

🔗 **[Kaggle Notebook](https://www.kaggle.com/code/simidubey/bank-customer-churn-analysis)**

---

## Dataset

**Bank Customer Churn Dataset**

Source:

https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling

### Dataset Features

- CustomerId
- Surname
- CreditScore
- Geography
- Gender
- Age
- Tenure
- Balance
- NumOfProducts
- HasCrCard
- IsActiveMember
- EstimatedSalary
- Exited (Churn Status)

### Dataset Size

- 10,000+ Customer Records
- Multiple Customer Attributes
- Real-world Banking Data

---

## Objectives

- Analyze customer demographics and distribution
- Study customer churn behavior
- Compare balance trends across countries
- Examine credit score patterns
- Analyze customer salary distribution
- Identify factors associated with customer retention
- Generate business insights through SQL analysis

---

## Technologies Used

- Python
- SQL (SQLite)
- Pandas
- Matplotlib
- Kaggle Notebook

---

## Project Workflow

1. Load banking customer dataset
2. Create SQLite database connection
3. Import customer data into SQL table
4. Execute SQL queries for business analysis
5. Analyze customer behavior and churn patterns
6. Create visualizations for key metrics
7. Generate insights and findings

---

## SQL Analysis Performed

### Customer Overview

- Total customer count
- Customer distribution by country
- Gender distribution analysis

### Financial Analysis

- Average account balance
- Top customers by balance
- Salary distribution analysis
- Average balance by geography

### Churn Analysis

- Customer retention vs churn comparison
- Average age by churn status
- Active member analysis
- Customer exit patterns

### Credit Score Analysis

- Minimum credit score
- Maximum credit score
- Average credit score
- Credit score distribution insights

### Product Usage Analysis

- Number of products per customer
- Customers with multiple banking products

---

## Sample SQL Queries

### Total Customers

```sql
SELECT COUNT(*) AS Total_Customers
FROM Customers;
```

### Average Balance by Country

```sql
SELECT Geography,
       ROUND(AVG(Balance),2) AS AvgBalance
FROM Customers
GROUP BY Geography;
```

### Customer Churn Analysis

```sql
SELECT Exited,
       COUNT(*) AS Customers
FROM Customers
GROUP BY Exited;
```

---


## Repository Structure

```text
bank-customer-churn-analysis/
│
├── bank_customer_churn_analysis.ipynb
├── README.md
└── findings.md
```

---

## How to Run

### Option 1: Kaggle

1. Open Kaggle Notebooks
2. Upload the Bank Customer Churn Dataset
3. Open the notebook
4. Run all cells sequentially
5. Review SQL query outputs and visualizations

### Option 2: Jupyter Notebook

1. Install required libraries

```bash
pip install pandas matplotlib
```

2. Download the dataset

3. Open the notebook

4. Run all cells

---

## Learning Outcomes

Through this project, the following concepts were practiced:

- SQL Query Writing
- Database Operations
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Customer Segmentation
- Churn Analysis
- Data Visualization
- Business Insight Generation

---

## Future Improvements

- Build customer churn prediction models using Machine Learning
- Create an interactive dashboard using Power BI or Tableau
- Perform advanced customer segmentation
- Analyze customer lifetime value
- Deploy an interactive analytics application using Streamlit

---

## Author

**Simi Dubey**

B.Sc. Data Science Student

Aspiring Data Analyst | SQL | Python | Data Visualization | Machine Learning

---
