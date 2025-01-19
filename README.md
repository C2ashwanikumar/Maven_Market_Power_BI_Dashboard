# 🌟 Maven Market Business Insights Dashboard Project  

## 🚀 Overview  
Welcome to the Maven Market Business Insights Dashboard! This project leverages **Power BI** to analyze and visualize business data to uncover actionable insights. From customer trends to product performance and store analysis, this dashboard suite provides comprehensive tools for decision-making.  

---

## 📂 Data Sources  
The project uses the following datasets (CSV files):  
- **Transactions** (`MavenMarket_Transactions`)  
- **Calendar** (`MavenMarket_Calendar`)  
- **Customers** (`MavenMarket_Customers`)  
- **Products** (`MavenMarket_Products`)  
- **Regions** (`MavenMarket_Regions`)  
- **Returns** (`MavenMarket_Returns_1997-1998`)  
- **Stores** (`MavenMarket_Stores`)  

---

## 🛠️ Data Cleaning and Transformation  
Data cleaning and transformation were performed using **Power Query**, including:  
- 🧹 **Null Value Removal**: Ensured datasets were clean and reliable.  
- 🔄 **Data Type Conversion**: Standardized column formats for analysis.  
- 🏗️ **Dataset Merging**: Combined relevant tables for deeper insights.  
- 📊 **Calculated Columns**: Added custom columns to enhance analysis.  

---

## 📊 Dashboards  

### **1. Customer Dashboard**  
🌟 **Highlights**:  
- KPIs: `Total Customers`, `Revenue Per Customer`.  
- Visualizations:  
  - 📈 **Line Chart**: Tracks total customers and revenue per customer over time.  
  - 🥧 **Pie Charts**: Orders breakdown by income level and occupation.  
  - 📋 **Customer Table**: Displays top customers with transactions and revenue.  

---

### **2. Map Dashboard (Store Performance)**  
🌍 **Highlights**:  
- KPIs: `Total Stores`, `Average Revenue per Store`.  
- Visualizations:  
  - 📊 **Bar Graph**: Revenue breakdown by store type.  
  - 🗺️ **Map Visualization**: Displays top-performing stores with filters for country-wise analysis.  

---

### **3. Product Details Dashboard**  
🛒 **Highlights**:  
- KPIs:  
  - Monthly comparisons of `Revenue`, `Profit`, and `Orders` vs. Targets.  
  - Drill-through for **Top 10 Products**, showing eco-friendliness and health benefits.  
- Visualizations:  
  - 📉 **Line Charts**: Adjusted profit, total profit, total revenue, and cost.  
  - 🔎 **Product Insights**: Detailed views of each product's performance.  

---

### **4. Decomposition Tree and Key Influencers**  
🔍 **Key Features**:  
- **Decomposition Dashboard**:  
  - Visualizes contributing factors for metrics like revenue and profit.  
- **Key Influencers Analysis**:  
  - Examines the impact of customer attributes:  
    - Annual income.  
    - Occupation.  
    - Homeowner status.  
    - Marital status.  
    - Parental status.  

---

### **5. Custom Tooltip Dashboard**  
💡 **Custom Tooltips**:  
- Adds interactivity with additional contextual data on hover, enriching the user experience.  

---

## 📈 DAX Measures  
Key **DAX Measures** were created for analysis:  
- **Total Revenue**: `SUM(Transactions[Revenue])`  
- **Total Profit**: `SUM(Transactions[Profit])`  
- **Total Transactions**: `COUNTROWS(Transactions)`  
- **Total Customers**: `COUNT(Customers[CustomerKey])`  
- **Return Rate**: `(SUM(Returns[Returns]) / SUM(Transactions[Transactions])) * 100`  
- **Profit Margin**: `(SUM(Transactions[Profit]) / SUM(Transactions[Revenue])) * 100`  
- **Monthly KPIs**: Revenue, Profit, and Transactions by month.  

---

## 📌 Key Features  
1. **Interactive Dashboards**:  
   - Slicers and filters for dynamic exploration.  
2. **Advanced Analytics**:  
   - Decomposition trees and key influencer visuals.  
3. **In-depth Product Insights**:  
   - Drill-through functionality for targeted analysis.  
4. **Map Visualizations**:  
   - Geographical performance insights.  

