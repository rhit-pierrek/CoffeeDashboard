# Coffee Sales Dashboard Project

## Overview
This project involves creating an interactive Coffee Sales Dashboard in Excel using data transformation techniques, pivot tables, and pivot charts. The dashboard dynamically visualizes coffee sales data across different countries, customer segments, and timeframes. 

## Project Workflow

### 1. Data Gathering
The dataset consists of three primary tables:
- **Orders Table**: Contains transaction details including order ID, date, customer ID, product ID, and quantity.
- **Customers Table**: Holds customer details such as customer ID (primary key), name, email, country, and loyalty card status.
- **Products Table**: Stores product information including product ID (primary key), coffee type, roast type, size, unit price, and profitability.

lookup operations used to integrate the data across tables:
- **XLOOKUP**: Used to retrieve customer details from the Customers Table.
- **INDEX-MATCH**: Applied to extract product details dynamically from the Products Table.

### 2. Data Transformation
Data cleaning and transformation steps included:
- Populating missing values using **XLOOKUP** and **INDEX-MATCH**.
- Creating new calculated fields:
  - **Sales Amount** (`Unit Price * Quantity`)
  - **Expanded Coffee Type and Roast Type Names** (via **IF functions** for readability).
- Formatting numerical and date fields:
  - Date format adjusted to `DD-MMM-YYYY` for consistency.
  - Currency formatting applied to sales figures.
- Handling missing data:
  - Adjusting formulas to return blank values instead of zeros when information is unavailable.

### 3. Converting Data to Tables
The dataset was converted into an **Excel Table (Ctrl + T)** named `OrdersTable`. This allows for automatic expansion of pivot tables when new data is added.

### 4. Data Analysis with Pivot Tables
Three pivot tables were created for analysis:
1. **Total Sales Over Time** (Line Chart):
   - Summarizes total sales over months, split by coffee type.
2. **Sales by Country** (Bar Chart):
   - Displays total sales figures by country.
3. **Top 5 Customers** (Bar Chart):
   - Ranks the top five customers based on total purchases.

### 5. Visualization Using Pivot Charts
Pivot charts were created and customized:
- **Line Chart**: Depicting total sales trends over time.
- **Bar Charts**: Displaying sales distribution by country and top customers.

### 6. Adding Interactive Elements
For better a better user experience slicers were integrated:
- **Timeline Slicer** (for filtering data over different time periods).
- **Three Slicers**:
  - **Roast Type** (Dark, Medium, Light)
  - **Size** (0.2kg, 0.5kg, 1kg, 2.5kg)
  - **Loyalty Card Status** (Yes/No)

Slicers were formatted for a cohesive look, and **report connections** were made so all visualizations update simultaneously based on user selections.

### 7. Creating the Final Dashboard
- A new worksheet named `Dashboard` was created.
- Pivot tables and slicers were arranged for usability.
- Formatting included:
  - **Removing gridlines** for a clean interface.
  - **Disabling formula bars and row/column headers** to create a seamless dashboard experience.
  - **Enabling scroll bars** to allow navigation across different screen sizes.

## Why We Used These Processes

### **1. XLOOKUP vs. INDEX-MATCH**
- **XLOOKUP** is easier for simple lookups but requires multiple formulas.
- **INDEX-MATCH** is more dynamic, allowing one formula to populate multiple columns efficiently.

### **2. Using Pivot Tables & Charts**
- Pivot tables enable quick data aggregation without manual calculations.
- Pivot charts provide a dynamic visualization of sales trends, allowing for easy business insights.

### **3. Table Conversion (Ctrl + T)**
- Automatically expands pivot tables when new data is added.
- Improves formula referencing and structured data management.

### **4. Slicers & Timelines**
- Provide an interactive way to filter data without modifying formulas manually.
- Enable real-time updates to visualizations for better data exploration.




