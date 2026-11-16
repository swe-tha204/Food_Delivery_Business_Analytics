# 🍔 Food Delivery Business Analytics

### End-to-End Data Analytics Project | Python • SQL • Power BI

## 📌 Project Overview

This project focuses on analyzing food delivery business operations to uncover meaningful insights related to customer behavior, revenue performance, restaurant operations, delivery efficiency, and customer satisfaction.

The project follows an end-to-end data analytics workflow using Python, SQL, and Power BI, starting from raw data cleaning and exploratory data analysis (EDA) to SQL-based business analysis and interactive dashboard development.

The objective is to transform raw food delivery data into actionable business insights that can support better operational and business decisions.

## 🎯 Business Objectives

- Analyze food delivery order trends and peak ordering hours.
- Evaluate revenue performance and Average Order Value (AOV).
- Identify high-performing restaurants and restaurant categories.
- Understand customer purchasing behavior and high-value customer segments.
- Analyze delivery performance and late delivery patterns.
- Investigate the relationship between traffic, weather, distance, and delivery time.
- Identify order cancellation trends and their major reasons.
- Evaluate customer satisfaction through ratings.
- Develop an interactive Power BI dashboard for business performance monitoring.

## 📊 Dataset Overview

**Dataset:** Food Delivery Orders and ETA Logistics Dataset

| Description | Details |
|---|---|
| Total Records | 50,000 orders |
| Total Columns | 37 |
| Analysis Period | October 1–30, 2025 |
| Completed Orders | 49,132 |
| Cancelled Orders | 868 |
| Unique Customers | 4,979 |
| Unique Restaurants | 250 |
| Unique Delivery Partners | 200 |

### Key Dataset Attributes

- Order Information – Order ID, order date, timestamp, hour, and day of week.
- Customer Information – Customer ID, age, customer type, and ratings.
- Restaurant Information – Restaurant ID, restaurant category, and ratings.
- Financial Information – Subtotal, discount, tax, service fee, delivery fee, tips, and order total.
- Delivery Information – Delivery distance, estimated delivery time, actual delivery time, and late delivery status.
- Operational Information – Traffic level, weather, delivery partner experience, and restaurant preparation time.
- Cancellation Information – Order status and cancellation reasons.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data analysis and data processing |
| Pandas | Data cleaning, manipulation, and EDA |
| NumPy | Numerical and statistical operations |
| Matplotlib | Data visualization |
| Jupyter Notebook | Interactive analysis and documentation |
| SQL | Business queries and data analysis |
| SQLite | Database management |
| Power BI | Interactive dashboard development |
| DAX | Custom KPI calculations and measures |

## 🔄 Project Workflow

### 1. Python – Data Cleaning & Exploratory Data Analysis

The raw dataset was imported into Python using Pandas and NumPy.

**Data Cleaning & Validation**
- Inspected dataset structure using `head()`, `info()`, and `describe()`.
- Checked and verified duplicate records and duplicate order IDs.
- Identified and investigated missing values.
- Converted date and timestamp columns into appropriate datetime formats.
- Validated numerical ranges and categorical values.
- Checked financial consistency using order-total calculations.
- Investigated delivery-time and late-delivery classification consistency.

**Data Quality Findings**
- No completely duplicated records were identified.
- No duplicate order IDs were identified.
- Missing values were investigated and found to be structurally related to order status.
- Financial calculations were validated, with negligible rounding differences.

**Exploratory Data Analysis (EDA)**

Performed analysis across the following business areas:

- Order demand by hour and day.
- Weekday vs. weekend order patterns.
- Revenue and Average Order Value.
- Restaurant and restaurant-category performance.
- Delivery-time distribution and late deliveries.
- Traffic and weather impact on delivery efficiency.
- Cancellation trends and cancellation reasons.
- Customer segmentation and high-value customer analysis.
- Customer, restaurant, and delivery-partner ratings.
- Correlation analysis between operational and customer-related variables.

**Data Visualization**

Created visualizations using Matplotlib to understand business trends, distributions, comparisons, and relationships.

### 2. SQL – Business Analysis Using SQLite

The cleaned dataset was loaded into an SQLite database.

**Database Details**
- Database: `food_delivery.db`
- Table: `food_delivery_orders`
- Records loaded: 50,000
- Columns: 37

Performed SQL-based business analysis using:

- SELECT, WHERE, ORDER BY
- GROUP BY and HAVING
- Aggregate functions: COUNT(), SUM(), AVG(), MIN(), MAX()
- CASE WHEN
- Subqueries
- Conditional aggregations
- Customer and restaurant performance analysis

**Business Analysis Areas**
- Order demand by hour and city.
- Revenue and Average Order Value.
- Restaurant revenue and order performance.
- Revenue by restaurant category.
- Customer-type revenue analysis.
- Delivery-time and late-delivery analysis.
- Traffic and weather impact.
- Cancellation rates and cancellation reasons.
- Customer ratings and satisfaction.

### 3. Power BI – Interactive Dashboard Development

The cleaned dataset was imported into Power BI to develop an interactive business analytics report.

**Dashboard Structure**

**Page 1 – Executive Overview**
- Overall business performance.
- Key Performance Indicator (KPI) cards.
- Order and revenue analysis.
- Customer and restaurant performance.

