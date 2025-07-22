### 📊 Power BI Project – Retail Sales Dashboard (Blinkit)

A complete end-to-end Power BI dashboard project analyzing retail sales data, designed for business insights, performance trends, and category-wise analysis.

---

#### 🧩 Project Overview

This project focuses on building a real-time, interactive retail sales dashboard using Power BI. The dashboard offers insights into total sales, item performance, outlet analysis, and average ratings. It is inspired by real business use cases in e-commerce retail analytics.

---

#### 📁 Dataset Used

- **Source:** CSV/Excel (Imported)
- **Dataset:** Sales data including columns such as:
  - `Item Type`
  - `Outlet Size`
  - `Outlet Type`
  - `Location`
  - `Total Sales`
  - `Avg Sales`
  - `Ratings`

---

#### 📸 Dashboard Preview

> _Replace these with your actual screenshots from the project._

| Main Dashboard | Item Analysis | Outlet Performance |
|----------------|----------------|--------------------|
| ![MainDashboard](screenshots/main_dashboard.png) | ![ItemAnalysis](screenshots/item_analysis.png) | ![OutletPerformance](screenshots/outlet_performance.png) |

---

#### 🔧 Key Power BI Features Used

- Power Query Editor for data cleaning
- DAX formulas for KPI calculations
- Slicers, filters, and dynamic visuals
- KPI cards, clustered bar chart, doughnut charts
- Responsive and color-coded theme

---

#### 🧮 Key DAX Measures

```dax
Total Sales = SUM(Sales[Sales_Amount])

Avg Sales = AVERAGE(Sales[Sales_Amount])

High Rating Products = CALCULATE(COUNTROWS(Sales), Sales[Rating] >= 4.0)
```

---

#### ⚙ Sample M-Code (Power Query)

```m
= Table.TransformColumnTypes(Source,{{"Sales_Amount", Currency.Type}, {"Date", type date}})
```

---

#### 📊 Dashboard KPIs

- 📦 **Total Sales**
- 🛒 **Average Sales**
- ⭐ **Average Rating**
- 🏪 **Outlet Type Comparison**
- 🦃 **Top Item Types by Revenue**

---

#### 💡 Insights

- **Tier 3 outlets** contributed the highest revenue.
- Items with **medium fat content** saw more consistent ratings.
- Supermarket Type 1 outlets showed the highest average sales.

---

#### 🛠 Tools & Technologies

- Power BI (Desktop)
- Power Query
- DAX
- Excel/CSV as source

---

#### 📁 Folder Structure

```
📁 Blinkit_PowerBI_Project
│
├── 📁 dataset
│   └── retail_sales.csv
│
├── 📁 screenshots
│   ├── main_dashboard.png
│   ├── item_analysis.png
│   └── outlet_performance.png
│
├── 📁 pbix_file
│   └── Blinkit_Sales_Analysis.pbix
│
└── README.md
```

---

#### 📌 How to Use

1. Clone this repo
2. Open the `.pbix` file in Power BI Desktop
3. Connect to the provided dataset if needed
4. Explore and interact with visual elements
