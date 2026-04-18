# Superstore's-Finance-summary
# 📊 Superstore Financial Performance Dashboard (Power BI)

## 📌 Project Overview

This project showcases a comprehensive **Financial Performance Dashboard** built using Power BI. The workflow includes data validation, transformation, modeling, and visualization to derive meaningful business insights.

---

## 🔄 Project Workflow

### 🔹 1. Data Import & Validation (SQL Server)

* Imported raw dataset into **SQL Server**
* Performed data validation checks to ensure:

  * Accuracy
  * Consistency
  * Data completeness
Example

-- Check duplicate records 
     SELECT 
        row_id,
       Order_id,
       Product_ID,
       Customer_ID,
       COUNT(*) As Duplicate
     
      FROM DBO.[Sample - Superstore]
      GROUP BY row_id,
               Order_id,
               Product_ID,
               Customer_ID
     HAVING    COUNT(*) >1
---

### 🔹 2. Data Integration in Power BI

* Connected Power BI with SQL Server
* Imported validated dataset into Power BI for further analysis

---

### 🔹 3. Data Modeling

* Created a **separate Date Table** for time intelligence
* Established relationships between tables
* Marked Date Table as a **Date Table** for accurate calculations

---

### 🔹 4. DAX Calculations

Developed key measures using DAX:

* Total Revenue
* Total Profit
* Total Orders
* Profit Margin (%)
* Year-over-Year Growth (using SAMEPERIODLASTYEAR)

---

### 🔹 5. Data Visualization

Designed an interactive dashboard using:

* KPI Cards (Revenue, Profit, Orders, Margin)
* Revenue Trend by Month (Line Chart)
* Impact of Discount on Profit Margin
* Profit Margin by Category & Segment
* Revenue by Region (Treemap)

---

### 🔹 6. Advanced Features

#### 📌 Tooltips

* **Category Tooltip** → Displays Sub-Category breakdown
* **Region Tooltip** → Shows Top 5 States by Revenue

#### 📌 Interactivity

* Year slicer for dynamic filtering
* All visuals respond to user selection

---

## 📊 Key Insights

* Revenue and order volume show strong growth trends
* Profit margin decreases with increasing discount levels
* Technology category is most profitable
* Furniture category shows low profitability
* West region contributes highest revenue

---

## 🛠 Tools & Technologies

* SQL Server (Data Validation)
* Power BI
* DAX (Data Analysis Expressions)
* Data Modeling

---

## 🧠 Skills Demonstrated

* Data Validation & Cleaning
* Data Modeling & Relationships
* DAX (Time Intelligence & KPIs)
* Dashboard Design & Visualization
* Business Insight Generation

---

## 📷 Dashboard Preview

(dashboard.png)<img width="1452" height="801" alt="Screenshot 2026-04-18 224823" src="https://github.com/user-attachments/assets/caa9e735-ce6e-4012-8780-85c75d7896be" />


---

## 🚀 Conclusion

This project demonstrates end-to-end data analysis, from raw data validation to delivering actionable insights through an interactive dashboard.

---

## 👩‍💻 Author

**Deepika | Aspiring Data Analyst**
Skilled in Power BI, SQL, and data visualization.

