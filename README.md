# 🧠 Banking Domain Data Analytics Project

### *A Complete Business Analytics Walkthrough — Using SQL Server as a Host & Python for Smart Analysis*

---

## 📌 Overview

This end-to-end project explores real-world **banking operations and customer behavior** by combining structured data warehousing with deep exploratory analytics. It focuses on understanding clients, deposits, loans, and branches — to derive actionable insights for decision-making.

The core work was done using **Python and Power BI**, with SQL Server (SSMS) used for database hosting and structured storage.

---

## 🎯 Problem Statement

> **How can banks better understand customer demographics, product adoption, and branch-level performance through descriptive data analysis and dashboards — without predictive modeling?**

---

## 🔄 Project Workflow

### 1️⃣ Data Source & Transformation

* Initial format: **Excel**
* Cleaned and converted into **CSV** for easier manipulation and import
* Loaded into **SQL Server (SSMS)** as a structured database

### 2️⃣ SQL Server as Data Host (Not Query Engine)

* Used **SSMS to create tables** and import CSVs
* No complex SQL queries were written here — only used for **centralized storage**
* All data manipulation and logic were done after extracting into Python

> ✅ **Why this approach?**
> Because it separates **storage from logic** — allowing reproducible, scriptable analytics workflows in Python.

### 3️⃣ Data Extraction & Analysis in Python

* Connected SQL Server to Python using `pyodbc`
* Loaded tables into **Pandas DataFrames**
* Performed all **data cleaning, joining, filtering, and EDA** within Jupyter Notebook
* Tools used: `pandas`, `matplotlib`, `seaborn`

### 4️⃣ Exploratory Data Analysis (EDA)

Analyzed key banking features such as:

* **BRID (Branch ID)** performance
* **Loan distribution** by type, region, and occupation
* **Deposits** segmented by year, client profile, and nationality
* **Account insights**, customer-product combinations, and temporal trends

---

## 📊 Dashboard (Power BI)

Built an interactive **Power BI report** to communicate findings with clarity:

| Page              | Highlights                                                                  |
| ----------------- | --------------------------------------------------------------------------- |
| Deposit Analysis  | Year-wise and BRID-wise trends, filters by occupation and region            |
| Loan Analysis     | Types of loans by income band, client profile, and branch                   |
| Account Overview  | Accounts per client, nationality breakdown, BRID-level aggregation          |
| Executive Summary | Snapshot view for leadership using KPIs and heatmaps                        |
| Segmentation Tool | Interactive filters: Occupation, Fee, Nationality, Loan Status, Year Joined |


---

## 💡 Business Insights

* **Branch IDs (BRIDs)** showed high performance variation — potential benchmark branches
* **Certain occupations** held higher loan volumes — useful for credit targeting
* **Clients with multiple products** (e.g., deposits + loans) showed higher retention potential
* **Nationality and region-based behaviors** influenced deposit size and frequency
* Year-over-year data showed **digital onboarding impact on account volume**

---

## ⚙️ Tools Used

| Tool     | Purpose                                          |
| -------- | ------------------------------------------------ |
| Excel    | Raw data source                                  |
| CSV      | Intermediary format                              |
| SSMS     | Centralized relational data storage (no queries) |
| Python   | All querying, transformation, EDA                |
| Power BI | Dashboards & storytelling for stakeholders       |

---

## 📂 File Structure

```
📁 Banking_Analytics_Project
│
├── data/
│   ├── banking.csv
│   ├── banking.xlsx
│
├── notebooks/
│   └── EDA_and_SQL_Connection.ipynb
│
├── dashboards/
│   └── PowerBI_Report.pbix
│
└── README.md
```

---

## 🧠 Learnings & Takeaways

* Built a **data pipeline from Excel → SQL → Python → Dashboard**
* Learned how to separate **storage (SSMS)** from **logic and analysis (Python)**
* Strengthened **exploratory analysis and business storytelling**
* Applied real-world concepts like **customer segmentation** and **branch performance tracking**
* Future scope:

  * Predictive models for churn or credit scoring
  * Real-time dashboard deployment

---

> *“Good data tells a story — but only great analysis gives it a voice.”*

---

