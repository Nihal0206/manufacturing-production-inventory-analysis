# Data Analysis of Bicycle Manufacturing Company
### Production & Inventory Analytics using Python, SQL & Power BI

---

## Overview

This project presents a **Production and Inventory Analysis** using the Microsoft **AdventureWorks** sample database.  
AdventureWorks is a fictional bicycle manufacturing company that represents real-world **ERP (Enterprise Resource Planning)** data.

The analysis focuses on the **Manufacturing and Inventory** domain with the objective of identifying:
- Production inefficiencies
- Major waste cost drivers
- Inventory utilization and turnover issues

An **interactive Power BI dashboard** is built by connecting to **SQL Server**, supported by data modeling and analytics.

---

## Data Source

- **Dataset:** Microsoft AdventureWorks Sample Database  
- **Domain Used:** Manufacturing & Inventory  
- **Purpose:** Learning, analytics, and portfolio demonstration

---

## Data Model

A **Star Schema** data model was implemented to improve performance and simplify analytical reporting.

![Data Model](images/data_model.png)

### Tables Used
- **Production Location** – Assembly locations and manufacturing stages  
- **Production Product** – Product attributes such as size, weight, and cost  
- **Product Category** – High-level product grouping  
- **Product Subcategory** – Detailed product classification  
- **Product Inventory** – Inventory quantity and stock details  
- **Scrap Reason** – Manufacturing waste reasons  
- **Work Order** – Production transactions  
- **Work Order Routing** – Production scheduling data  
- **Sales Order Detail** – Sales transaction data  
- **Calendar** – Custom fiscal calendar (October–September)

---

## Tools & Technologies

- **SQL Server** – Data storage, joins, and extraction  
- **Power BI** – Data modeling, DAX measures, and dashboards  
- **Python** – Data preprocessing and validation  
- **DAX** – KPI creation and fiscal calendar logic  

---

## Dashboard Analysis

### Main Page

The dashboard is designed with an **app-like navigation interface**, allowing users to move between Production and Inventory views.

![Main Page](images/main_page.png)

---

## Production Overview

Provides a high-level summary of manufacturing performance.  
A **custom fiscal calendar (October–September)** was created using DAX.

![Production Overview Page](images/production_overview_page.png)

### Key KPIs
- Fiscal Year-to-Date Production  
- Fiscal Year-to-Date Waste Cost  
- Average Production Lead Time  
- On-Time Production Percentage  

![Production Overview KPI](images/production_overview_kpi.png)

---

## Category Analysis

Enables deeper investigation into **product-level and component-level production issues**.

![Production Category Analysis](images/Production%20Category%20Analysis.png)

### Pareto Charts

Used to identify the **most significant components and products** contributing to production volume and waste cost.

![Pareto Charts](images/Pareto_Charts.jpg)

### Waste Cost – Product Matrix

Breaks down waste cost by:
- Waste reason  
- Bikes vs Components  

Conditional formatting highlights high-cost defect areas.

![Waste Cost Matrix](images/Waste_Cost_Matrix.jpg)

### On-Time Production by Category

Shows the percentage of products completed on time across categories.

![On-Time Production by Category](images/On_time_production_by_category.jpg)

---

## Inventory Overview

Focuses on inventory utilization across assembly locations.

![Inventory Data Overview](images/Inventory%20data%20overview.png)

### Inventory KPIs
- Inventory Quantity  
- Inventory Value  
- Inventory Turnover  

![Inventory Overview KPI](images/inventory_overview_kpi.png)

### Inventory Turnover Analysis

Compares inventory turnover across fiscal years to support better production planning.

![Inventory Turnover](images/Inventory_tunrover_chart.jpg)

---

## Key Insights

- Pareto analysis identified components driving most production volume  
- Waste analysis highlighted major defect reasons increasing cost  
- Inventory analysis revealed overstocked assembly stages  
- On-time production analysis exposed scheduling inefficiencies  

---

## Conclusion

This project demonstrates how **data analytics and visualization** can:
- Identify manufacturing inefficiencies  
- Reduce waste cost  
- Improve inventory utilization  
- Support data-driven decision-making  

---

## Disclaimer

This project is created for **educational and portfolio purposes** using the publicly available **Microsoft AdventureWorks** sample dataset.  
All analysis and insights are independently developed.
