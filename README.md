# 🛍️ Retail Sales Analytics Dashboard
### *An End-to-End Data Analytics Project using Python · SQL · Power BI*

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GIVEN-CHINYAMA/retail-sales-analytics-dashboard/blob/main/retail_sales_analytics_dashboard.ipynb)
[![View on nbviewer](https://img.shields.io/badge/View-nbviewer-orange?style=flat&logo=jupyter)](https://nbviewer.org/github/GIVEN-CHINYAMA/retail-sales-analytics-dashboard/blob/main/retail_sales_analytics_dashboard.ipynb)
[![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat&logo=python&logoColor=white)](https://python.org)
[![SQL](https://img.shields.io/badge/SQL-SQLite-003B57?style=flat&logo=sqlite&logoColor=white)](https://sqlite.org)
[![PowerBI](https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=flat&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![Status](https://img.shields.io/badge/Status-Complete-2ecc71?style=flat)](https://github.com/GIVEN-CHINYAMA/retail-sales-analytics-dashboard)

**Author:** Given Chinyama
**Institution:** Kwame Nkrumah University
**Date:** April 2026
**GitHub:** [github.com/GIVEN-CHINYAMA](https://github.com/GIVEN-CHINYAMA)

---

## 👆 Click "Open in Colab" Above to View the Full Notebook

> GitHub cannot render large notebooks with embedded visualisations. Click the **Open in Colab** badge above to view the complete project with all code, outputs, and professional charts — no setup required.

---

## 📊 Executive KPI Summary (2021–2025)

| KPI | Value |
|---|---|
| 💰 **Total Revenue** | £ See notebook output |
| 📈 **Total Profit** | £ See notebook output |
| 🧾 **Total Orders** | 50,000 transactions |
| 📦 **Units Sold** | See notebook output |
| 📊 **Avg Order Value** | See notebook output |
| 💹 **Avg Profit Margin** | See notebook output |
| 🏪 **Stores Analysed** | 8 stores across 6 regions |
| 🛍️ **Product Categories** | 6 categories · 43 products |

---

## 📅 Annual Revenue Highlights

| Year | Performance |
|---|---|
| 2021 | Baseline year — full annual data |
| 2022 | Year-over-Year growth computed via SQL CTE |
| 2023 | Seasonal peaks confirmed in November–December |
| 2024 | Regional expansion effect visible in store data |
| 2025 | Full 5-year trend analysis completed |

> 🏆 **November and December consistently drive the highest monthly revenue** across all 5 years — confirming strong seasonal demand patterns in retail.

---

## 📁 Project Overview

Retail businesses generate enormous volumes of transactional data every day. Without proper analytics infrastructure, this data sits idle — a wasted asset. This project builds a **complete retail analytics pipeline** that transforms 50,000 raw sales transactions into actionable business intelligence and a professional **Power BI dashboard**.

This project demonstrates the **full data analyst and data scientist workflow** — from raw data through SQL querying, Python EDA, and a Power BI executive dashboard.

### Why This Project Stands Out

Unlike most dashboard projects that use pre-cleaned Kaggle datasets, this project:
- **Generates realistic retail data** with embedded seasonality, regional variation, and product-level pricing — mirroring what real retail systems produce
- **Uses SQL (SQLite)** for all business aggregations — including CTEs and year-over-year growth calculations
- **Combines three tools** in one pipeline — Python, SQL, and Power BI — the exact stack used by data teams in retail, banking, and FMCG
- **Delivers business recommendations** framed for executive stakeholders — not just charts

---

## 🔍 Problem Statement

> *"How is the business performing, which products and regions drive the most value, and where should leadership focus to maximise profitability?"*

Retail leadership teams need a reliable analytics system that can:
- **Track revenue and profit** across time, products, stores, and regions
- **Identify seasonal patterns** to inform stock and staffing decisions
- **Rank store and regional performance** for resource allocation
- **Analyse customer behaviour** to guide loyalty and retention strategy
- **Measure discount impact** on profitability before campaign launches
- **Deliver all of this in a single dashboard** that any executive can use

---

## 📦 Dataset

| Property | Details |
|---|---|
| **Type** | Synthetic retail transactions — realistic pricing, seasonality, and regional distribution |
| **Records** | 50,000 transactions |
| **Period** | January 2021 — December 2025 (5 years) |
| **Stores** | 8 stores across 6 Zambian regions |
| **Categories** | Electronics · Clothing · Home & Kitchen · Books · Sports · Beauty |
| **Products** | 43 unique products with real-world price ranges |
| **Features** | TransactionID · Date · CustomerID · Product · Category · Store · Region · Quantity · UnitPrice · UnitCost · DiscountPct · Revenue · Cost · Profit · ProfitMargin · PaymentMethod |

### Engineered Features

| Feature | Description |
|---|---|
| `Revenue` | UnitPrice × Quantity × (1 − Discount%) |
| `Cost` | UnitCost × Quantity |
| `Profit` | Revenue − Cost |
| `ProfitMargin` | (Profit / Revenue) × 100 |
| `Year` | Extracted from transaction date |
| `Month` | Extracted from transaction date |
| `Quarter` | Q1–Q4 derived from date |
| `DayOfWeek` | Monday–Sunday derived from date |
| `WeekOfYear` | ISO week number |

---

## 🗂️ Project Stages

| Stage | Description |
|---|---|
| Stage 1 | Environment setup — library installation and imports |
| Stage 2 | Data generation — 50,000 realistic retail transactions with seasonality |
| Stage 3 | Data overview — shape, dtypes, statistical summary |
| Stage 4 | Data cleaning — business rule validation, deduplication, type enforcement |
| Stage 5 | SQL database setup — load into SQLite, run 8 business queries |
| Stage 6 | EDA — KPI cards, distributions, overview statistics |
| Stage 7 | Sales trend analysis — monthly/annual revenue, YoY growth, seasonality |
| Stage 8 | Product & category analysis — top 15 products, revenue share, margin by category |
| Stage 9 | Regional & store performance — revenue ranking by region and store |
| Stage 10 | Customer analysis — purchase frequency, CLV distribution, payment methods |
| Stage 11 | Profitability analysis — margin heatmap, discount impact analysis |
| Stage 12 | Export for Power BI — 4 clean CSV tables ready for dashboard import |
| Stage 13 | Power BI dashboard guide — step-by-step build instructions |
| Stage 14 | Business insights — 7 actionable recommendations for leadership |
| Stage 15 | Conclusion — technical summary and skills demonstrated |

---

## 🗄️ SQL Queries Included

| # | Query | Technique |
|---|---|---|
| 1 | Annual revenue and profit summary | GROUP BY · aggregation |
| 2 | Revenue and margin by category | GROUP BY · subquery for % share |
| 3 | Top 10 products by revenue | ORDER BY · LIMIT |
| 4 | Regional and store performance | Multi-level GROUP BY |
| 5 | Monthly revenue trend | GROUP BY Year + Month |
| 6 | Payment method analysis | GROUP BY · percentage share |
| 7 | Year-over-year revenue growth | CTE · self-join · percentage change |
| 8 | Top customers by lifetime value | GROUP BY · MIN · MAX · ORDER BY |

---

## 🛠️ Technologies Used

| Tool | Purpose |
|---|---|
| Python 3.10+ | Core language — data generation, cleaning, EDA |
| SQLite (via Python) | SQL querying — business aggregations and KPIs |
| Pandas / NumPy | Data manipulation and feature engineering |
| Matplotlib / Seaborn | Static visualisations — 14 publication-quality charts |
| Plotly | Interactive visualisations |
| Power BI Desktop | Executive dashboard — KPI cards, slicers, trend charts |
| Google Colab | Cloud execution platform |

---

## 💡 Key Findings

- **November and December** drive the highest monthly revenue every year — Christmas and Black Friday effect confirmed across all 5 years
- **Clothing** generates the highest order volume; **Electronics** generates the highest revenue per single transaction
- **Lusaka region** (Central and East stores combined) accounts for approximately 38% of total revenue — the dominant market
- **Beauty and Books** carry the highest profit margins despite lower absolute revenue — high-margin, low-ticket products
- **Card and Mobile Money** together account for 63% of all transactions — cash usage is declining year on year
- **20% discount orders** show the worst profit margins across all discount tiers — the discount strategy needs a cap at 15%
- **Top 10% of customers** generate a disproportionately large share of total revenue — the Pareto Principle confirmed in this dataset
- **Year-over-year revenue growth** is positive across all years — the business is scaling consistently

---

## 📸 Visualisations

The notebook generates **14 publication-quality charts**:

| # | Chart | Description |
|---|---|---|
| 1 | KPI Cards | 6 executive KPIs rendered as colour-coded summary cards |
| 2 | Monthly Revenue Trend | 5-year area + line chart for revenue |
| 3 | Monthly Profit Trend | 5-year area + line chart for profit |
| 4 | Annual Revenue Bar + YoY | Bar chart with dual-axis YoY growth line |
| 5 | Seasonality by Month | Average monthly revenue — seasonal pattern |
| 6 | Revenue by Day of Week | Average revenue per day |
| 7 | Category Revenue Bar | Horizontal bar — revenue by category |
| 8 | Category Margin Bar | Average profit margin by category |
| 9 | Category Revenue Pie | Revenue share % by category |
| 10 | Top 15 Products Revenue | Horizontal bar — top products |
| 11 | Top 15 Products Profit | Horizontal bar — most profitable products |
| 12 | Regional & Store Revenue | Bar charts for region and store performance |
| 13 | Profit Margin Heatmap | Category × Month heatmap — margin patterns |
| 14 | Discount Impact Analysis | Order volume, revenue, and margin by discount tier |

---

## 📊 Power BI Dashboard

The notebook exports **4 clean CSV tables** directly importable into Power BI Desktop:

| File | Contents |
|---|---|
| `retail_sales_clean.csv` | Full 50,000-row transaction table |
| `monthly_summary.csv` | Revenue, profit, orders aggregated by month |
| `category_summary.csv` | Revenue and margin aggregated by category |
| `store_summary.csv` | Revenue and margin aggregated by store and region |

### Dashboard Features
- 4 KPI cards — Revenue, Profit, Orders, Avg Margin
- Revenue trend line chart with Year slicer
- Category revenue bar chart
- Store performance bar chart
- Payment method donut chart
- Interactive slicers — Year · Category · Region

---

## 💼 Business Insights & Recommendations

| Priority | Recommendation |
|---|---|
| 🔴 **Critical** | Double Q4 stock levels — November/December spike is predictable and consistent |
| 🔴 **Critical** | Launch a VIP programme for top 10% customers — they generate outsized revenue |
| 🟡 **Important** | Cap maximum discount at 15% — 20% discount tier is destroying margin |
| 🟡 **Important** | Expand Mobile Money payment options — fastest-growing payment method |
| 🟡 **Important** | Investigate Solwezi and Chipata branches — lowest revenue; root cause unknown |
| 🟢 **Strategic** | Expand Lusaka footprint before other regions — demand clearly supports it |
| 🟢 **Strategic** | Push Beauty and Books promotions — highest margin categories, undermarketed |

---

## 🚀 How to Run

### Option 1 — Google Colab (Recommended)

Click the **Open in Colab** badge at the top of this page. All dependencies install automatically in Cell 3. No local setup required. Total runtime: approximately **3–5 minutes**.

> ⚠️ **Important:** Always click **Runtime → Run all** when opening the notebook.
> Colab loses all variables when a session times out. Run all ensures every cell
> executes in order before you interact with the outputs.

### Option 2 — Run Locally

```bash
git clone https://github.com/GIVEN-CHINYAMA/retail-sales-analytics-dashboard.git
cd retail-sales-analytics-dashboard
pip install pandas numpy matplotlib seaborn plotly openpyxl jupyter
jupyter notebook retail_sales_analytics_dashboard.ipynb
```

---

## 📌 Repository Structure
