# Customer Shopping Behavior Analysis 🛒📊

An end-to-end data engineering and analytics project exploring customer purchasing patterns, optimized segmentation, and business metrics using Python, SQL Server, and Power BI.

## 📊 Dashboard Preview
Click the image below to open the **Live Interactive Dashboard**.

[![Customer Behavior Dashboard]([https://raw.githubusercontent.com/your-username/your-repo-name/main/dashboard_preview.png](https://github.com/datta116/Customer-Behaviour/blob/b9e4ef0b2bc68d3eecd034ae6bdb892511ecca29/Docs/1209.gif))](https://app.powerbi.com/view?r=eyJrIjoiNWRhYzQzMzgtNmQzNS00NThhLTkzNDgtMzNmZDNhZjUxNmFmIiwidCI6IjEwZDg5ZTg1LWM2MTEtNDk5MS04YmNiLTJiYzM0MjFlMDYwZCJ9)

> **[🚀 Click Here to Open Live Report](https://app.powerbi.com/view?r=eyJrIjoiNWRhYzQzMzgtNmQzNS00NThhLTkzNDgtMzNmZDNhZjUxNmFmIiwidCI6IjEwZDg5ZTg1LWM2MTEtNDk5MS04YmNiLTJiYzM0MjFlMDYwZCJ9)**

---

## 🌟 Project Overview
This project follows a full data lifecycle analyzing 3,900 customer records:
1.  **Exploratory Data Analysis (EDA):** Performed cleaning and feature engineering in Python.
2.  **Database Management:** Automated data migration to a local SQL Server.
3.  **Business Intelligence:** Conducted deep-dive analysis using T-SQL to answer business KPIs.
4.  **Data Visualization:** Built an interactive Power BI dashboard.

## 🛠️ Tech Stack
* **Language:** Python (Pandas, NumPy, SQLAlchemy)
* **Database:** Microsoft SQL Server (T-SQL)
* **Visualization:** Power BI & Plotly
* **Environment:** Jupyter Notebook & SSMS

## 📂 Project Structure & Key Logic

### 1. Data Cleaning & Engineering (`EDA.ipynb`)
* **Missing Value Imputation:** Handled 37 null values in `review_rating` by calculating the mean rating per product category.
* **Feature Engineering:**
    * **Age Groups:** Classified customers into *Young Adult*, *Adult*, *Middle-aged*, and *Senior*.
    * **Frequency Mapping:** Converted purchase frequency text (e.g., "Weekly") into numerical days (7).
* **SQL Integration:** Established a connection using `sqlalchemy` to push the cleaned dataset into SQL Server automatically.

### 2. Business Analysis (`Business Analysis.sql`)
Key business insights extracted using SQL include:
* **Revenue Analysis:** Total revenue comparison between Male and Female customers.
* **Customer Loyalty:** Segmented users into **New**, **Returning**, and **Loyal** based on their previous purchase counts.
* **Top Products:** Ranked the top 3 items per category using `ROW_NUMBER()` window functions.
* **Discount Strategy:** Identified products with the highest percentage of discount-based purchases.

## ⚙️ Setup & Installation
1.  **Clone the Repo:** `git clone https://github.com/your-username/your-repo-name.git`
2.  **Run Cleaning:** Open `EDA.ipynb` and ensure your `SERVER_NAME` matches your local SQL instance.
3.  **Execute SQL:** Run `Business Analysis.sql` in SSMS to view generated reports.

---
**Author:** [Your Name]
