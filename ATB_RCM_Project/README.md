# 🚀 **Project Overview**

This project demonstrates:

- Professional **ETL pipeline implementation**  
- Deep understanding of **RCM domain**  
- Feature engineering on patient AR aging  
- Creation of financial **KPI dashboards**  
- Clean Python architecture + folder structure  
- Visualization & reporting skills  

If you work in Revenue Cycle Management, AR tracking, or Healthcare Analytics — this project represents a realistic workflow.

---

# 🔧 **Tech Stack**

| Technology | Purpose |
|-----------|----------|
| **Python** | Core ETL + analysis |
| **Pandas** | Data cleaning, transformation |
| **NumPy** | Numeric operations |
| **Matplotlib** | Charts and visualizations |
| **Jupyter Notebook** | Data exploration |
| **GitHub** | Version control, documentation |

---

# 🛠 **ETL Pipeline Workflow**

### **1️⃣ Extract**
- Load the raw Aged Trial Balance Excel file from `ATB_ROWDATA/`
- Normalize column names
- Identify important fields:  
  `service_date`, `billing_date`, `fees`, `payments`, `adjustments`, `balance`, `insurance`, etc.

---

### **2️⃣ Transform**

Performed data cleaning & transformation:

#### ✔ Standardize headers  
- Remove spaces  
- Lowercase  
- Convert inconsistent text fields  

#### ✔ Convert raw date columns  
- `service_date`, `billing_date`, `last_edited`, `follow_up_date`
- Converted to datetime
- Re-formatted to `MM-DD-YYYY`

#### ✔ Numeric Cleaning  
Converted financial columns to numeric:
- `fees`
- `payments`
- `adjustments`
- `refunds`
- `balance`

#### ✔ Feature Engineering
Created:
- `days_since_billing` → (today - billing_date)
- `aging_bucket` → 0–30, 31–60, 61–90, 91–120, 120+

#### ✔ Remove null/invalid rows  
Ensured consistency and quality in the final dataset.

---

### **3️⃣ Load**

Final cleaned dataset exported as: OUTCOME/ATB_cleaned_with_aging.csv


Charts automatically generated into:

Charts-- 

# 📊 **KPIs Generated**

| KPI | Description |
|-----|-------------|
| **Total AR** | Sum of all outstanding balances |
| **Total Fees** | Total provider charges |
| **Total Payments** | Total payments received |
| **Total Adjustments** | Sum of all adjustments |
| **Refunds Analysis** | Total refunded amount |
| **Net Collection Ratio (NCR)** | Payments / Adjusted charges |
| **Average Days in AR** | Mean of days_since_billing |
| **AR in 120+ bucket** | High-risk aging accounts |
| **Unique Patients** | Count of distinct patients |
| **Unique Claims** | Claim volume measurement |

---

# 📈 **Visualizations (10 Dashboards)**

The following charts are included inside the `CHARTS/` folder:

1. **AR Balance by Aging Bucket (Bar Chart)**  
2. **Top 10 Insurance Payers by AR**  
3. **AR by Department**  
4. **AR by Rendering Provider**  
5. **Monthly Fees Trend**  
6. **Monthly AR Trend**  
7. **Top 10 Accounts by Balance**  
8. **Days in AR Distribution (Histogram)**  
9. **Fees vs Payments vs Adjustments vs Refunds**  
10. **AR Share by Aging Bucket (Pie Chart)**

Example:

```md
![Aging Bucket](/ATB_RCM_Project/CHARTS/01_ar_by_aging_bucket.png)



