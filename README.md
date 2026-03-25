# amazon-sales-powerbi-dashboard
Interactive Power BI dashboard analyzing Amazon sales performance
 Amazon Sales Performance Dashboard (Power BI)

 Project Overview

This project presents an interactive **Amazon Sales Performance Dashboard** built using Microsoft Power BI.
The dashboard provides deep insights into sales trends, product performance, customer behavior, and order fulfillment.

The objective of this project is to transform raw e-commerce data into meaningful insights that support **data-driven decision-making**.

---

 Dataset Description

The dataset contains transactional-level Amazon sales data with the following key fields:

* Order ID
* Date
* Status (Shipped, Cancelled, Returned, etc.)
* Fulfilment type
* Sales Channel
* Product Category
* SKU & Style
* Quantity (Qty)
* Revenue (Amount)
* Customer Location (City, State, Country)
* Courier Status
* Promotion IDs
* B2B Indicator

---

 Data Cleaning & Preprocessing

The dataset was cleaned and prepared using Power BI Power Query:

✔ Removed Irrelevant Columns
✔ Data Type Conversion
✔ Handling Missing Values
✔ Standardization

* Uniform formatting for:

  * Category
  * Status
  * State names

---

##  Data Transformation & Modeling

###  Measures Created (DAX)

```DAX
Total Revenue = SUM(Amount)

Total Orders = COUNT(Order ID)

Total Quantity = SUM(Qty)

Average Order Value = DIVIDE(Total Revenue, Total Orders)

Cancelled Orders = CALCULATE(Total Orders, Status = "Cancelled")

Shipped Orders = CALCULATE(Total Orders, Status = "Shipped")
```


## 📈 Dashboard Features & Visualizations

The dashboard is divided into multiple analytical sections:


1. KPI CARDS
Total Orders
Total Quantity
Total Revenue
Average Order Value

👉 Visual Type: Card

 2. GAUGE CHART
Total Revenue vs Target

👉 Visual Type: Gauge

 3. LINE CHART (Sales Trend)
Total Revenue over time

👉 Visual Type: Line Chart

 4. LINE CHART (Orders Trend)
Total Orders by Year & Quarter

👉 Visual Type: Line Chart

 5. BAR CHART (Category Analysis)
Total Revenue by Category

👉 Visual Type: Clustered Bar Chart

 6. COLUMN CHART (Size Analysis)
Total Quantity by Size

👉 Visual Type: Clustered Column Chart

 7. DONUT CHART (Order Status)
Total Orders by Status

👉 Visual Type: Donut Chart

 8. TABLE VISUAL
ship-state
Revenue values

👉 Visual Type: Table

 9. SCATTER PLOT
Total Quantity vs Total Revenue
Category as legend

👉 Visual Type: Scatter Chart

 10. MULTI-CATEGORY COLUMN CHART
Revenue by ship-city and Category

👉 Visual Type: Clustered Column Chart (with Legend)

 11. HORIZONTAL BAR CHART (Order Status Detailed)
Status-wise order distribution

👉 Visual Type: Bar Chart

 12. SLICERS (FILTERS)
Dropdown Slicers:
Category
Size
Range Slicer:
Date (slider)

👉 Visual Type: Slicer


##  Key Insights

* Sales show a consistent upward trend
* “Set” category generates the highest revenue
* Major sales come from metropolitan cities
* Most orders are successfully delivered
* Average order value remains stable

---

## 🎯 Conclusion

This dashboard provides a comprehensive view of Amazon sales performance, enabling businesses to:

* Monitor KPIs in real time
* Identify high-performing products
* Analyze customer and regional trends
* Improve order fulfillment strategies

---

## 🛠 Tools & Technologies

* Microsoft Power BI
* Power Query (Data Cleaning)
* DAX (Data Analysis Expressions)

---

## 📸 Dashboard Preview

**##Page 1:**

<img width="800" height="661" alt="dashboard-preview 1" src="https://github.com/user-attachments/assets/11b70f8f-aec8-4729-9065-6793a5096485" />

**##Page 2:**

<img width="800" height="661" alt="dashboard-preview 2" src="https://github.com/user-attachments/assets/cb948403-66ff-4344-b6ad-5092b30ee1ab" />


## 🚀 Future Enhancements

* Profit & Cost Analysis
* Customer Segmentation
* Forecasting & Predictive Analytics
* Real-time data integration

---

## 👤 Author

M.S.Varsha
(Student)

---
