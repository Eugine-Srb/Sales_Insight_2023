# Sales_Insight_2023
Power BI dashboard for 2023 daily sales
# 📊 2023 Revenue Analysis Dashboard (Power BI + Python)

## 🔍 Project Overview

**Goal:**  
To analyze company revenue performance throughout the entire year of 2023 using daily transactional data. This project focuses on identifying trends, anomalies, and influencing factors using DAX-based metrics and Power BI visuals — all grounded in fact-based analysis (no forecasting or projections).

---

## 📁 Dataset

- **Source Table:** `Sales_Report`
- **Period:** January 1, 2023 – December 31, 2023 (daily granularity)
- **Columns:**
  - `Date`: Daily transaction date (Date type)
  - `Revenue`: Total daily revenue value
- **Supplementary Table:** Custom `Date Table` created for advanced time intelligence

- **No missing values (NaN)** in the dataset  
- An additional helper table was created using **Python** to support analytical views

---

## 📌 Key Report Pages (Power BI)

### 1️⃣ KPI Dashboard
- Total revenue, monthly revenue, and MoM change
- Visual cards + bar chart
- Highlights performance spikes and slowdowns

### 2️⃣ Anomaly Detection
- Revenue vs rolling average and standard deviation
- Conditional formatting flags outliers
- CI bands for visual deviation alerts

### 3️⃣ Key Influencers
- Power BI’s AI visual used to detect primary drivers
- Interaction with months, weeks, and time-based factors

### 4️⃣ Time Intelligence
- Rolling 3-month and 6-month averages
- YTD and MTD calculations
- Seasonal monthly pattern tracking

### 5️⃣ Smart Narrative
- Auto-generated narrative with plain-text insights
- Executive-level storytelling for business review

---

## ⚙️ Modeling Approach

- All calculations and logic done with **DAX** in Power BI
- **No machine learning** or predictive analytics used in this version
- Python was used **only** for generating a custom supporting table

---

## ⚠️ Limitations

- Dataset includes **only 1 year** (2023) → no multi-year comparison
- Forecasting or predictive models intentionally excluded
- No segmentation by product, customer, or region

---

## 📈 Future Enhancements

- Add historical years (e.g., 2022) for trend comparison
- Apply anomaly detection by product, category, or region
- Integrate AI forecasting models (Prophet, SARIMA) in future experiments

---

## 👥 Intended Audience

Executives, analysts, and decision-makers who want a transparent, in-depth overview of real revenue activity over a single year — with strong visual storytelling and zero guesswork.

---

## 🧩 Tools Used

- **Power BI** (Data model, DAX metrics, visual dashboards)
- **Python** (Custom table generation)
- **Pandas, datetime** (light data prep)
