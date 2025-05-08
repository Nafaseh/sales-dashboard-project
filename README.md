#  Retail Sales Analysis – Superstore Dataset

This is a complete end-to-end data analytics project using the **Sample Superstore dataset**.  
The objective is to extract actionable insights from retail sales data using **Excel**, **SQL**, and **Power BI**.

---

## 📊 Tools & Technologies

- Microsoft **Excel** – Data cleaning, transformation, and pivot analysis  
- **SQL** – Structured queries for revenue and profit insights  
- **Power BI** – Interactive dashboards for executive reporting

---

## 🎯 Objectives

- Identify top-performing regions and products
- Analyze sales and profit trends over time
- Understand customer segments and behavior
- Provide dynamic visual reporting through dashboards

---

## 🔧 Project Workflow

### 1. **Data Cleaning (Excel)**
- Removed duplicates and blank rows
- Added calculated columns:
  - `Profit Ratio = Profit / Sales`
  - `Order Month` and `Order Year`
- Built pivot tables to explore sales by category and region

### 2. **SQL Analysis**
- Imported dataset into SQL (SQLite)
- Sample Queries:
```sql
SELECT Region, SUM(Sales) AS TotalSales
FROM Orders
GROUP BY Region
ORDER BY TotalSales DESC;

SELECT Category, SUM(Profit) AS TotalProfit
FROM Orders
GROUP BY Category;
