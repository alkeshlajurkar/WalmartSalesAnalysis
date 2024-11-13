# 🌟 Walmart Sales Data Analysis

## 📘 About the Project

This project explores Walmart sales data to uncover insights into top-performing branches, product trends, and customer behavior, aiming to refine sales strategies for optimization. The data was sourced from the [Kaggle Walmart Sales Forecasting Competition](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting).

> "In this competition, participants are provided with historical sales data for 45 Walmart stores across various regions, including markdown events that influence sales." [source](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting)

---

## 🎯 Project Goals

1. **Product Analysis**: Identify top-selling product lines and areas for improvement.
2. **Sales Analysis**: Track product sales trends over time.
3. **Customer Analysis**: Understand customer segments and purchasing behaviors.

---

## 📊 About the Data

This dataset contains 17 columns and 1000 rows, covering sales transactions at three Walmart branches in Mandalay, Yangon, and Naypyitaw. Below are the primary columns:

| Column                  | Description                             | Data Type      |
| :---------------------- | :-------------------------------------- | :------------- |
| invoice_id              | Invoice for each sale                   | VARCHAR(30)    |
| branch                  | Branch where sale was made              | VARCHAR(5)     |
| city                    | Location of the branch                  | VARCHAR(30)    |
| customer_type           | Type of customer                        | VARCHAR(30)    |
| gender                  | Customer gender                         | VARCHAR(10)    |
| product_line            | Product category                        | VARCHAR(100)   |
| unit_price              | Price per unit                          | DECIMAL(10, 2) |
| quantity                | Quantity sold                           | INT            |
| VAT                     | Tax on purchase                         | FLOAT(6, 4)    |
| total                   | Total purchase cost                     | DECIMAL(10, 2) |
| date                    | Date of purchase                        | DATE           |
| time                    | Time of purchase                        | TIMESTAMP      |
| payment_method          | Payment method                          | VARCHAR(20)    |
| cogs                    | Cost of Goods Sold                      | DECIMAL(10, 2) |
| gross_margin_percentage | Gross margin percentage                 | FLOAT(11, 9)   |
| gross_income            | Gross Income                            | DECIMAL(10, 2) |
| rating                  | Customer rating                         | FLOAT(2, 1)    |

---

## 📌 Analysis Checklist

### Product Analysis

- Which product lines are most and least popular?
- Identify high-performing products and those needing strategy adjustments.

### Sales Analysis

- Track monthly revenue trends.
- Assess COGS by product and branch to identify cost-saving opportunities.

### Customer Analysis

- Identify customer demographics, behavior, and preferred purchasing times.
- Examine ratings to enhance customer satisfaction strategies.

---

## 🔍 Approach

1. **Data Cleaning & Wrangling**: Detect and address null values, ensuring data integrity.
2. **Feature Engineering**: Add insightful columns such as `time_of_day`, `day_name`, and `month_name` to capture daily and monthly patterns.
3. **Exploratory Data Analysis (EDA)**: Visualize trends to answer the project’s core business questions.

---

## 📈 Business Questions

**Generic Questions**

1. How many unique cities and branches are in the dataset?

**Product Analysis**

1. Which payment method is most common?
2. What are the most and least popular product lines?
3. Which branches and cities generate the highest revenue?

**Sales Analysis**

1. How do sales vary by time of day and customer type?
2. Which branch has the highest sales and gross margin?

**Customer Analysis**

1. What is the gender distribution per branch?
2. What times and days yield the highest customer ratings?

---

## 📊 Revenue & Profit Formulas

Calculations:

1. **COGS** = `unit_price * quantity`
2. **VAT** = `5% of COGS`
3. **Gross Profit** = `Total Revenue - COGS`
4. **Gross Margin** = `Gross Income / Total Revenue`

---

## 📂 Code

Find the code for SQL queries in [Walmart_SQL_Queries.sql](Walmart_SQL_Queries.sql).
