# Customer Shopping Behavior Analysis 🛒📊

An end-to-end data analytics project that explores customer purchasing patterns, optimizes segmentation, and visualizes key business metrics using Python, SQL Server, and Power BI.

## 🌟 Project Overview
This project analyzes a dataset of 3,900 customer transactions to uncover insights into shopping habits. It follows a full data lifecycle:
1.  **Exploratory Data Analysis (EDA):** Cleaning and feature engineering using Python.
2.  **Database Management:** Automating data migration to SQL Server.
3.  **Business Intelligence:** Performing complex SQL queries to solve specific business questions.
4.  **Data Visualization:** Creating an interactive dashboard for executive decision-making.

## 📊 Dashboard Output
Since GitHub does not support live iframes, you can access the interactive Power BI report via the link below.

> [!TIP]
> **[👉 Click Here to View the Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNWRhYzQzMzgtNmQzNS00NThhLTkzNDgtMzNmZDNhZjUxNmFmIiwidCI6IjEwZDg5ZTg1LWM2MTEtNDk5MS04YmNiLTJiYzM0MjFlMDYwZCJ9)**

*(Recommended: Add a screenshot of your dashboard here as `dashboard_preview.png` for a better visual appeal)*

## 🛠️ Tech Stack
* **Language:** Python (Pandas, NumPy, SQLAlchemy)
* **Database:** Microsoft SQL Server (T-SQL)
* **Visualization:** Power BI & Plotly
* **Environment:** Jupyter Notebook & SSMS

## 📂 Project Structure & Logic
### 1. Data Cleaning & Feature Engineering (`EDA.ipynb`)
* **Handling Missing Data:** Found 37 missing values in `review_rating`.
* **Imputation:** Filled missing ratings by grouping by `category` and applying the mean of that specific category.
* **Feature Engineering:** * Created `age_group` (Young Adult, Adult, Middle-aged, Senior) using quartiles.
    * Mapped `frequency_of_purchases` to numerical `frequency_purchases_days` (e.g., Weekly = 7, Annually = 365).
* **Data Migration:** Automated the transfer of cleaned data to a SQL Server database named `customer_behavior` via `sqlalchemy`.

### 2. Business Analysis (`Business Analysis.sql`)
The following business questions were answered using T-SQL:
* **Revenue Analysis:** Calculated total revenue by gender.
* **Customer Segmentation:** Used `CASE` statements to segment users into **New**, **Returning**, and **Loyal** based on `previous_purchases`.
* **Product Performance:** Identified the top 3 most purchased products within each category using `ROW_NUMBER()`.
* **Discount Impact:** Identified the top 5 products with the highest percentage of purchases using discounts.

## ⚙️ Setup Instructions
1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  **Database Connection:**
    * Open `EDA.ipynb`.
    * Update the `SERVER_NAME` variable to match your local SQL Server instance (currently set to `ksaidatta\SQLEXPRESS`).
3.  **Run the Pipeline:**
    * Execute the Jupyter Notebook to clean data and populate your SQL table.
    * Run `Business Analysis.sql` in SSMS to generate business reports.

## 📜 License
This project is open-source and available under the MIT License.

---
**Author:** [k sai datta]