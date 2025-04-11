# Plant-Company-Performance-Analysis

This project demonstrates my ability to utilize Power BI to create a dynamic and informative performance dashboard. The dashboard visualizes data related to sales, accounting, and product performance, which can be useful for analysis in various industries.

## The Final Dashboard 
![image](https://github.com/user-attachments/assets/d1ff7bec-56a6-4f4a-8555-c999a4896cd8)


## Dataset
The dataset used for this project covers the time period from 2022 to 2024. It consists of three main tables within an Excel workbook, each containing approximately 3,000 rows:
1. **Sales Data (Fact Table)**: Includes fields such as product ID, sales quantity, sales price, cost of goods sold, invoice date, and associated account details.
2. **Account Table**: Contains account information, including account ID, country code, latitude, and longitude.
3. **Product Hierarchy**: This table features various levels to drill down into product specifics, including product family, group, name, size, and type.

## Key Steps in Building the Dashboard
1. **Data Import and Preparation**:
   - Imported the Excel dataset using Power Query.
   - Cleaned the data by renaming columns for clarity, removing duplicates to ensure accuracy, and checking the data types.

2. **Data Modeling**:
   - Created a date table to facilitate better time based analysis.
   - Added several DAX measures, including:
     - **Sales**: Total sales computed using SUM of sales from the fact table.
     - **Gross Profit**: Calculated as Sales minus Cost of Goods Sold (COGS).
     - **Quantity Sold**: Total units sold during the specified period.
     - **Year-to-Date `(YTD)`**: Enables analysis of metrics from the start of the current year (2024) up to the selected date, allowing users to track performance over time.
     - **Prior Year-to-Date `(PYTD)`**: Facilitates comparison of the current year’s performance with the previous year (2023) for the same period, providing critical insights into business trends and seasonal fluctuations.

3. **Visual Development**:
   - Designed the dashboard layout using various visual elements such as cards, scatter charts, and waterfall charts to highlight key performance indicators.
   - Incorporated dynamic features using slicers, which empower users to filter the data based on selected metrics `[Sales, Gross Profit, Quantity]` and specific timeframes.

4. **Conditional Formatting**:
   - Applied conditional formatting to key visuals to enhance their appeal and make it easier for users to identify significant performance trends at a glance.

5. **Final Review and Publishing**:
   - Conducted a thorough review of the dashboard's alignment and functionality.

## Features of the Dashboard
- **Dynamic Metrics**: Users can seamlessly switch between various performance metrics `[Sales, Gross Profit, Quantity]` using intuitive slicers.
- **YTD and PYTD Analysis**: The dashboard includes measures for both Year-to-Date and Prior Year-to-Date, allowing users to:
- **YTD**: Analyze current performance metrics from January 2024 to the present day and understand operational performance over the year.
- **PYTD**: Compare these metrics against corresponding data from the previous year, supporting effective trend analysis and decision-making.
- **User-Friendly Design**: The layout is designed to be clear and intuitive, ensuring users can navigate the dashboard effortlessly and extract valuable insights promptly.
-----------

## Key Insights 📊

- **2024 vs 2023 Performance**: Sales down by 135.9K and Gross Profit down by 77.6K by April 2024.
- **Top Underperforming Countries**: Canada, Germany, Croatia, and Colombia showed major drops. China had the biggest drop in 2023 (-760.4K).
- **Product Trends**: March had the highest YTD values in 2024 across all product types (Indoor, Landscape, Outdoor), with a drop in April suggesting seasonality.
- **Profitability Segmentation**: Most accounts are low-margin, low-value. A few high-value, high-profit accounts should be prioritized.
- **Stable GP%**: Despite revenue shifts, Gross Profit % stayed steady around 40% along the 3 years, showing strong cost control.
