# 📈 Electronics Sales Transaction Analysis

An end-to-end data analytics and predictive modeling project analyzing one year of electronics sales transactions to generate business insights and support data-driven decision-making ahead of Black Friday.

---

## Project Overview

As part of an electronics company's data team, the objective of this project was to analyze historical sales data and identify opportunities to improve revenue, optimize inventory planning, and enhance customer engagement strategies.

Using transaction data from the previous fiscal year, we explored customer behavior, product performance, purchasing trends, and developed machine learning models to predict customer actions.

---

## Business Problem

With Black Friday approaching, stakeholders needed answers to questions such as:

- Which customer segments generate the most revenue?
- Which products should receive additional inventory investment?
- What sales trends should the company prepare for?
- Can we predict customer behaviors to improve marketing efforts?

This project aimed to transform raw sales data into actionable business recommendations.

---

## Dataset

**Source:** Kaggle

### Dataset Characteristics

- 20,000 transactions
- 16 variables
- Time period: September 2023 – September 2024

### Key Features

- Customer ID
- Age
- Gender
- Loyalty Member Status
- Product Type
- SKU
- Rating
- Order Status
- Payment Method
- Quantity
- Unit Price
- Total Price
- Purchase Date
- Shipping Type
- Add-ons Purchased
- Add-on Total

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Data Cleaning & Feature Engineering

Several preprocessing steps were performed to improve data quality:

### Missing Value Treatment

**Gender**
- Missing values were imputed using probability-based random assignment according to the observed gender distribution.

**Add-ons Purchased**
- Missing values were replaced with `"None"`.

### Feature Engineering

Because add-on purchases contribute to actual revenue, a new variable was created:

```
Final Price = Total Price + Add-on Total
```

This metric was used throughout the analysis.

---

## Exploratory Data Analysis

### Customer Insights

- Middle-aged customers (35–64 years old) generated the highest revenue.
- Male customers consistently spent more across age groups.

### Product Performance

- Smartphones were the most profitable product category.
- Headphones generated the lowest revenue.

### Sales Trends

- Smartphone sales peaked in October 2023.
- Overall sales surged during the holiday season and declined throughout mid-2024.
- Completed orders peaked in January 2024.
- Canceled orders reached their highest level in August 2024.

### Customer Satisfaction

- Most customers provided 3-star ratings.
- Approximately 70% of transactions received ratings of 3 stars or higher.

---

## Predictive Modeling

Three classification models were developed to predict customer behaviors.

### 1. Overnight Shipping Prediction

**Objective**

Predict whether a customer would choose overnight shipping.

**Result**

- Mean Absolute Error (MAE): ~0.17
- Approximate predictive performance: **83%**

**Business Value**

Target customers likely to select overnight shipping with tailored shipping promotions.

---

### 2. Loyalty Membership Prediction

**Objective**

Predict whether a customer is likely to be a loyalty program member.

**Result**

- Mean Absolute Error (MAE): ~0.22
- Approximate predictive performance: **78%**

**Business Value**

Identify high-potential customers and encourage enrollment through personalized incentives.

---

### 3. Thursday Shopping Prediction

**Objective**

Predict whether a customer would make purchases on Thursdays.

**Result**

- Accuracy: **86–87%**

**Business Value**

Optimize inventory levels and launch targeted Thursday promotions to increase sales.

---

## Key Business Recommendations

Based on the analysis, the company should:

- Focus marketing efforts on middle-aged customers.
- Continue prioritizing smartphone inventory and promotions.
- Use predictive models to personalize shipping offers.
- Expand loyalty program enrollment initiatives.
- Investigate declining Thursday sales despite strong purchase likelihood.

---

## Repository Structure

```
electronics-sales-analysis/
│
├── Electronics Sales Transaction Analysis.ipynb
├── presentation/
│   └── Electronics Sales Transaction Analysis.pptx
├── assets/
│   └── dashboard-preview.png
├── index.html
└── README.md
```

---

## Future Improvements

Potential enhancements include:

- Deploying an interactive dashboard using Tableau or Power BI.
- Experimenting with advanced classification models such as XGBoost.
- Performing customer segmentation using clustering techniques.
- Building a sales forecasting model for Black Friday demand.

---

## Authors

- Ha Tran
- Adithya Venkatramanan

---

## Contact

Feel free to connect with me on LinkedIn or explore more projects in my GitHub portfolio.
