# Sales Data Analysis and Visualization

![Sales Analytics Dashboard](https://github.com/user-attachments/assets/fbfcc704-ee72-44f8-8c4f-1a0c188c8506)


## Project Overview
This project demonstrates how sales data can be transformed, analyzed, and visualized using **Power BI**. The focus is on uncovering trends, identifying top-performing products and cities, and understanding revenue metrics. The project showcases expertise in working with large datasets, transforming data, and creating interactive dashboards that enable strategic decision-making.

### Key Features:
- Data cleaning and transformation for analysis.
- Interactive dashboards to visualize sales trends and top performers.
- Business insights into product sales, city-based performance, and revenue distribution.

---

## Table of Contents
1. [Objective](#objective)
2. [Tools and Technologies Used](#tools-and-technologies-used)
3. [Data Description](#data-description)
4. [Step-by-Step Workflow](#step-by-step-workflow)
5. [Visualizations in Power BI](#visualizations-in-power-bi)
6. [Files in Repository](#files-in-repository)

---

## Objective
To analyze and visualize sales data for actionable business insights, enabling decisions such as:
- Identifying top-selling products and cities.
- Understanding sales performance over time.
- Measuring revenue metrics like total sales, profit margins, and quantity sold.

---

## Tools and Technologies Used

| **Tool**         | **Purpose**                                |
|-------------------|--------------------------------------------|
| **Power BI**      | Data transformation and interactive visualization |
| **Google Sheets** | Quick data exploration and cleaning         |


---

## Data Description
The dataset contains sales information, including:
- **Order ID**: Unique identifier for each transaction.
- **Product**: Name of the product sold.
- **Quantity Ordered**: Number of units sold.
- **Price Each**: Price per unit.
- **Order Date**: Date and time of the order.
- **Purchase Address**: Full address of the customer.
- **City**: City extracted from the purchase address.
- **Month**: Month of the sale (derived).
- **Sales**: Total sales amount (calculated).
- **Hour**: Time of the order (derived).

---

## Step-by-Step Workflow

### **1. Data Transformation**
- **Objective**: Clean and structure the dataset for analysis.
- **Key Steps**:
  - Imported the dataset into Power BI using the **Get Data** feature.
  - Promoted the first row to headers.
  - Detected and assigned appropriate data types to each column.
  - Split the `Order Date` column into separate `Date` and `Time` columns.
  - Extracted `City` from the `Purchase Address` column.
  - Calculated the `Sales` column as:
    ```
    Sales = Quantity Ordered * Price Each
    ```

### **2. Data Visualization**
- **Objective**: Create interactive and insightful dashboards.
- **Key Visualizations**:
  - **Sales Trend Over Time (Line Chart)**:
    - Shows monthly sales trends in chronological order.
    - Steps:
      1. Use the `Month` column for the x-axis.
      2. Aggregate the `Sales` column for the y-axis.
      3. Sort months by their numeric order.
  - **Top-Selling Products (Tree Map)**:
    - Highlights products based on total sales.
    - Steps:
      1. Drag `Product` to the **Category** field.
      2. Drag `Sales` to the **Values** field.
  - **Top 5 Products by Quantity Sold (Bar Chart)**:
    - Steps:
      1. Drag `Product` to the y-axis.
      2. Drag `Quantity Ordered` to the x-axis.
      3. Filter the chart to show the top 5 products.
  - **City-Wise Sales Distribution (Map)**:
    - Displays cities with their total sales.
    - Steps:
      1. Drag `City` to the **Location** field.
      2. Drag `Sales` to the **Size** field.
  - **Weekly Sales Distribution (Column Chart)**:
    - Shows sales by day of the week.
    - Steps:
      1. Extract the weekday from the `Date` column.
      2. Use the column as the x-axis and `Sales` as the y-axis.
  - **Revenue Metrics (Cards)**:
    - Display total sales, total units sold, and profit margins.
    - Steps:
      1. Use the **Card** visual.
      2. Aggregate the `Sales`, `Quantity Ordered`, and calculated `Profit Margin` fields.

### **3. Interactivity**
- **Slicers**:
  - Allow filtering by `Month` and `City`.
  - Adjusted slicer layouts for usability.
- **Filters**:
  - Added filters for `Product` and `Order Date` to drill down into specific data.

---

## Visualizations in Power BI
### Dashboard Highlights:
- **Sales Trends**: Understand performance across months and weekdays.
- **Product Insights**: Identify top-selling and underperforming products.
- **City-Based Performance**: Pinpoint regions contributing the most to revenue.
- **Interactive Exploration**: Filters and slicers allow in-depth data exploration.

![Sales Data_page-0001](https://github.com/user-attachments/assets/e39f0a7c-5e17-4559-9821-faec0e1772b9)


---



## Files in Repository

| **File Name**                  | **Description**                                              |
|--------------------------------|--------------------------------------------------------------|
| `sales_data.csv`               | Raw dataset used in the project.                            |
| `Sales_Analytics_Dashboard.pbix` | Power BI file containing the final dashboard.               |


---

