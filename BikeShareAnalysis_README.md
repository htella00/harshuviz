# BikeShare_Analysis-Dashboard

## Problem Statement

 As a Data Analyst for a fictional bike-sharing company, the company needs a dashboard that displays key performance metrics, including hourly revenue analysis, profit and revenue trends, seasonal revenue, and rider demographics. The dashboard should align with the company's colors and design aesthetics. Additionally, we need to answer a central analysis question from the stakeholders: "Can we raise prices next year?"

### Steps Followed 

- Step 1 : Created a database and imported the bike-share data using the SQL Server Management Studio.
- Step 2 : Developed SQL queries to clean and prepare the data, including joining tables and performing calculations for revenue and profit.
- Step 3 : Created a data model in SQL Server by combining data from different tables using SQL UNION and JOIN operations.
- Step 4 : Built and tested SQL queries to calculate key metrics such as revenue and profit, and created common table expressions (CTEs) for cleaner code.
- Step 5 : Connected Power BI to the SQL Server database, using the SQL queries to bring in the cleaned data.
- Step 6 : Designed a Power BI dashboard with various visualizations, including line charts, bar charts, and matrices, to display revenue, profit, and rider demographics.
- Step 7 : Added interactive features to the dashboard, such as slicers for filtering data by year and animated elements to enhance the visual appeal.
- Step 8 : Tested and refined the dashboard to ensure it met the stakeholders' requirements and provided clear insights.
- Step 9 : Conducted a price elasticity analysis to determine if the company could raise prices next year without negatively impacting demand.

### Findings 
- To answer the question, Yes we can raise the prices for the upcoming year.
- The hourly sales data reveals that the most profitable hours are during the midday and early evening, particularly between 10 AM to 3 PM. This insight is critical for optimizing operations and possibly offering special promotions or adjusting pricing during these peak hours.
- The "Sum of Revenue by Season" bar chart indicates that Season 3 (likely the summer months) is the most profitable, generating 4.9M in revenue. This suggests that customer demand is highest during this period, which could be leveraged for targeted marketing campaigns.
- The "Sum of Riders by Rider Type" donut chart shows that 81.17% of riders are casual, while 18.83% are members. This demographic split highlights the importance of catering to casual riders, who form the majority of the customer base, while also exploring strategies to convert more casual riders into members.
- The line chart displaying KPIs over time shows consistent growth in the number of riders, revenue, and profit. This trend reflects the ongoing success of the service, with clear seasonal fluctuations that align with the previously noted peak in Season 3.

### Recommendations
- Introduce seasonal pricing models where prices are slightly higher during peak seasons (e.g., summer) and lower during off-peak times. This can maximize revenue while maintaining customer satisfaction.
- Launch a customer loyalty program that offers discounts or exclusive benefits to frequent riders, encouraging long-term commitment despite potential price increases.
- Use the additional revenue from the price increase to improve bike availability and maintenance, ensuring a high-quality service that justifies the higher prices.

### Snapshot of Final Dashboard
![Screenshot 2024-09-03 152415](https://github.com/user-attachments/assets/6b721864-c601-4222-a773-98233e1dfbbd)

### References
- BikeShare Analysis by AbsentData (Youtube)
