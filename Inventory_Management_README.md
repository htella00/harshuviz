
### Inventory Management Dashboard

### Problem Statement

 Optimize the inventory management system for a warehouse or in-plant inventory. The goal is to develop a comprehensive dashboard that includes:

- ABC Inventory Classification based on revenue generated
- XYZ Classification based on demand certainty (X: constant demand, Y: variable demand, Z: uncertain demand)
- Calculation of key metrics like Inventory Turnover Ratio (ITR), Safety Stock, and Reorder Points
- Classification of stock status (in stock, out of stock, or below reorder point)
- Demand forecasting for the upcoming period

This analysis will help inventory managers effectively manage stock levels, improve service levels, reduce stockouts, and minimize overstocking, thereby optimizing inventory operations.


### Steps Followed

- Step 1. Data Loading: Loaded stock and order data from an Excel sheet, representing typical ERP data, including fields such as SKU ID, stock quantity, lead times, and order quantities.
  
- Step 2. Data Preparation: Ensured correct data types (numbers, dates, currencies) for all fields before proceeding with calculations.

- Step 3. ABC Classification :
   - Calculated annual sales for each SKU based on order data from the past year.
   - Computed annual revenue by multiplying the sales quantity with unit prices.
   - Determined the percentage share of revenue for each SKU.
   - Classified SKUs into A (high value), B (medium value), and C (low value) categories using the Pareto principle.

- Step 4. XYZ Classification :
   - Analyzed weekly demand for each SKU by creating a new weekly demand table.
   - Calculated average weekly demand and standard deviation for each SKU.
   - Derived the Coefficient of Variation (CV) and classified SKUs into X (constant demand), Y (variable demand), and Z (uncertain demand) categories.

- Step 5. Inventory Turnover Ratio (ITR) : 
   - Calculated ITR by dividing annual sales by the current stock value to measure warehouse efficiency.

- Step 6. Safety Stock & Reorder Points : 
   - Computed safety stock based on peak weekly demand, maximum lead time, and average weekly demand.
   - Determined reorder points as the sum of safety stock and average consumption.
   - Identified SKUs that required reordering based on stock levels falling below the reorder point.

- Step 7. Stock Status Classification : 
   - Classified SKUs into three categories: in stock, out of stock, and below reorder point.

- Step 8. Visualization : 
   - Developed visualizations for ABC and XYZ classification matrices, distribution of revenue, current stock value, inventory turnover ratio, and reorder requirements.
   - Created a demand forecast using Power BI’s built-in exponential smoothing technique.


### Findings

- ABC Classification : 
  - High-value SKUs (A category) accounted for 70% of total revenue, while low-value SKUs (C category) generated the least revenue but comprised the majority of stock.
  
- XYZ Classification : 
  - X category items had constant demand, while Z category items exhibited high demand uncertainty, leading to higher stock levels to prevent stockouts.
  
- Inventory Turnover : 
  - The highest ITR was observed in A category and X category SKUs, indicating efficient management. However, Z category SKUs (uncertain demand) had low ITR, suggesting overstocking.
  
- Reorder Analysis : 
  - 274 SKUs required immediate reordering as their stock levels had fallen below the reorder point.

- Sales Forecast:
  - A weekly sales forecast was developed using Power BI’s exponential smoothing method. The forecast predicted sales trends for the upcoming weeks, allowing the warehouse to anticipate demand and adjust stock levels accordingly.


### Recommendations

-  Focus on High-Value Items : Maintain optimal stock levels for A category items to ensure high service levels without overstocking.
  
- Improve Z Category Efficiency : For SKUs with uncertain demand (Z category), consider reducing stock levels to improve the inventory turnover ratio while maintaining service levels.
  
- Forecasting and Planning : Leverage demand forecasting models to anticipate future demand and align stock levels accordingly to minimize stockouts and overstocking.
  
-  Regular Review of Reorder Points : Continuously review and adjust reorder points based on demand patterns, especially for items with high variability in demand (Y and Z categories).

-  Automation : Implement an automated inventory control system to track stock levels in real time, alerting managers when stock falls below reorder points, improving efficiency.


### Snapshot of The Dashboard
![Screenshot 2024-09-03 153048](https://github.com/user-attachments/assets/a50bd7be-7855-49e8-a717-e94f02f25c84)

Ref & DataSource : https://drive.google.com/file/d/15uoiFP5t3eV5SRrkv42vdwu8klxENbx2/view
