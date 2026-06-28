# advanced-sql-retail-analytics-reporting-
This project is the advanced analysis and reporting-layer phase of a two-part SQL portfolio project. It builds on the initial EDA work by applying CTEs, window functions, segmentation logic, cumulative analysis, and Customer 360 reporting views.

---

🚀 **Advanced Retail Data Analytics & Reporting**

An advanced data analytics workflow using MySQL. Building upon foundational exploratory data analysis, this project utilizes complex SQL logic to transform raw retail metrics into a stakeholder-ready reporting layer.

---

🎯 **Project Background**

This project uses a simulated retail dataset representing a global bicycle and cycling gear business.

The company processes significant transaction volumes, but its historical sales data, customer lifecycle behaviors, and product performance metrics have been previously underutilized. This project thoroughly analyzes and synthesizes this data to uncover critical insights that will improve the company's customer retention and overall commercial success.

Insights and recommendations are provided on the following key areas:

- **Sales Trends Analysis:** Evaluation of historical sales patterns and revenue growth, specifically analyzing the massive revenue surge during the 2013 fiscal year.
- **Product Level Performance:** An analysis of the company's product catalog, focusing on the revenue concentration of premium products versus entry-level traffic drivers.
- **Customer Retention & Segmentation:** An assessment of the customer lifecycle, identifying retention bottlenecks and the dependency on "VIP" and "Regular" recurring buyers.
- **Regional Comparisons:** An evaluation of sales volume and customer acquisition across major geographic markets, particularly the US and Australia.

---

🛠️ **Data Structure**

The database consists of three relational tables structured in a Star Schema. The core sales fact table captures over **60,400 item-level transaction records** (spanning 27,000+ distinct orders), supported by comprehensive customer and product dimension tables.

<img width="671" height="321" alt="ERD" src="https://github.com/user-attachments/assets/8312d358-630b-47a1-ba30-645d99ede03f" />

---

🛠️ **Tools & Techniques Used**

SQL Dialect: MySQL

Techniques: Window Functions (OVER(), PARTITION BY), Common Table Expressions (CTEs), Advanced Aggregations, CASE WHEN logic for segmentation, and complex Date/Time calculations.

---

🗺️ **Analytical Methodology**

This project follows a structured, real-world advanced analytics roadmap to explore the dataset step-by-step:

**Changes Over Time**: Tracking seasonality, monthly sales trends, and historical revenue growth.

**Cumulative Analysis**: Using window functions to calculate running totals and revenue build-up over time.

**Performance Analysis**: Benchmarking current product metrics against historical averages to identify growth or decline (e.g., finding the "Performance Gap").

**Part-to-Whole Analysis**: Determining category market share and percentage contributions to the grand total.

**Data Segmentation**: Bucketing customers and products into targeted business tiers (e.g., VIP vs. Regular, Price Ranges).

**Final Reporting**: Consolidating all KPIs into a single, optimized "Customer 360" database view ready for BI tool integration.

---

💡 **Key Business Insights Discovered**

**Significant Revenue Growth in 2013 (Cumulative Analysis Time-Series Trends)**: Cumulative and year-over-year analysis highlighted 2013 as a massive breakout year. Annual sales skyrocketed to $16.3 Million, nearly tripling the revenue of 2012 ($5.8M). This historic surge indicates highly successful scaling, marketing, or inventory expansion during that specific 12-month period.

**Revenue Concentration in the Bike Category (Part-to-Whole Analysis)**: Percentage contribution analysis confirmed that Bikes represent the overwhelming majority of historical revenue, accounting for 96.46% of total historical sales ($28.3M). Accessories (2.39%) and Clothing (1.16%) function purely as low-revenue, complementary add-ons.

**Product Lifecycle Dynamics (Performance Gap)**: By tracking year-over-year performance against lifetime historical averages, the data clearly identifies product breakouts and adoption phases. For example, the All-Purpose Bike Stand struggled below its historical average in 2012 (generating only $159), but saw a massive, successful adoption surge in 2013, skyrocketing to $37.6k in sales and far exceeding its benchmark.

**The Premium Product Pillar (Part-to-Whole Analysis Cost Segmentation)**: Segmenting products by cost revealed a massive revenue concentration. Out of the entire catalog, just 39 premium products (priced above $1,000) generated $23.8M in historical revenue. Meanwhile, the 110 entry-level products (priced below $100) generated only $1 Million, acting primarily as high-volume traffic drivers rather than profit centers.

**The Retention Bottleneck (Part-to-Whole Analysis Customer Segments)**: The customer segmentation model exposed a significant opportunity for lifecycle marketing. Out of the customer base, 14,828 users are classified as "New" (likely single-purchase or low-tenure buyers). The business currently relies on a highly valuable but much smaller core of 1,619 "VIPs" and 2,037 "Regulars" to sustain its metrics. Converting more "New" customers into recurring buyers is the primary lever for future growth.

---

💻 **How to Use This Repository**

The scripts file contains all the SQL scripts categorized by the methodology steps above.
Ensure you have a MySQL environment set up with the retail database schema imported.
Run the queries sequentially to follow the advanced analytical journey, culminating in the creation of the final report_customers database view.

---

**Acknowledgments:**

A huge thank you to Data with Baraa for the incredible tutorial series and for providing such high-quality, real-life materials to learn from.
