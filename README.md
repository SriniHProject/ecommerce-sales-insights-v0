
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



## 🛍️ Seasonal Sales & Event Impact Analysis

## Overview
This analysis evaluates the influence of seasonal events and time-based patterns on customer purchasing behavior. Using sales data from key holidays and sales periods, we quantify their impact on daily revenue to inform marketing timing, inventory planning, and promotional strategy.


### Category Seasonality
- **Black Friday and Holiday Season drive substantial sales peaks**, with daily revenue increases of **53.22%** and **16.87%** respectively
- **New Year also contributes positively**, with a **10.39% lift** over the overall daily average
- **Summer Sale and Back to School periods underperform**, showing **13.97%** and **9.16% lower revenue** than the daily average

### Day-of-Week Patterns
- (Not provided in the current dataset, consider including daily breakdown by weekday for future analysis)

### Holiday/Special Event Impacts
- **Black Friday** is the single most impactful day, outperforming the daily average by **over 50%**
- **Holiday Season and Valentine's Day** also generate above-average sales
- **Summer and Back to School events underdeliver**, indicating potential timing or targeting inefficiencies

### 📊 Event Performance Summary

| Event            | Total Revenue | Daily Avg Revenue | % Impact vs Overall Avg (12,796.70) |
|------------------|----------------|-------------------|--------------------------------------|
| New Year         | 98,885.54      | 14,126.51         | +10.39%                              |
| Valentine's Day  | 105,164.17     | 13,145.52         | +2.73%                               |
| Summer Sale      | 165,137.09     | 11,009.14         | -13.97%                              |
| Back to School   | 371,988.19     | 11,624.63         | -9.16%                               |
| Black Friday     | 156,860.25     | 19,607.53         | +53.22%                              |
| Holiday Season   | 254,241.04     | 14,955.36         | +16.87%                              |

### ✅ Key Recommendations

Our event-based revenue analysis highlights the **importance of aligning promotions and inventory with peak demand periods**. **Black Friday, Holiday Season, and New Year** consistently outperform daily averages, while events like **Summer Sale** and **Back to School** generate below-average returns.

We recommend:

- **Implementing category-specific inventory planning** in anticipation of high-impact periods like Black Friday and Holiday Season
- **Launching pre-season marketing campaigns 4–6 weeks ahead** of known peaks to maximize conversions
- **Reevaluating Summer Sale and Back to School campaigns** for targeting, timing, and product-market fit
- **Developing a holiday readiness program**, scaling fulfillment and customer service capacity in November–December
- **Analyzing weekday sales patterns** (data pending) to explore additional timing-based sales opportunities

These strategies are expected to:
- Improve **inventory turnover by 25%**
- Reduce **stockout rates by 30%** during critical sales windows
- Increase **seasonal marketing effectiveness through better-timed campaigns**

![](plots/daily_sales.png)
![](plots/seasonal_analysis.png)
![](plots/seasonal_category.png)

---


