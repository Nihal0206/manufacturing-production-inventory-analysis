# Production & Inventory Analytics – Manufacturing Domain

## Overview
This project analyzes production efficiency, waste cost, and inventory utilization
for a bicycle manufacturing company using the AdventureWorks dataset.
The objective is to identify manufacturing bottlenecks and high-cost areas.

## Business Problem
Manufacturing organizations commonly face:
- High scrap and waste cost
- Delays in production completion
- Poor inventory turnover

This project uses analytics to address these challenges.

## Data Source
AdventureWorks sample database (Manufacturing & Inventory modules).

## Data Modeling
- Star schema data model implemented
- Fact tables: WorkOrder, WorkOrderRouting
- Dimension tables: Product, Category, Scrap Reason, Location, Calendar
- Custom fiscal year (October–September) created using DAX

## Tools & Technologies
- SQL Server
- Power BI
- Python
- DAX

## Key Insights
- Pareto analysis identified major components driving production volume
- Waste analysis highlighted key defect reasons increasing costs
- Inventory analysis revealed overstocked assembly stages
- On-time production analysis showed scheduling inefficiencies

## Disclaimer
This project is created for learning and portfolio purposes using publicly available data.
All analysis and insights are independently developed.
