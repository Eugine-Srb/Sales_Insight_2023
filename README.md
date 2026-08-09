# Sales\_Insight\_2023

## 📊 2023 Revenue Analysis Dashboard (Power BI + Python)

### 🔍 Project Overview

**Goal:**
To analyze company revenue performance throughout the entire year of 2023 using daily transactional data. This project focuses on identifying trends, anomalies, and influencing factors using DAX-based metrics and Power BI visuals — all grounded in fact-based analysis (no forecasting or projections).

### 📁 Dataset

* **Source Table:** `Sales_Report`
* **Period:** January 1, 2023 – December 31, 2023 (daily granularity)
* **Columns:**

  * `Date`: Daily transaction date (Date type)
  * `Revenue`: Total daily revenue value
* **Supplementary Table:** Custom `Date Table` created for advanced time intelligence
* No missing values (NaN) in the dataset
* An additional helper table was created using Python to support analytical views

### 📌 Key Report Pages (Power BI)

**1️⃣ KPI Dashboard**

* Total revenue, monthly revenue, and MoM change
* Visual cards + bar chart
* Highlights performance spikes and slowdowns

**2️⃣ Anomaly Detection**

* Revenue vs rolling average and standard deviation
* Conditional formatting flags outliers
* CI bands for visual deviation alerts

**3️⃣ Key Influencers**

* Power BI’s AI visual used to detect primary drivers
* Interaction with months, weeks, and time-based factors

**4️⃣ Time Intelligence**

* Rolling 3-month and 6-month averages
* YTD and MTD calculations
* Seasonal monthly pattern tracking

**5️⃣ Smart Narrative**

* Auto-generated narrative with plain-text insights
* Executive-level storytelling for business review

### ⚙️ Modeling Approach

* All calculations and logic done with **DAX** in Power BI
* **No machine learning or predictive analytics** used in this version
* **Python** was used only to generate a supporting analytical table for CI-based visualizations

### ⚠️ Limitations

* Dataset includes only **1 year (2023)** → no multi-year comparison
* Forecasting or predictive models **intentionally excluded**
* No segmentation by product, customer, or region

### 📈 Future Enhancements

* Add historical years (e.g., 2022) for trend comparison
* Apply anomaly detection by product, category, or region
* Integrate AI forecasting models (Prophet, SARIMA) in future experiments

### 👥 Intended Audience

Executives, analysts, and decision-makers who want a transparent, an in-depth overview of revenue activity over a single year — with strong visual storytelling and zero guesswork.

### 🧩 Tools Used

* **Power BI**: Data model, DAX metrics, visual dashboards
* **Python**: Custom table generation
* `pandas`, `datetime` (light data prep)

### 📁 Project Structure

```bash
/
├── data/
│   ├── Enhanced_Mock_Sales_Dashboard_Data.xlsx      # Raw dataset
│   ├── Sales_Report_Slim.xlsx                       # Transformed Excel dataset
│   └── CI_Analysis.csv                              # Python-generated output
│
├── notebooks/
│   └── CI_Analysis.ipynb                            # Python code for CI analysis
│
├── powerbi/
│   └── Mock_Revenue_Analysis.pbix                   # Power BI dashboard file
│
├── README.md
```

### 🔁 Reproducibility Notes
* Note: The file CI_Analysis.csv is already included in the data/ folder for direct use in Power BI.
* You can re-generate it by running the Python notebook located at notebooks/CI_Analysis.ipynb.

### 💻 Run in Google Colab
* Use this link to open and run the Python notebook in a cloud environment:

* 🔗 [Open in Colab](https://colab.research.google.com/drive/18TdahMbAtTh89zM0FduGzOra22I9xBUH?authuser=1#scrollTo=f071f99b-1d79-48f1-ac6a-3f46304562c2)

### 📊 Power BI Dashboard

* 🔗 [Power BI Report](https://app.powerbi.com/view?r=eyJrIjoiMDA2NjhhZGItNzkxMy00ODljLTg4OTctYzNjZDdiOGM4MWNjIiwidCI6IjQxOTI3ZjQyLTQ2NWMtNDFmOS1iYzAwLTUxMTVjM2QzNTE3NCIsImMiOjl9&pageName=c47665786b1b50502d0a)
