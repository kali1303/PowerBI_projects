# PowerBI_projects

# Pizza Sales Report


## Problem Statement

Pizza companies often struggle to understand customer preferences, identify best-selling products, and optimize sales strategies due to scattered and unstructured data. This project addresses these challenges by analyzing sales data to uncover insights about top-performing pizzas, peak order times, and popular categories. By visualizing key metrics such as total revenue, average order value, and sales trends, the dashboard empowers decision-makers to make data-driven choices. The insights help improve inventory management, tailor marketing efforts, and boost overall profitability. This solution enables pizza businesses to stay competitive in a data-driven market.


### Steps followed 
### Step 1: Data Import & Initial Processing
Data Source: Imported the pizza_sales.csv dataset into Power BI Desktop.

Data Type Verification: Ensured correct data types for each column:

order_date: Date/Time

pizza_name, pizza_category, pizza_size: Text

quantity, total_price: Numeric

#### Data Quality Checks:

Enabled "Column Quality," "Column Distribution," and "Column Profile" in Power Query Editor.

Selected "Column profiling based on entire dataset" for comprehensive analysis.

Identified and removed any null or inconsistent entries.
YouTube
GitHub

### Step 2: Data Modeling
Relationships: Established relationships between tables, ensuring referential integrity.

#### Calculated Columns:

Month: Extracted from order_date for monthly analysis.

Day of Week: Derived to analyze weekly trends.

### Step 3: Report View – Page 1 (Sales Overview)
#### 🎯 KPIs Displayed:

Total Revenue: $817,860

Total Pizzas Sold: 49,574 units

Total Orders: 21,350

Average Order Value: $38.32

![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/KPIs.png?raw=true)

#### 📊 Revenue by Day of the Week:
Highest Sales: Fridays – $136,000

Lowest Sales: Mondays – $99,200

Visualization: Clustered bar chart depicting daily revenue.


![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Daily_trends.png?raw=true)

### 📅 Monthly Revenue Trend:
Peak Month: July with $72,560 in sales.

Lowest Month: October with $60,000 in sales.

Visualization: Line chart depicting monthly revenue fluctuations.

![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Monthly_trends.png?raw=true)

### 🍕 Revenue by Pizza Category:
Classic: $220,000 (26%)

Supreme: $208,000 (25%)

Chicken: $180,000 (24%)

Visualization: Donut chart illustrating category-wise revenue distribution.


![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Sales_by_pizza.png?raw=true)

### 📏 Sales by Pizza Size:
Large: $375,320 (46%)

Medium: $249,300 (30%)

Regular : $178,080 (22%)

Visualization: Bar chart showing revenue by pizza size.



  
### Step 4: Report View – Page 2 (Deep Dive Analysis)
#### 🔝 Top 5 Pizzas by Revenue,Quantity,Orders:
### By Revenue
Thai Chicken Pizza – $43,430

BBQ Chicken Pizza – $42,770
 
The California Chicken Pizza - $41,410

Classic Deluxe Pizza – $38,180
  
The Spicy Italian Pizza - $34,830



![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Top_selling_pizza.png?raw=true)

#### 📉 Bottom 5 Pizzas by Revenue,Quantity,Orders:
### By Revenue
The Spinach Pesto Pizza – $15,600

The Mediterranean Pizza – $15,360

The Spinach Supreme Pizza - $15,280

The green Garden Pizza - $15,960

The Brie Carre Pizza - $11,590



![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Bottom_pizza.png?raw=true)



----------------------------------------------------

### 📌 Quick Glance Insights (Summary Box Purpose)


![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Quick_details_pizza.png?raw=true)

✅ This box provides a concise summary of key insights from the dashboard.

🔍 It is intended for users who want to understand performance quickly without analyzing each chart.

🎯 Highlights the busiest days, months, top-performing categories, and pizza sizes.

🗓️ Busiest Days & Times:

Orders peak during weekends, especially on Friday and Saturday evenings.

Helps identify when to expect the highest order volumes.

📅 Top Performing Months:

Most orders come from July and January, indicating seasonal peaks.

📦 Sales Performance:

The Classic category leads in both total orders and revenue.

Large size pizzas contribute the most to overall sales figures.

## 🧮 Step 5: DAX Measures Implemented
Total Revenue: SUM(pizza_sales[total_price])

Total Orders: DISTINCTCOUNT(pizza_sales[order_id])

Average Order Value: [Total Revenue] / [Total Orders]

Total Pizzas Sold: SUM(pizza_sales[quantity])

Average Pizzas per Order: [Total Pizzas Sold] / [Total Orders]

Month-over-Month Growth: Utilized DATEADD and CALCULATE functions for dynamic comparisons.

## 📆 6. Time Period Slicer (Date Range Filter)
🔄 Interactive Date Slicer is added at the top right to filter the report based on a specific time period.

👀 Users can view insights for any selected date range between Jan 1, 2015 to Dec 31, 2015, helping focus on a specific month, quarter, or season.

🧠 This enables:

Identifying seasonal sales trends (e.g., Classic pizza in July and January).

Filtering total revenue, orders, and pizza sold during custom periods.

Making period-based comparisons (like first half vs second half of the year).

📊 All visualizations — KPIs, charts, category-wise sales, and size breakdowns — automatically update based on the selected date range.

⚙️ A must-have feature for dynamic reporting, allowing users to perform ad-hoc analysis with just a few clicks.

## The Pizza sales report images:
### Page 1
![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Pizza_sales_1.png?raw=true)

### Page 2
![Pizza KPI Dashboard](https://github.com/kali1303/PowerBI_projects/blob/main/Pizza/Pizza_sales_2.png?raw=true)

## 📌 Conclusion
This Pizza Sales Report offers a comprehensive overview of key performance metrics including revenue, order trends, and category-wise sales.
By identifying top and bottom-selling pizzas, it helps the business make data-driven decisions to optimize offerings.
Monthly and daily trends reveal high-demand periods, enabling smarter promotional planning.
The report empowers the organization to address underperforming areas through targeted strategies like discounts or campaigns.
Overall, it serves as a valuable tool for enhancing customer engagement and maximizing sales performance.



