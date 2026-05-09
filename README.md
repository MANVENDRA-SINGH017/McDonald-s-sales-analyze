# McDonald-s-sales-analyze
This project analyzes McDonald’s sales data to uncover insights into revenue performance, customer behavior, and product popularity using Excel, Power Query, and Power Pivot.

# McDonald's Sales Analysis Dashboard

## Overview
This project analyzes McDonald's sales data to uncover insights into revenue performance, customer behavior, and product popularity using Microsoft Excel, Power Query, and Power Pivot.

The goal of this project is to transform raw transactional data into meaningful business insights and present them through an interactive dashboard.

---

## Dataset
The project is based on two datasets:

- **Menu List**
  - menu_item_id
  - item_name
  - category
  - price

- **Order Details**
  - order_details_id
  - order_id
  - order_date
  - order_time
  - item_id

---

 Data Preprocessing
Data cleaning and transformation were performed using Power Query:

- Handled missing values in `item_id` using forward fill
- Removed invalid or erroneous date records
- Standardized data types (date, time, numeric)
- Created derived columns:
  - Time of Day (Morning, Afternoon, Evening, Night)
  - Day Name
  - Month
  - Weekday/Weekend classification

---

 Data Modeling
A relational data model was created in Power Pivot:

- **Fact Table:** Order Details
- **Dimension Table:** Menu List
- Relationship:
  - `menu_list[menu_item_id] → order_details[item_id]`

This structure enables efficient aggregation and analysis without data duplication.

---

 Key Metrics (DAX Measures)

- Total Revenue  
- Total Orders  
- Total Items Sold  
- Average Items per Order  

---

 Analysis Performed

The project answers the following business questions:

1. Total sales revenue for each category  
2. Number of orders per day  
3. Most frequently ordered menu item  
4. Total revenue generated  
5. Revenue comparison by category over months  
6. Average number of items per order  
7. Order volume by time of day  
8. Weekday vs weekend sales trends  
9. Category performance across months  
10. Top 5 menu items by sales  

---

## Dashboard Features

- Interactive Excel dashboard  
- Slicers for filtering (Month, Category, Time of Day, Day Type)  
- KPI cards for key metrics  
- Trend analysis using line charts  
- Product and category comparisons  

---

 Tools Used

 Microsoft Excel  
 Power Query (Data Cleaning & Transformation)  
 Power Pivot (Data Modeling & DAX)  



 Key Insights

- Identification of top-performing menu items and categories  
- Clear understanding of peak ordering times  
- Revenue trends across months and customer behavior patterns  
- Comparison between weekday and weekend sales performance  

---

 Conclusion

This project demonstrates end-to-end data analysis using Excel, from data preprocessing to dashboard creation. It highlights the ability to clean, model, and visualize data effectively while deriving actionable business insights.

---

## Author
Manvendra Singh Bhati
