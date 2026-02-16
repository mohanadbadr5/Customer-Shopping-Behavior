# Customer Shopping Behavior Analysis 🛒📊

## 1. Project Overview
This project provides a comprehensive analysis of customer shopping behavior using a dataset of **3,900 purchases**. The goal was to transform raw transactional data into actionable business intelligence to optimize marketing spend, improve customer retention, and refine pricing strategies.

## 2. Tech Stack
*   **Data Cleaning & Preprocessing:** Python (Pandas, NumPy)
*   **Database Management:** PostgreSQL
*   **Data Visualization:** Power BI
*   **Documentation:** Microsoft Word & PowerPoint

## 3. Data Pipeline & Methodology

### 🐍 Phase 1: Python (EDA & Cleaning)
*   **Missing Value Imputation:** Handled missing data in the `Review Rating` column by imputing values based on the median rating per product category.
*   **Feature Engineering:** 
    *   Binned ages into `age_group` (Young Adult, Middle-aged, Adult, Senior).
    *   Calculated `purchase_frequency_days`.
*   **Data Loading:** Cleaned data was exported to a PostgreSQL database using `SQLAlchemy` for structured querying.

### 🐘 Phase 2: SQL (Strategic Analysis)
Key business questions addressed via PostgreSQL:
*   **Revenue Segmentation:** Analyzed revenue by gender, identifying a 67% male vs. 33% female split.
*   **Customer Tiering:** Classified users into **New, Returning, and Loyal** segments.
*   **Discount Impact:** Identified "Discount-Dependent" products to evaluate margin protection strategies.

### 📊 Phase 3: Power BI (Visualization)
Developed an interactive 3-page dashboard:
1.  **Executive Overview:** High-level KPIs (Revenue, Subscription %, Avg. Rating).
2.  **Product Insights:** Deep dive into category performance and review correlations.
3.  **Shopping Behavior:** Analysis of shipping preferences and discount usage.

## 4. Key Insights & Business Recommendations
*   **Loyalty Gap:** 80% of the customer base (3,116) are "Loyal," but the "New User" segment is underperforming (83). **Recommendation:** Prioritize Top-of-Funnel marketing.
*   **Subscription Conversion:** Identified 2,518 repeat buyers who are not yet subscribers. **Recommendation:** Launch a "First-Month Free" loyalty campaign.
*   **Inventory Synergy:** Blouses, Pants, and Jewelry shared identical sales volumes. **Recommendation:** Implement "Complete Look" bundling to increase Average Order Value (AOV).

## 5. Repository Structure
```text
├── Data/               # Raw and Cleaned Datasets
├── Notebooks/          # Python Scripts for EDA & Cleaning
├── SQL_Queries/        # PostgreSQL scripts for business analysis
├── Dashboard/          # Power BI .pbix file and screenshots
└── README.md           # Project Documentation
