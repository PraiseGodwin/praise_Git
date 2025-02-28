# **Inventory Forecasting Project - README**

## **Project Overview**
This project showcases an **Inventory Forecasting Dashboard** built using **Power BI & Excel**, aimed at helping businesses manage stock levels, prevent stockouts, and optimize supply chain efficiency. The dashboard provides real-time insights into total sales volume, stock levels, and products that require restocking. 

## **Project Goals**
- Predict inventory demand based on historical sales trends.
- Identify products that need restocking.
- Optimize reorder points to prevent overstocking or stockouts.
- Provide actionable insights through **Power BI visualizations**.

## **Dataset Description**
The dataset consists of **10,000+ records** and includes the following columns:

| Column Name | Description |
|-------------|-------------|
| **Product_ID** | Unique identifier for each product |
| **Product_Name** | Name of the product (e.g., Smartwatch, Refrigerator, Tablet) |
| **Category** | Product category (Accessories, Electronics, Appliances) |
| **Sales_Date** | Date of the sales transaction |
| **Sales_Volume** | Number of units sold on a given day |
| **Stock_Level** | Available stock for the product |
| **Lead_Time** | Time in days required to restock |
| **Supplier** | Name of the supplier |
| **Reorder_Point** | Minimum stock level before reordering |
| **Demand_Forecast** | Predicted demand based on historical sales |

## **Technology Stack**
- **Power BI** - Data visualization & dashboard creation
- **Excel** - Data preprocessing & forecasting functions

## **Power BI Dashboard Components**
1. **KPI Cards**: 
   - **Total Sales Volume**: Displays total sales across all products.
   - **Total Stock Level**: Shows the current inventory level.
   - **Products Needing Restock**: Indicates how many products are below their reorder points.

2. **Sales Volume by Year**: 
   - A **line chart** visualizing the trend of total sales over time.

3. **Sales Volume by Product Name**: 
   - A **donut chart** showing the proportion of sales across different product categories (e.g., Smartwatch, TV, Tablet, etc.).

4. **Reorder Status Table**: 
   - A **detailed table** listing product names, stock levels, reorder points, and categories.
   - Conditional formatting highlights **low-stock products** needing replenishment.

5. **Demand Forecast vs. Stock Level**: 
   - A **bar chart** comparing the predicted demand and available stock levels for different products.

6. **Category Filter/Slicers**: 
   - Buttons allow users to filter products by **Accessories, Appliances, and Electronics**.

## **Key Insights from the Dashboard**
- **Declining Sales Trend**: The sales volume trend shows a **decline from 2023 to 2024**, indicating potential seasonal changes or market shifts.
- **High Stock Levels vs. Demand**: Some products have **high stock levels** but low forecasted demand, suggesting the need for inventory reduction strategies.
- **Reorder Alerts**: 839 products have **fallen below the reorder point**, requiring urgent restocking to prevent shortages.
- **Category-Based Insights**: Electronics have the highest sales volume, while accessories show **consistent but moderate demand**.

## **How to Use the Dashboard**
1. **Load the dataset** into Power BI.
2. **Transform the data** in Power Query, ensuring correct data types and structure.
3. **Create key measures** using DAX formulas:
   ```DAX
   Reorder_Status = IF('Table'[Stock_Level] < 'Table'[Reorder_Point], "Reorder Needed", "Sufficient Stock")
   ```
4. **Build visuals** to reflect the data insights.
5. **Apply filters and slicers** to drill down into specific product categories or suppliers.

## **Future Enhancements**
- Automate data updates using **real-time database integration**.
- Add **supplier performance tracking** to optimize procurement decisions.
- Implement **machine learning forecasting models** to improve demand predictions.

## **Author**
**Godwin Praise Tobechi**  
📧 Email: godwinpraise377@gmail.com  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/praise-godwin-455a64198?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)  


