# 🛍️ Customer Shopping Behavior Analysis

## 📌 Project Overview

This project focuses on analyzing customer purchasing behavior using transactional data from approximately **3,900 records** across multiple product categories. The main goal is to identify patterns in customer spending, segment users, understand product preferences, and evaluate subscription behavior to support data-driven business decisions.

---

## 📊 Dataset Summary

* **Total Records:** 3,900
* **Total Features:** 18

### 🔑 Key Data Fields

* **Customer Information:** Age, Gender, Location, Subscription Status
* **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
* **Behavioral Data:** Discount Usage, Promo Codes, Previous Purchases, Purchase Frequency, Review Rating, Shipping Type

### ⚠️ Missing Values

* 37 missing values found in the **Review Rating** column

---

## 🧹 Data Processing & EDA (Python)

Data cleaning and preparation were performed using Python:

* Loaded dataset using **pandas**
* Performed initial inspection using `info()` and `describe()`
* Handled missing values by filling review ratings with the **median of respective categories**
* Standardized column names using **snake_case format**
* Created new features:

  * `age_group` → grouped customer ages
  * `purchase_frequency_days` → derived from purchase patterns
* Removed redundant column (**promo_code_used**)
* Exported cleaned data to **PostgreSQL** for further analysis

---

## 🧠 Data Analysis (SQL - PostgreSQL)

Performed structured queries to extract business insights:

1. Revenue comparison by gender
2. Identification of high-spending customers using discounts
3. Top 5 highest-rated products
4. Comparison of purchase value across shipping types
5. Spending behavior of subscribers vs non-subscribers
6. Products highly dependent on discounts
7. Customer segmentation (New, Returning, Loyal)
8. Top 3 products within each category
9. Subscription trends among repeat buyers
10. Revenue contribution by different age groups

---

## 📈 Dashboard (Power BI)

An interactive dashboard was created to visualize insights such as:

* Revenue distribution
* Customer segments
* Product performance
* Purchase behavior trends

---

## 💡 Business Recommendations

* **Increase Subscriptions:** Offer exclusive benefits to attract users
* **Strengthen Loyalty Programs:** Encourage repeat purchases
* **Optimize Discounts:** Balance between sales growth and profit margins
* **Promote Top Products:** Highlight best-performing and top-rated items
* **Target Marketing:** Focus on high-value customer groups and fast-shipping users

---

## 🛠️ Tech Stack

* **Python** (pandas, data cleaning, EDA)
* **PostgreSQL** (data analysis, queries)
* **Power BI** (data visualization & dashboarding)

---

## 🚀 How to Use

1. Clone the repository
2. Load dataset into Python
3. Perform data cleaning and preprocessing
4. Import cleaned data into PostgreSQL
5. Run SQL queries for analysis
6. Open Power BI dashboard file to explore insights

---

## 📌 Conclusion

This project demonstrates a complete **end-to-end data analytics workflow**, from raw data processing to business insights visualization. It highlights how data can be transformed into actionable strategies for improving customer engagement and business performance.

---
