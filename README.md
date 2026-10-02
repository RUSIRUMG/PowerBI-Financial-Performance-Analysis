```
# 📊 Executive Financial Performance Analytics | Power BI Project

An executive-ready Financial Overview Dashboard built using Microsoft Power BI to evaluate Revenue, Cost of Goods Sold (COGS), Net Profitability, and Margin trends (2013–2014) for business decision-makers (CFO/CEO view).

---

## 📸 Dashboard Overview
![Financial Dashboard](Financials%20Dashboard%206.png)

---

## 🎯 Project Objective
The primary goal of this project was to transform raw financial transactional data into actionable strategic insights. By establishing a robust data model and dynamic DAX measures, the dashboard enables leadership to monitor core P&amp;L performance, track monthly profit trends, and evaluate profitability across product segments and geographic locations.

---

## 💡 Key Strategic Insights &amp; Recommendations

1. **Enterprise Segment Turnaround (Cost &amp; Discount Control):** 
   - *Finding:* Generated over \$4M+ in gross revenue but incurred an overall net loss with a **-4.78% Profit Margin**.
   - *Action:* Re-evaluate high-discount strategies and cost structures in Enterprise contracts to mitigate margin leakage.

2. **Capitalizing on Channel Partners (High-Margin Expansion):** 
   - *Finding:* Delivered an exceptional **72.82% Profit Margin** despite relatively low sales volume (\$398K).
   - *Action:* Scale marketing and distribution efforts in this segment to maximize net profitability with minimal incremental overhead.

3. **Safeguarding Core Cash Flows (Government Segment):** 
   - *Finding:* Represents the company's core pillar, driving nearly 50% of total sales (~\$13M) with a sustainable **22.06% Profit Margin**.
   - *Action:* Maintain strong delivery standards to preserve baseline stability.

4. **Discount Policy Optimization:** 
   - *Finding:* Cross-filtering indicates that higher discount bands severely compress overall margins across flagship products (Paseo, Velo).

---

## 🛠️ Technical Implementation &amp; Architecture

### 1. Data Modeling (Star Schema)
- Created a dedicated **`Dim_Date`** table using DAX (`CALENDARAUTO()`).
- Established clean **1-to-Many single-direction relationships** between `Dim_Date` and the fact table.
- Resolved alphabetical month-sorting issues using `Sort by Column` (`Month Number` &amp; `YearMonthKey`).

### 2. Core DAX Measures Used
- **Total Sales:** `SUM(financials[Sales])`
- **Total Cost:** `SUM(financials[COGS])`
- **Total Profit:** `SUM(financials[Profit])`
- **Profit Margin %:** `DIVIDE([Total Profit], [Total Sales], 0)`

### 3. Executive UX/UI Features
- **Left Navigation Sidebar Architecture:** Clean, modern enterprise layout for controls.
- **Drill-down Hierarchy Matrix:** Segment-to-Country breakdown with Conditional Formatting (Data Bars for volume, Heatmaps for margins).
- **Interactive Visuals:** Monthly line trend, Product comparison bar charts, and Country Profit Share Donut Chart.
- **Reset View Bookmark:** One-click reset functionality clearing both slicers and visual cross-filtering states.

---

## 📁 Repository Structure

'''

├── Financial\_Performance\_Dashboard.pbix # Main Power BI Desktop Report File
├── Financials Dashboard 6.png # Executive Dashboard View Screenshot 
└── README.md # Detailed Project Documentation

'''

---

## 👤 Author
Developed by an aspiring Data Analyst focusing on Business Intelligence, Financial Modeling, and Data Storytelling.
```
