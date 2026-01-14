# Optimizing Power BI DirectQuery Performance using Aggregations

## Project Overview
This project demonstrates how to optimize report performance in Power BI when working with **DirectQuery mode**. Using the Adventure Works dataset, the focus is on reducing query load on the data source and improving report responsiveness through **query reduction techniques, aggregations, and storage modes**.



## Problem Statement
The Adventure Works dataset contains a very large fact table. When users interact with visuals and filters in DirectQuery mode, Power BI sends queries to the data source each time. This resulted in **slow report performance and increased query workload** on the database.



## Solution Approach
To address the performance issue, the following optimization steps were implemented:

- Established a DirectQuery connection to the dataset  
- Applied **query reduction settings** to limit unnecessary queries  
- Created an **aggregated table (SalesAgg)** using Power Query  
- Grouped data by Order Date to reduce granularity  
- Established relationships between aggregated and dimension tables  
- Configured **aggregation behavior** so Power BI can automatically use the aggregated table when possible  



## Key Features Implemented
- DirectQuery optimization using query reduction  
- Aggregations for large fact tables  
- Improved query performance and report interactivity  
- Proper data modeling with fact and dimension tables  



## Tools & Technologies
- Power BI Desktop  
- Power Query Editor  
- DirectQuery mode  
- Aggregations  
- Data modeling concepts (fact & dimension tables)  



## Key Learnings
- How DirectQuery impacts report performance  
- How aggregations reduce query workload on the data source  
- Difference between Import, DirectQuery, and Dual storage modes  
- How Power BI automatically selects aggregated tables for queries  



## How to Use This Project
1. Download and open the `.pbix` file in Power BI Desktop  
2. Explore the data model and aggregation settings  
3. Review query reduction options and storage modes  
4. Interact with visuals to observe performance optimization  



## Conclusion
DirectQuery enables real-time data analysis but can negatively impact performance if not optimized. By applying query reduction strategies and using aggregations effectively, Power BI reports can achieve **faster performance and a smoother user experience**, even with large datasets.
