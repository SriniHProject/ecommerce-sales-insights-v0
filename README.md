
# 📊 E-Commerce Marketing & Sales Analysis (2019)
### 🧩 Business Problem & Case Study

In a rapidly growing e-commerce market, the company seeks to **maximize customer acquisition**, **enhance retention**, and **optimize revenue**, while ensuring **efficient marketing spend**. Despite year-round sales activity, fluctuations in customer growth, inconsistent marketing ROI, and uneven revenue contributions from different customer segments present critical business challenges.

This project leverages a full year (**2019**) of transaction, marketing, and customer data to address over 20 specific business questions spanning:

- 📈 Monthly acquisition and retention trends  
- 💸 Coupon effectiveness and purchase behavior  
- 🧠 Customer segmentation and lifetime value  
- 📦 Product/category performance and seasonality  
- 📊 Marketing ROI and pricing/delivery optimization  

Through **exploratory data analysis (EDA)**, **statistical testing**, and **segmentation techniques**, we aim to deliver **insightful, actionable strategies** to improve customer engagement and support sustainable revenue growth.


# 📦 Dataset Overview
All data spans **January 1, 2019 to December 31, 2019**.

| **Dataset**             | **Description**                                | **Key Fields**                                                  |
|-------------------------|------------------------------------------------|------------------------------------------------------------------|
| `Online_Sales.csv`      | Transaction-level sales data                   | `CustomerID`, `Transaction_Date`, `Product_Category`, `Quantity`, `Avg_Price`, `Coupon_Status`, `Delivery_Charges` |
| `Customers_Data.csv`    | Customer demographics and tenure               | `Gender`, `Location`, `Tenure_Months`                            |
| `Discount_Coupon.csv`   | Coupon availability by category and month      | `Month`, `Product_Category`, `Discount_pct`                      |
| `Marketing_Spend.csv`   | Daily marketing spend (online & offline)       | `Date`, `Offline_Spend`, `Online_Spend`                          |
| `Tax_Amount.csv`        | GST rate by product category                   | `Product_Category`, `GST`                                       |

All data spans January 1, 2019 to December 31, 2019.

### 📅 Monthly Acquisition Trends

- **Highest acquisition month**: January, with **215 new customers**
- **Lowest acquisition month**: November, with only **68 new customers**
- **Coefficient of Variation (CV)** in acquisition: **0.36**, indicating **high month-to-month volatility** in customer acquisition patterns

Such variation causes challenges in resource planning, budget forecasting, and consistent sales pipeline development.

![Monthly Customer Acquisition Histogram](plots/monthly_acquisition_hist.png)




---

## ✅ Recommendations

Our analysis reveals significant variability in monthly customer acquisition. January outperforms with 215 new customers (40% above average), while November significantly underperforms with just 68 (43% below average). The high coefficient of variation (0.36) highlights a need for strategic intervention to ensure year-round acquisition consistency.

We recommend:

- 📬 **Launching a Q4 “Reactivation” campaign**: Incentivize dormant customers or lapsed browsers in slower months like November with personalized reactivation emails or flash discounts.
- 💰 **Reallocating 20% of marketing budget** from high-performing months to February, September, and November, where acquisition drops significantly.
- 🎯 **Introducing limited-time offers** like first-purchase bundles or trial products targeted at new users during historically low-acquisition periods.
- 📈 **Running performance forecasting models** to pre-emptively boost acquisition before anticipated dips based on seasonal trends.

By implementing these strategies, the company can **reduce acquisition volatility by 25–30%**, leading to **more stable growth and better operational efficiency** throughout the year.


## Business Case Overview
[Brief introduction to the business case and problem statement - focus on the e-commerce company's need to leverage data for customer acquisition, retention, and revenue optimization]

## Data Description
The analysis uses e-commerce transaction data from January to December 2019, comprising multiple datasets:

1. **Online_Sales.csv**: Transaction-level data with customer purchases, pricing, and coupon usage
2. **Customers_Data.csv**: Customer demographics including gender, location, and tenure
3. **Discount_Coupon.csv**: Details of discount coupons by category and month
4. **Marketing_Spend.csv**: Daily marketing expenditure across online and offline channels
5. **Tax_Amount.csv**: GST tax rates by product category

## Key Findings

### Customer Acquisition
- [Key finding about monthly acquisition patterns]
- [Key finding about highest/lowest acquisition months]
- [Key finding about acquisition strategies]

### Customer Retention
- [Key finding about retention patterns]
- [Key finding about customer behavior during high retention periods]
- [Key finding about strategies to improve retention]

### Revenue Analysis
- [Key finding about new vs. existing customer revenue contribution]
- [Key finding about coupon impact on revenue]
- [Key finding about top-performing products]

### Marketing Effectiveness
- [Key finding about marketing ROI]
- [Key finding about optimal marketing allocation]
- [Key finding about channel effectiveness]

### Customer Segmentation
- [Key finding about RFM segments and their characteristics]
- [Key finding about segment revenue contribution]
- [Key finding about targeted strategies]

### Cohort Analysis
- [Key finding about retention patterns by cohort]
- [Key finding about lifetime value trends]
- [Key finding about acquisition quality over time]

### Statistical Insights
- [Key finding about coupon usage and transaction value]
- [Key finding about demographic purchase patterns]
- [Key finding about tenure and purchase behavior]
- [Key finding about pricing factors and customer behavior]

### Seasonal Trends
- [Key finding about category seasonality]
- [Key finding about day-of-week patterns]
- [Key finding about holiday/special event impacts]

## Recommendations

### Acquisition Strategy
- [Recommendation for improving acquisition]
- [Recommendation for targeting specific customer types]

### Retention Strategy
- [Recommendation for improving overall retention]
- [Recommendation for customer segment-specific retention approaches]

### Revenue Optimization
- [Recommendation for pricing strategy]
- [Recommendation for coupon and discount approach]
- [Recommendation for product focus]

### Marketing Strategy
- [Recommendation for marketing spend allocation]
- [Recommendation for campaign timing]
- [Recommendation for channel optimization]

### Seasonal Strategy
- [Recommendation for capitalizing on seasonal trends]
- [Recommendation for addressing slow periods]

## Implementation Roadmap
1. [First priority action item]
2. [Second priority action item]
3. [Third priority action item]
4. [Additional action items...]

## Data Science Approach
The analysis utilized various techniques including:
- Exploratory data analysis
- Time series analysis
- RFM customer segmentation
- Cohort analysis
- Statistical hypothesis testing
- Correlation analysis

## Visualizations
[Include thumbnails of key visualizations with brief descriptions]

## Repository Structure
- `E-commerce_Analysis.ipynb`: Main Jupyter notebook with complete analysis
- `data/`: Directory containing the datasets
- `images/`: Directory containing exported visualizations
- `README.md`: This document

## Conclusion
[Brief summary of the most important findings and their potential impact on the business]
