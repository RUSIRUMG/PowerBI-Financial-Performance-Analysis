
# 📊 Financial Performance Dashboard in Power BI | P&amp;L Analysis &amp; Learning Journey

A practical Financial Performance Analytics project built using Microsoft Power BI to explore Revenue, Cost of Goods Sold (COGS), Profitability, and Margin trends (2013–2014) from an executive (CFO/CEO) perspective.

---

## 🎥 Dashboard Preview 

### 1️⃣ Executive Default View
![Financial Dashboard 1](financial%20dashboard%201.png)

### 2️⃣ Country Slicer
![Financial Dashboard 1](financial%20dashboard%202.png)

### 3️⃣ Cross filtering
![Financial Dashboard 1](financial%20dashboard%203.png)

### 🎬 Interactive Video Walkthrough
[📥 Click here to watch/download the Video Demo](financial%20dashboard%20video%20.mp4)
---

## 🎯 Project Purpose
As part of my ongoing journey to learn Data Analytics and Business Intelligence, I developed this dashboard to practice transforming raw financial transactional data into structured executive insights. The goal was to build a clean, functional report that helps analyze core P&amp;L performance across segments, countries, and product lines.

---

## 💡 Key Business Findings &amp; Observations

1. **Enterprise Segment (Discount &amp; Cost Control):** 
   - *Observation:* The Enterprise segment incurred an overall net loss with a **-4.78% Profit Margin** despite generating over \$4M in gross revenue.
   - *Takeaway:* Re-evaluating discount structures and contract cost allocations can eliminate margin leakage.

2. **Channel Partners Segment (High-Margin Area):** 
   - *Observation:* Achieved an exceptional **72.82% Profit Margin** despite a lower sales volume (\$398K).
   - *Takeaway:* Highlights a highly profitable opportunity for potential expansion with low overhead.

3. **Government Segment (Core Revenue Pillar):** 
   - *Observation:* Generates nearly 50% of total company revenue (~\$13M) with a stable **22.06% Profit Margin**.
   - *Takeaway:* Serves as the primary baseline for cash flow stability.

4. **Discount Band Impact:** 
   - *Observation:* Visual analysis showed that higher discount bands heavily compress net profit margins across flagship products (Paseo, Velo).

---

## 🛠️ Technical Implementation &amp; Learning Highlights

### 1. Data Modeling (Star Schema)
- Created a dedicated **`Dim_Date`** table using DAX (`CALENDARAUTO()`).
- Established clean **1-to-Many single-direction relationships** between `Dim_Date` and the fact table.
- Resolved alphabetical month sorting issues by applying **`Sort by Column`** (`Month Number` &amp; `YearMonthKey`).

### 2. DAX Measures Used
- **Total Sales:** `SUM(financials[Sales])`
- **Total Cost:** `SUM(financials[COGS])`
- **Total Profit:** `SUM(financials[Profit])`
- **Profit Margin %:** `DIVIDE([Total Profit], [Total Sales], 0)` *(Handling zero-division gracefully)*

### 3. Report UX/UI Setup
- **Left Navigation Sidebar Architecture:** Organizes slicers and reset controls cleanly.
- **Segment-to-Country Matrix:** Includes Conditional Formatting (Data Bars for volume, Heatmaps for margins).
- **Reset View Bookmark:** Single-click action clearing both visual cross-filtering and slicer selections.

---

## 📁 Repository Structure

```

├── 07) Financial Dashboard 2.pbix # Power BI Desktop Report File 
├── financial dashboard 1.png # Dashboard View Screenshot 
├── financial dashboard video .mp4 # Interactive Video Demo 
└── README.md # Detailed Project Documentation

```

---

## 💬 Feedback &amp; Continuous Learning
Since I am actively building my skills in Power BI, DAX, and Data Modeling, I know there is always room for improvement and optimization. If you have any feedback, suggestions, or constructive critiques, please feel free to open an issue or connect with me! 💡

---

## 👤 Author

**Rusiru Mihiranga**  
*Aspiring Data Analyst | Business Intelligence & Power BI Developer*


