# 📦 SAP Order-to-Cash Analytics — Unilever Pakistan

**Analyzing Q1 2026 sales operations data to diagnose fulfillment gaps, rejection patterns, and order-to-billing performance across regions, divisions, and brands.**

---

## 🔗 [View Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiOWRiMTk2MTAtZTk2Mi00N2FmLWExNmYtNDBkNWMxOWMzNmJiIiwidCI6IjNiNWIwMDgyLTczNmQtNGIwNi1hYjU1LWUyYzQ0ZGI3YWIzMSIsImMiOjl9)

---

## 🛠 Tech Stack

- 📊 Power BI Desktop
- 🧠 DAX (KPI measures)
- 📂 Power Query (ETL & data cleaning)
- 📝 Data Modeling (Star Schema)
- 📊 Excel (data preparation & pivot analysis)

---

## 📂 Data Source

SAP Order-to-Cash (O2C) extract for a FMCG business in Pakistan covering **Q1 2026** 70,653 order lines across 29 columns spanning the full order lifecycle from creation through billing. Data covers multiple divisions, brands, cities, and ordering interfaces (DMS+, NEO, EDI, eCOP, EXCEL).

---

## 💡 Dashboard Breakdown

### Business Problem
A large FMCG operation runs thousands of orders weekly across multiple regions and product divisions. Without structured visibility, it's impossible to know: how much volume is being lost to rejections, where fulfillment is breaking down, which brands are underdelivering, and whether the order-to-billing cycle is running efficiently.

### Goal
Build an interactive O2C analytics dashboard that tracks fulfillment performance, surfaces rejection patterns by region and brand, and gives operations teams the visibility they need to act filterable by division and date range.

---

### 🖥️ Walkthrough of Key Pages

---

**Page 1 — Order to Billing Performance**

![Order to Billing Performance](https://raw.githubusercontent.com/Mariarais24/sap-o2c-analytics-powerbi/main/order-billing-performance.png)

Operational overview of Q1 2026 order flow. 68,940 total orders with 4,040 MT ordered and 3,081 MT billed, a fulfillment rate of **76.28%**, leaving 958 MT unfulfilled. A regional bar chart compares ordered vs billed volume across cities; Lahore leads with 1,316 MT ordered but only 909 MT billed. The weekly trend chart shows a peak in W11 (1,087 MT) followed by a steady decline toward W9. The order fulfillment funnel breaks down where volume is getting stuck: 46K billed, 12K rejected, 10K pending, with minimal confirmed-not-delivered and delivered-not-billed volume. Billed volume by division shows Home Care dominating at 43% (1,315 MT), with Surf, Knorr, and Lifebuoy leading by brand.

---

**Page 2 — Fulfillment & Rejection Analysis**

![Fulfillment and Rejection Analysis](https://raw.githubusercontent.com/Mariarais24/sap-o2c-analytics-powerbi/main/fulfillment-rejection.png)

Diagnoses where and why orders fail. Rejection rate sits at **17.35%** (11,958 rejected orders), with an average delivery lead time of 1.4 days and a rescheduling rate of 89.56%. Lahore accounts for 4,974 rejected orders, the highest absolute rejection volume followed by Karachi at 2,816. Lead time by region shows Faisalabad, Lahore, and Gujranwala at 2 days vs 1 day for most other cities flagging potential supply chain pressure. Fulfillment rate by brand reveals Comfort (94.4%) and Hellmann's (92.8%) at the top, while Paddle Pop/Max (71.8%) and Lux (72.3%) lag significantly behind. Weekly rejection rate peaked at 35% in W13, declining to 11% by W11.

---

### Business Impact & Insights

- ⚠️ **76.28% fulfillment rate** — nearly 1 in 4 MT ordered is not reaching billing
- 🔴 **17.35% rejection rate** — 11,958 orders rejected in a single quarter
- 📍 **Lahore drives the highest rejection volume (4,974)** — proportional to order size but still the biggest operational risk
- ⏱️ **89.56% rescheduling rate** — almost 9 in 10 orders are being rescheduled, signaling systemic order confirmation issues
- 📉 **Weekly rejection rate peaked at 35% in W13** before declining — a spike worth investigating for root cause
- 🏆 **Surf (826 MT) leads billed volume** — Home Care is the strongest performing division

---

## ✅ Recommendations

| # | Action |
|---|---|
| 1 | Investigate **Lahore and Karachi rejection drivers** — highest absolute rejection volumes in Q1 |
| 2 | Address the **89.56% rescheduling rate** — near-universal rescheduling suggests a systemic order confirmation process issue |
| 3 | Review **Lux and Paddle Pop/Max supply chain** — fulfillment rates below 72% indicate consistent availability gaps |
| 4 | Investigate the **W13 rejection spike (35%)** — understanding the cause can prevent recurrence in Q2 |
