# sql-data-analyst-portfolio-project-
An advanced SQL portfolio project building a retail data reporting layer.

---

🚀 **Advanced Retail Data Analytics & Reporting**

An advanced data analytics workflow using MySQL. Building upon foundational exploratory data analysis, this project utilizes complex SQL logic to transform raw retail metrics into a stakeholder-ready reporting layer.

---

🎯 **Project Objective**

The goal of this project is to elevate foundational data into strategic business intelligence using MySQL. By applying advanced SQL techniques like window functions and complex segmentations, this project builds automated, stakeholder-ready reports and "Customer 360" views that drive actionable decision-making.

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

**The 2013 Revenue Explosion (Cumulative Analysis Time-Series Trends)**: Cumulative and year-over-year analysis highlighted 2013 as a massive breakout year. Annual sales skyrocketed to $16.3 Million, nearly tripling the revenue of 2012 ($5.8M). This historic surge indicates highly successful scaling, marketing, or inventory expansion during that specific 12-month period.

**The "Bike Monopoly" (Part-to-Whole Analysis)**: Percentage contribution analysis confirmed that Bikes are not just the core of the business—they essentially are the business, accounting for 96.46% of total historical sales ($28.3M). Accessories (2.39%) and Clothing (1.16%) function purely as low-revenue, complementary add-ons.

**Product Lifecycle Dynamics (Performance Gap)**: By tracking year-over-year performance against lifetime historical averages, the data clearly identifies product breakouts and adoption phases. For example, the All-Purpose Bike Stand struggled below its historical average in 2012 (generating only $159), but saw a massive, successful adoption surge in 2013, skyrocketing to $37.6k in sales and far exceeding its benchmark.

**The Premium Product Pillar (Part-to-Whole Analysis Cost Segmentation)**: Segmenting products by cost revealed a massive revenue concentration. Out of the entire catalog, just 39 premium products (priced above $1,000) generated a staggering $23.8 Million. Meanwhile, the 110 entry-level products (priced below $100) generated only $1 Million, acting primarily as high-volume traffic drivers rather than profit centers.

**The Retention Bottleneck (Part-to-Whole Analysis Customer Segments)**: The customer segmentation model exposed a significant opportunity for lifecycle marketing. Out of the customer base, 14,828 users are classified as "New" (likely single-purchase or low-tenure buyers). The business currently relies on a highly valuable but much smaller core of 1,619 "VIPs" and 2,037 "Regulars" to sustain its metrics. Converting more "New" customers into recurring buyers is the primary lever for future growth.

---

💻 **How to Use This Repository**

The scripts file contains all the SQL scripts categorized by the methodology steps above.
Ensure you have a MySQL environment set up with the retail database schema imported.
Run the queries sequentially to follow the advanced analytical journey, culminating in the creation of the final report_customers database view.

---

**Acknowledgments:**

A huge thank you to Data with Baraa for the incredible tutorial series and for providing such high-quality, real-life materials to learn from.
