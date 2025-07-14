📦 Inventory Management Dashboard – Power BI
Overview
This is an advanced, industry-level inventory analytics project built using Power BI. The goal was to analyze warehouse inventory data to identify which products are high-value, which ones need to be reordered, and how efficiently the stock is turning over — ultimately helping reduce holding costs and avoid stockouts.

Project Summary (Layman Explanation)
Imagine managing a warehouse with 303 SKUs. Every day, you need to answer questions like: Which products are running low? How many items are out of stock? What’s the total inventory value? Which items are critical to revenue and need constant attention?
To solve this, I built a fully dynamic and interactive Power BI dashboard that automates the tracking and classification of inventory based on value, demand pattern, reorder thresholds, and more.

The dashboard clearly shows that:

Total inventory value in the warehouse is ₹77.33M

We are tracking 303 SKUs

275 SKUs need to be reordered

10 SKUs are completely out of stock

The inventory turnover ratio is 5.46, which means the stock is cycling 5.46 times a year on average

Key Visuals and Insights

ABC Classification: SKUs are classified into A (High Value), B (Medium Value), and C (Low Value) using cumulative revenue shares.

For instance, A-class SKUs (Variable Demand) contribute ₹232.86M in revenue.

XYZ Classification: Based on demand variability:

Y = Variable demand

Z = Uncertain demand

Inventory Turnover Ratio: At 5.46, it shows how efficiently inventory is moving.

Reorder Point & Safety Stock: Calculated for each SKU based on peak demand and lead times.

Stock Status: Automatically identifies whether an SKU is “In Stock,” “Below Reorder Point,” or “Out of Stock.”

Sales & Demand Trends: Line charts for weekly sales and demand show seasonality and trends over time.

How It Works (Technical Summary)

Safety Stock = (Peak Weekly Demand × Max Lead Time ÷ 7) − (Avg Weekly Demand × Avg Lead Time ÷ 7)

Reorder Point = Safety Stock + (Avg Weekly Demand × Avg Lead Time ÷ 7)

Stock Status is evaluated using a conditional DAX formula comparing current stock vs reorder point

Inventory Turnover Ratio = Annual Sales Quantity ÷ Current Stock Quantity

SKUs to Reorder are dynamically counted where the current quantity < reorder point

All of this is powered through DAX calculations, LOOKUPVALUEs across tables, and visualized using cards, bar charts, donut charts, and trend lines.

Business Value
This dashboard enables proactive inventory management. It flags items at risk of stockouts, improves order planning, and helps warehouse managers focus on high-impact SKUs based on value and variability. It also reduces capital locked in low-moving inventory.

Tech Stack

Power BI for dashboard creation

DAX for business logic and custom calculations

Excel for initial data prep

Real-World Applications

Retail and warehouse operations

Demand planning teams

Inventory optimization in FMCG, e-commerce, and manufacturing
