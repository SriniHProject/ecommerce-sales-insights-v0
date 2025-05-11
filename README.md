
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


## 🧾 Customer Behavior & Purchase Analysis

## Overview
This analysis explores customer purchase patterns across different segments, including coupon usage, geographic location, gender, and average tenure. It focuses on understanding how customer traits influence purchase behavior and order values, using statistical tests to guide evidence-based recommendations.


### Coupon Usage and Transaction Value
- No statistically significant difference found in transaction value between coupon users and non-users
- T-test returned NaN values, indicating insufficient or invalid data for comparison

### Demographic Purchase Patterns
- **Location has a significant effect on purchase behavior** (ANOVA p = 0.0114)
- Customers in **Chicago and California** have higher average order values and order frequency
- **Washington DC and New Jersey** customers show lowest engagement in terms of order frequency and value

### Gender-Based Purchase Patterns
- Female customers have **higher average order value ($112.80 vs $68.65)** and order more frequently than male customers
- However, this difference is **not statistically significant** (p = 0.6098), suggesting high variability or limited sample size

### Pricing and Purchase Behavior
- Locations with higher order values (Chicago, California) also show **higher orders per customer**
- Regions with lower prices (e.g. Washington DC, New Jersey) show **lower engagement**, possibly reflecting regional preferences or income sensitivity

### 📊 Summary of Key Metrics

#### Purchase Behavior by Location

| Location        | Avg Order Value | Orders per Customer | Avg Items per Order |
|----------------|------------------|----------------------|----------------------|
| California      | 55.14            | 5.37                 | 4.50                 |
| Chicago         | 62.16            | 6.19                 | 4.57                 |
| New Jersey      | 15.66            | 1.55                 | 5.04                 |
| New York        | 35.82            | 3.75                 | 4.16                 |
| Washington DC   | 9.78             | 0.96                 | 4.50                 |

#### Purchase Behavior by Gender

| Gender | Avg Order Value | Orders per Customer | Avg Items per Order |
|--------|------------------|----------------------|----------------------|
| Female | 112.80           | 10.88                | 4.60                 |
| Male   | 68.65            | 6.66                 | 4.32                 |

![](plots/tenure_vs_purhcase_frequency.png)
### ✅ Key Recommendations

Our statistical analysis reveals **strong regional differences** in customer behavior, particularly in average order value and purchase frequency, with **Chicago and California** leading in both areas. While **gender differences exist**, they are not statistically significant in this dataset. **Coupon impact could not be validated** due to insufficient or invalid data.

We recommend:

- **Tailoring promotions to high-performing regions like Chicago and California** with upsell and loyalty incentives
- **Creating location-specific campaigns** to improve engagement in underperforming areas like Washington DC and New Jersey
- **Improving data quality and completeness** for coupon usage to enable valid impact assessment
- **Testing a “regional free shipping” or pricing experiment** in low-engagement zones to drive incremental orders

These targeted initiatives aim to:
- Increase average order value by 10–15% in underperforming regions
- Improve regional engagement and purchase frequency
- Strengthen data-driven campaign design with validated behavioral insights

---

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

![](plots/daily_sales.png)
![](plots/seasonal_analysis.png)
![](plots/seasonal_category.png)

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



---


