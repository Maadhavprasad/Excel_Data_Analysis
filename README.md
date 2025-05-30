# Excel_Data_Analysis
# 🛍️ Ferns and Petals Sales Analysis (Excel Project)

## 📌 Objective
Analyze the sales data of Ferns and Petals to uncover trends in customer behavior, product performance, and seasonal demand. Build an interactive Excel dashboard to support business decision-making.

---

## 📁 Dataset Overview
The dataset includes:
- Order ID
- Order Date & Delivery Date
- Product Category & Product Name
- City
- Occasion
- Quantity
- Price & Revenue

---

## 🔧 Data Cleaning & Preparation (Using Excel Power Query)

All data preparation was done in **Power Query**:
- Removed duplicate records
- Handled null/missing values in `Delivery Date`, `Revenue`, and `City`
- Split `Date` and `Time` fields if combined
- Converted `Order Date` and `Delivery Date` columns to proper datetime formats
- Created calculated columns:
  - `Order Month` (from Order Date)
  - `Delivery Month`
  - `Order Hour` (from time portion of Order Date)
  - `Order-Delivery Days` = `Delivery Date` - `Order Date`

---

## 🔁 Data Transformation & Relationships (Using Power Pivot)

Used **Power Pivot** to:
- Create relationships between multiple tables (e.g., Orders, Products, Locations)
- Built measures using DAX:
  - `Total Revenue` = SUM(Revenue)
  - `Avg Spend per Customer` = [Total Revenue] / DISTINCTCOUNT(Customer ID)
  - `Average Order-Delivery Time`
- Created calculated columns for performance analysis:
  - `Month Name` for sorting charts
  - `Year-Month` key for timeline filtering

---

## 📊 Analysis Performed

### 1. **Revenue Analysis**
- Revenue by Occasion
- Revenue by Product Category
- Monthly Revenue Trend

### 2. **Customer Behavior**
- Average customer spending
- Peak order hours
- Top 10 Cities by Orders

### 3. **Product Performance**
- Top 5 Products by Revenue
- Product popularity during festivals (e.g., Diwali, Raksha Bandhan)

### 4. **Operational Metrics**
- Average Order to Delivery Time
- Revenue vs. Time of Day

---

## 📈 Dashboard Features (Built in Excel)

Built an interactive dashboard with:
- Pivot Tables and Pivot Charts
- Slicers for:
  - Occasion
  - Order Date
  - Delivery Date
- KPIs at the top:
  - Total Orders
  - Total Revenue
  - Avg Delivery Time
  - Avg Customer Spend
- Charts:
  - Revenue by Occasion, Category, Month
  - Revenue by Hour
  - Top Products by Revenue
  - Top Cities by Orders

---

## 🔍 Insights

- **Highest revenue** from **Anniversary** and **Raksha Bandhan** orders
- **Colors** and **Soft Toys** were top-selling categories
- March and September showed **spikes in monthly revenue**
- Most orders occurred between **11 AM to 3 PM**
- Cities like **Dhanbad** and **Imphal** had highest order volume
---

## 🧠 Skills Demonstrated

- Power Query for data cleaning
- Power Pivot for DAX & relationships
- Pivot Tables & Charts for analysis
- Dashboard design using Excel
- Business interpretation of data

---

## 📌 Status: ✅ Completed
