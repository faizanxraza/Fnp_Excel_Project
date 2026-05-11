# 🌸 Ferns and Petals (FNP) — Sales Analysis Dashboard

> An interactive Excel-based sales analytics dashboard that analyses Ferns and Petals' order, customer, and product data to uncover trends in sales performance, customer behaviour, and occasion-based demand.

## 📌 Overview

**Ferns and Petals (FNP)** is a leading gifting brand that delivers products for occasions like **Diwali, Raksha Bandhan, Holi, Valentine's Day, Birthdays, and Anniversaries**.

This project takes FNP's raw sales dataset and transforms it into a single, interactive **Sales Analysis Dashboard** built in **Microsoft Excel** using **Power Query, Power Pivot, and DAX**. The dashboard helps leadership quickly answer key business questions around revenue, top products, customer spend, delivery efficiency, and occasion-based demand — supporting better decisions on sales strategy and customer satisfaction.


## ❓ Problem Statement

FNP wanted to better understand its sales performance and customer behaviour to improve sales strategy and optimise the customer experience. The dashboard was built to answer **10 key business questions**:

1. **Total Revenue** — Identify the overall revenue
2. **Average Order and Delivery Time** — Evaluate how long orders take to deliver
3. **Monthly Sales Performance** — Examine how sales fluctuate across the months of 2023
4. **Top Products by Revenue** — Determine which products are the top revenue generators
5. **Customer Spending Analysis** — Understand how much customers spend on average
6. **Sales Performance by Top 5 Products** — Track the sales of the top 5 products
7. **Top 10 Cities by Number of Orders** — Find which cities place the most orders
8. **Order Quantity vs. Delivery Time** — Analyse whether higher order quantities impact delivery times
9. **Revenue Comparison Between Occasions** — Compare revenue across different occasions
10. **Product Popularity by Occasion** — Identify which products are most popular during specific occasions


## 📂 Dataset

