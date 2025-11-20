# 📊 Budget & Work Performance Dashboard  
*A full analytics system built with Google Sheets, Google Apps Script, and automated KPI logic.*

This project transforms raw weekly paystub data into a complete **financial + work-performance dashboard**, including forecasting, KPI scoring, visual analytics, and structured data pipelines ready for SQL, Tableau, Power BI, or Python.

---

# 📌 Project Overview

This dashboard combines **personal income tracking**, **monthly budgeting**, and **Stanley Steemer work performance metrics** into one unified analytics system.

It includes:

- Automated **weekly ingestion** of paystub data  
- **KPI engine** for performance scoring  
- **Monthly income vs expense** reporting  
- **Rolling averages** and **4-Pay Forecasting**  
- **Trend charts** for income, hours, add-ons, commissions  
- A fully structured data layer designed for **SQL warehousing & BI tools**

📄 **Dashboard PDF Preview:**  
[Monthly Budget.PDF](./assets/Monthly%20Budget.PDF)

---

# 🧩 Features

### **📅 Personal Finance Metrics**
- Avg Monthly Income  
- 3-Month Rolling Avg  
- Total Gross & Take-Home  
- Budget vs Actual Spending  
- Monthly Net Income  
- Category Breakdown (Rent, Groceries, Gas, etc.)

### **🧰 Work Performance Metrics**
- Hours Worked  
- Stops per Week  
- Add-On Amounts  
- Commission Earned  
- Time per Stop (hrs/min)  
- Effective Hourly Rate  
- Weekly Scorecard with Color-Coded Performance  

### **📈 Forecasting & Trends**
- 4-Pay Forecast (Gross + Net)  
- 3-Month Rolling Forecast  
- Effective Hourly Rate Trend  
- Add-On Trend  
- Commission Trend  
- Avg Time per Stop Trend  

### **⚙ Automation Layer**
- Google Apps Script OCR parsing  
- Data cleaning + URL logs  
- Weekly processing confirmation  
- Bonuses/flags  
- Structured date logic (week_id, month_id, quarter_id, year)

---

# 🧠 Data Pipeline

### **1️⃣ Input Layer (Raw Pay Data)**
From weekly paystubs:
- Date  
- Gross Pay  
- Take-Home Pay  
- Hours  
- Add-On Amount  
- Stop Count  
- Commission  
- Time per Stop  
- Apps Script log URLs  

### **2️⃣ Processing Layer**
Calculates:
- Add-On per Stop  
- Effective Hourly Rate  
- Time per Stop (hr/min)  
- Weekly Performance KPIs  
- Forecast Metrics  
- Rolling Averages  

### **3️⃣ Analytics Layer**
Powers dashboards:
- Monthly views  
- Weekly scorecards  
- Trend charts  
- Summary KPIs  
- Variance vs Goals  

### **4️⃣ Output Layer**
- Dashboard PDF  
- Sample CSV data  
- Clean structured tables for SQL/BI tools  

---

# 🗂 File Structure

```txt
Budget-Performance-Dashboard/
│
├── README.md
├── assets/
│   ├── Monthly Budget.PDF
│   ├── cover.png              # (You will add this later)
│   ├── banner.png             # (You will add this later)
│   └── charts/
│       ├── gross_vs_net.png
│       ├── weekly_scorecard.png
│       ├── income_trend.png
│       └── ehr_trend.png
│
├── data/
│   ├── sample_pay_data.csv
│   ├── sample_budget.csv
│   └── sample_kpi_output.csv
│
└── scripts/
    └── paystub_parser.gs      # Google Apps Script for OCR parsing
