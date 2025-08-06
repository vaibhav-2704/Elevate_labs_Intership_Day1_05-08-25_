**# 📊 Sales Performance Dashboard – Power BI Internship Project**

**# 📁 Project Overview**
This project was completed as part of my internship with a focus on creating professional-level dashboards using Power BI. 
The goal was to analyze sales performance and build compelling, 
insight-driven visualizations while following strict dashboarding principles like avoiding clutter, 
focusing on business insights, and using the right visuals.

**🎯 Objectives**
- Clean and transform the Superstore sales dataset

- Use the right charts and KPIs to highlight business insights

- Build a compelling data story

- Follow real-world best practices in layout, colors, slicers, and formatting

**📦 Dataset Info**
- Source: https://www.kaggle.com/datasets/vivek468/superstore-dataset-final

**Columns Used:**
- Order Date Segment, Category, Sub-Category, Sales, Quantity, Profit, Discount, Region etc.

**🧼 Data Cleaning Steps**
- Converted Order Date and Ship Date columns to Date type

- Added Month Name and Month Number columns

- Verified column types for accurate aggregation

- Removed unnecessary columns (e.g., Row ID)

- Ensured data granularity and formatting for DAX-ready use

**📊 Dashboards Overview**

🧩 Dashboard 1 – Overview & Growth Trends
💡 Focus: Sales, Profit, Discount Trends

✅ KPIs:

- Total Sales 💰

- Total Profit 📈

- Total Discount %

📈 Visualizations:

- Line Chart → Month-wise Sales & Profit Trend

- Clustered Bar Chart → Segment-wise Profit Margin

- Donut Chart → Sales Distribution by Category

🎛️ Slicers:

- Segment

- Category

🧠 Insights:

- This dashboard offers a clear view of how the business is performing over time, which segments drive profit, and how discounts affect profitability. Interactive slicers allow focused analysis.

**📊 Dashboard 2 – Performance Deep Dive**

💡 Focus: Sub-category, Segment Profitability, Monthly Profit Flow

✅ KPIs:

- Total Discount %

- Top Category

- Top Segment

📈 Visualizations:

- Clustered Bar Chart → Segment-wise Profit Margin

- Lollipop Chart → Top Sub-Category Sales

- Waterfall Chart → Month-wise Profit Flow

🎛️ Slicers:

- Segment

- Category

🧠 Insights:
- This dashboard presents deeper business insights with clean, non-repetitive visuals.

- It highlights segment-level profitability, sub-category leaders, and monthly profit shifts. 
Slicers enhance interactivity for targeted storytelling.

| **Measure Name**   | **DAX Formula**                                                                                                                                                      |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Total Sales`      | `SUM('Sample - Superstore'[Sales])`                                                                                                                                  |
| `Total Profit`     | `SUM('Sample - Superstore'[Profit])`                                                                                                                                 |
| `Total Discount %` | `DIVIDE(SUM('Sample - Superstore'[Discount]), COUNTROWS('Sample - Superstore')) * 100`                                                                               |
| `Profit Margin %`  | `DIVIDE(SUM('Sample - Superstore'[Profit]), SUM('Sample - Superstore'[Sales])) * 100`                                                                                |
| `Top Category`     | `CALCULATE(FIRSTNONBLANK('Sample - Superstore'[Category], 1), TOPN(1, VALUES('Sample - Superstore'[Category]), CALCULATE(SUM('Sample - Superstore'[Sales])), DESC))` |
| `Top Segment`      | `CALCULATE(FIRSTNONBLANK('Sample - Superstore'[Segment], 1), TOPN(1, VALUES('Sample - Superstore'[Segment]), CALCULATE(SUM('Sample - Superstore'[Sales])), DESC))`   |


**🧠 Key Learnings**

- DAX writing for KPI calculations

- Dashboard structuring using real-world layout standards

- Visual choice based on insight priority (not just aesthetics)

- GitHub project hosting & markdown writing

- Storytelling for data interpretation


**👨‍💻 Author**
**Saloora Vaibhav**

📧 www.linkedin.com/in/vaibhav-saloora-25a3562b2