- **Source:** Kaggle (public Ferns and Petals dataset)
- **Records:** 1,000+ orders
- **Period:** 2023 – 2024
- **Key Fields:**
  - `Order ID`
  - `Order Date` & `Delivery Date`
  - `Product Name`
  - `Category` (Cake, Colors, Mugs, Plants, Raksha Bandhan, Soft Toys, Sweets)
  - `Occasion` (Anniversary, Birthday, Diwali, Holi, Raksha Bandhan, Valentine's Day, etc.)
  - `City`
  - `Order Quantity`
  - `Revenue / Order Amount`


## 🛠️ Tools and Technologies

| Tool | Purpose |
|------|---------|
| **Microsoft Excel** | Primary platform for the dashboard |
| **Power Query Editor** | Data extraction, cleaning, and transformation |
| **Power Pivot** | Data modelling and relationship building |
| **DAX (Data Analysis Expressions)** | Calculated columns & measures (KPIs) |
| **Pivot Tables & Pivot Charts** | Aggregations and visualisations |
| **Slicers & Timelines** | Interactive filtering by Occasion and Date |


## 🧪 Methods

The project followed a structured analytics workflow:

1. **Data Extraction & Cleaning (Power Query)**
   - Imported the raw FNP dataset into Excel via Power Query
   - Handled missing values, corrected data types, and standardised text fields
   - Created derived columns such as Order Hour, Month, Year, and Order-to-Delivery duration

2. **Data Modelling (Power Pivot)**
   - Loaded cleaned data into the Power Pivot data model
   - Built relationships between fact and lookup tables
   - Optimised the model for performance and reusability

3. **KPI & Measure Creation (DAX)**
   - Wrote DAX measures for `Total Orders`, `Total Revenue`, `Avg. Customer Spend`, and `Avg. Order-to-Delivery Time`
   - Built measures supporting top-N analysis (Top 5 Products, Top 10 Cities)
   - Created occasion- and category-level revenue measures

4. **Dashboard Design**
   - Designed a single-page, purple-themed dashboard layout
   - Built 7 visualisations covering occasions, categories, time, products, and geography
   - Added slicers for **Occasion** and **Date (Order/Delivery)** to enable interactive exploration


## 💡 Key Insights

Mapping the analysis directly back to the 10 business questions:

| # | Business Question | Key Finding |
|---|-------------------|-------------|
| 1 | Total Revenue | **$3,520,984** across 1,000 orders |
| 2 | Avg. Order-to-Delivery Time | **5.53 days** on average |
| 3 | Monthly Sales Performance | **February (~$700K)** and **August (~$740K)** are the strongest months; April–July are weakest |
| 4 | Top Products by Revenue | **Magnam Set** leads, followed by Quia Gift and Dolores Gift |
| 5 | Avg. Customer Spend | **$3,520.98** per order |
| 6 | Top 5 Products Performance | Top 5 SKUs contribute **~$544K (≈15%)** of total revenue |
| 7 | Top 10 Cities by Orders | **Imphal, Dhanbad, Kavali, Haridwar** lead — strong Tier-2/Tier-3 traction |
| 8 | Order Quantity vs. Delivery Time | Higher order quantities show only a **mild impact** on delivery time |
| 9 | Revenue by Occasion | **Anniversary (~$675K)** and **Raksha Bandhan (~$625K)** dominate; **Diwali (~$315K) underperforms** |
| 10 | Product Popularity by Occasion | Sweets and Colors peak during Holi/Diwali; Soft Toys and Cakes dominate Birthdays and Anniversaries |


## 📈 Dashboard / Model / Output

The final dashboard includes:

- ✅ **4 KPI cards** — Total Orders, Total Revenue, Avg. Delivery Time, Avg. Customer Spend
- ✅ **Revenue by Occasion** (bar chart)
- ✅ **Revenue by Category** (bar chart)
- ✅ **Revenue by Hour of Order** (line chart)
- ✅ **Revenue by Month** (line chart)
- ✅ **Top 5 Products by Revenue** (bar chart)
- ✅ **Top 10 Cities by Order** (bar chart)
- ✅ **Interactive slicers** — Occasion, Order Date, Delivery Date


## ▶️ How to Run This Project

1. **Clone or download** this repository:
   ```bash
   git clone https://github.com/<your-username>/fnp-sales-analysis-dashboard.git
   ```

2. **Open the Excel file** `FNP_Sales_Analysis_Dashboard.xlsx` in Microsoft Excel
   *(Excel 2016 or later recommended for full Power Pivot / Power Query support)*

3. **Enable** the following Excel add-ins if not already active:
   - Power Pivot
   - Power Query (built into Excel 2016+)

4. **Refresh the data:**
   - Go to `Data` → `Refresh All`
   - This will reload the dataset from the `/data` folder via Power Query

5. **Interact with the dashboard:**
   - Use the **Occasion** slicer and **Date** timelines to filter views
   - Hover over charts for tooltips and detailed values

---

## ✅ Results & Conclusion

The FNP Sales Analysis Dashboard successfully answers all 10 business questions in a single, interactive view. Three core takeaways stand out:

1. **Revenue is heavily concentrated** in a few categories (Colors, Soft Toys, Sweets) and two peak months (February, August) — meaning planning and inventory should mirror this rhythm rather than spreading investment evenly across the year.
2. **Customer behaviour is evening-led**, with the 6 PM – 8 PM window driving the highest order intent — a clear signal for ad-spend timing and push-notification scheduling.
3. **Tier-2 and Tier-3 cities are quietly leading order volume**, with cities like Imphal and Dhanbad outperforming many Tier-1 metros — a strategic asset worth deepening further.

A clear gap surfaced too: **Diwali revenue is surprisingly low** for such a major Indian festival, signalling either a missed marketing window or an assortment that isn't aligned to Diwali gifting expectations — a priority area for the next festive cycle.

## 🚀 Future Work

- 🔮 **Add forecasting / predictive analysis** to project future revenue by month, occasion, and category
- 📊 Incorporate **trend lines and confidence intervals** into the existing time-based charts
- 🧠 Explore **what-if scenario analysis** using DAX and Excel's data tables
- 🔄 Add **customer cohort analysis** and **repeat-purchase metrics** in a future iteration
- 📉 Layer in **margin and return-rate data** to evolve from a sales view into a full commercial dashboard

## 👤 Author & Contact

**Faizan Raza**
Data Analytics Enthusiast | Excel • Power BI • SQL • Python

- 💼 **LinkedIn:** https://www.linkedin.com/in/faizan-raza-fai20/
- 🐙 **GitHub:** https://github.com/faizanxraza
- 📧 **Email:** faizanraza0660@gmail.com


*If you found this project helpful or insightful, consider giving it a star on GitHub!*