**Page 2 – Delivery, Operations & Customer Analysis**
- Delivery performance.
- Traffic and weather impact.
- Late delivery analysis.
- Cancellation analysis.
- Customer rating distribution.

**Dashboard Components**
- 6 KPI cards.
- 7 interactive slicers.
- 10 business-analysis visuals.
- Custom DAX measures for KPI calculations.
- Synchronized slicers across both report pages.
- Professional dashboard formatting and UI design.

## 💡 Key Business Insights & Findings

The analysis revealed the following important findings:

### 1. Order Demand Analysis
- 7 PM recorded the highest order volume with 4,746 orders.
- Thursday recorded the highest daily order volume with 8,472 orders.
- Weekdays accounted for approximately 73.29% of total orders.

**Business Insight:** Order demand was concentrated around lunch and evening hours, highlighting the importance of planning operational resources during peak periods.

### 2. Revenue Analysis
- Total revenue from completed orders: 1,874,176.57 monetary units.
- Average Order Value (AOV): 38.15 monetary units.
- Completed orders: 49,132.

**Business Insight:** Revenue and AOV provide important performance measures for evaluating business performance and customer spending patterns.

### 3. Restaurant Performance
- RES_0001 generated the highest revenue of approximately 286,626 monetary units.
- Burger was the highest-revenue restaurant category, generating approximately 538,745 monetary units.
- RES_0162 recorded the highest Average Order Value of 129.95 monetary units.

**Business Insight:** Restaurant performance varies depending on revenue, order volume, and average order value. These metrics should be evaluated together.

### 4. Delivery Performance
- Average actual delivery time: 35.15 minutes.
- Late delivery rate: 36.57%.
- High traffic was associated with an average delivery time of 39.89 minutes.
- Low traffic was associated with an average delivery time of 30.59 minutes.

**Business Insight:** Delivery efficiency is an important operational area, with traffic conditions associated with longer delivery times.

### 5. Weather Impact
- Clear weather: 33.56 minutes average delivery time.
- Rain: 39.16 minutes.
- Storm: 47.07 minutes.

**Business Insight:** Adverse weather conditions were associated with longer delivery times, indicating the importance of considering weather conditions in operational planning.

### 6. Cancellation Analysis
- Overall cancellation rate: approximately 1.74%.
- Total cancelled orders: 868.
- Driver Unassigned was the leading cancellation reason, accounting for 386 cancellations (44.47%).

**Business Insight:** Driver availability and assignment are important areas to investigate when analyzing order cancellations.

### 7. Customer Analysis
- Regular customers generated the highest customer-segment revenue.
- The top 10% of customers (495 customers) contributed 78.97% of total completed-order revenue.
- New customers recorded the highest Average Order Value at 40.72 monetary units.

**Business Insight:** A relatively small group of high-value customers contributed a significant share of revenue, highlighting the importance of understanding customer segments and purchasing behavior.

### 8. Customer Satisfaction
- Average customer rating: 4.30 / 5.
- Average restaurant rating: 4.21 / 5.
- Average delivery-partner rating: 4.50 / 5.
- Customer rating and actual delivery time showed a moderate negative correlation of -0.320.

**Business Insight:** Higher delivery times were associated with lower customer ratings, suggesting that delivery efficiency is an important factor to investigate when evaluating customer experience.

## 📈 Key Analytical Outcomes

| Business Metric | Result |
|---|---:|
| Total Orders | 50,000 |
| Completed Orders | 49,132 |
| Cancelled Orders | 868 |
| Total Revenue | 1,874,176.57 |
| Average Order Value | 38.15 |
| Average Delivery Time | 35.15 min |
| Late Delivery Rate | 36.57% |
| Cancellation Rate | 1.74% |
| Average Customer Rating | 4.30 / 5 |

## 📁 Repository Structure

```text
Food_Delivery_Business_Analytics/
│
├── Dataset/
│
├── Python/
│
├── SQL/
│
├── PowerBI/
│
├── Report/
│
└── README.md
```

## ⚠️ Project Limitations

- The dataset covers only October 1–30, 2025.
- Long-term customer retention cannot be reliably measured.
- Month-over-month and year-over-year growth analysis cannot be performed.
- Profitability cannot be calculated because restaurant cost and profit-margin information is unavailable.
- Correlation identifies relationships between variables but does not establish causation.

## 🏁 Conclusion

This project demonstrates an end-to-end data analytics workflow, transforming raw food delivery data into meaningful business insights using Python, SQL, and Power BI.

Through data cleaning, exploratory data analysis, SQL business queries, and interactive dashboard development, the project identified important patterns related to revenue performance, customer behavior, restaurant performance, delivery efficiency, cancellations, and customer satisfaction.

The final Power BI dashboard provides an interactive view of business performance through KPI cards, analytical visuals, and synchronized slicers.

This project strengthened practical skills in data preparation, exploratory analysis, SQL querying, data visualization, business analysis, and dashboard development.

---

## 👩‍💻 Author

**Swetha K**

Aspiring Data Analyst

**Technical Skills:** Python | SQL | Power BI | Excel | Statistics | Data Analytics

**GitHub:** [swe-tha204](https://github.com/swe-tha204)

---

⭐ If you find this project interesting, feel free to explore the repository and its contents.
