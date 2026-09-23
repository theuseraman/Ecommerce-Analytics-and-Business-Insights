# E-Commerce Sales & Customer Analytics

**Internship Project — BharatCares Data Analytics Program**

## 📌 Project Overview

This project analyzes an e-commerce platform's order, customer, product, and payment data to uncover business insights and translate them into actionable recommendations, following the **Raw Data → Information → Insights → Decision → Action** framework.

The analysis covers:
- Data cleaning & validation (missing values, duplicates, invalid ranges, data types)
- Exploratory Data Analysis (EDA) with visualizations
- Key business KPIs (Revenue, AOV, ARPU, Discount Leakage, Return Rate)
- Category, city, and customer-segment performance
- Risk, opportunity, and action recommendations

## 📊 Dataset

- **Source:** [E-Commerce Sales Data Analysis and EDA — Kaggle](https://www.kaggle.com/datasets/erfan4524/e-commerce-sales-data-analysis-and-eda)
- **Raw file:** `Ecommerce_Raw_Source_Data.xlsx` (4 sheets — Customers, Orders, Payments, Products)
- **Cleaned file used for analysis:** `cleaned_ecommerce_data.xlsx` (sheet: `clean_ecommerce_data`) — 49,222 rows × 17 columns
- **Note:** This is an independent dataset and is not the dataset used in the BharatCares masterclasses.

## 🧰 Tech Stack

- Python (Pandas, Matplotlib, Seaborn)
- Jupyter Notebook
- Excel (data source)

## 📈 Key Findings (Summary)

| KPI | Value |
|---|---|
| Net Revenue | ₹3,445,770 |
| Total Orders | 49,198 |
| Unique Customers | 9,820 |
| Average Order Value (AOV) | ₹70.04 |
| Revenue Per User (ARPU) | ₹350.89 |
| Return/Cancellation Rate | 0.04% |
| Discount Revenue Leakage | ₹282,153 (7.57% of potential sales) |

**Top insight:** Electronics drives 50.83% of total revenue, but flat discounting across all categories is leaking ~7.6% of potential sales without increasing basket size (discount-quantity correlation ≈ 0.002). VIP customers' average order value (₹68.63) trails Regular customers (₹70.20), indicating the loyalty tier needs redesigning.

Full KPI breakdown, category/segment analysis, and the 12-question business matrix are in the project report.

## 📁 Repository Structure

```
├── README.md                              # This file
├── requirements.txt                       # Python dependencies
├── ecommerce_analysis.ipynb               # Full code: cleaning, validation, EDA, KPIs
├── Project_Report.docx                    # Detailed report with dashboard screenshots
├── cleaned_ecommerce_data.xlsx            # Cleaned dataset used for analysis
└── dashboard/
    ├── dashboard_page1_executive_overview.png
    ├── dashboard_page2_sales_product.png
    └── dashboard_page3_customer_risk.png
```

## ▶️ How to Run

1. Clone this repository
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Make sure `cleaned_ecommerce_data.xlsx` is in the same folder as the notebook
4. Open and run `ecommerce_analysis.ipynb` in Jupyter Notebook / JupyterLab / VS Code

## 📊 Dashboard

A 3-page executive dashboard is included under `/dashboard`:
1. **Executive Overview** — core KPIs, revenue trend, order status
2. **Sales & Product Analysis** — category, product, city, and payment breakdown
3. **Customer & Risk Analysis** — segment performance, demographics, risk & opportunity callouts

## 🎯 Business Recommendations

1. Replace flat discounts with threshold-based discounting (e.g., "Spend ₹150, get 10% off") to lift basket size.
2. Redesign the VIP loyalty tier with exclusive bundles and priority perks, since VIP AOV currently trails Regular customers.
3. Prioritize Electronics in supply chain and inventory planning — it drives over half of total revenue.
4. Use city-category revenue patterns to guide regional warehouse and marketing allocation.

---
*Submitted as part of the BharatCares Data Analytics Internship final project.*
