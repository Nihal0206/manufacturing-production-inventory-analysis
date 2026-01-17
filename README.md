# Data Analysis of Bicycle Manufacturing Company Using Python, SQL and Power BI

## Overview

This project goes through the **Production and Inventory Analysis** of the Microsoft **AdventureWorks** Database.  
AdventureWorks is a fictional bicycle manufacturing company that contains standard transactional data from an
**Enterprise Resource Planning (ERP)** system.

The database includes multiple business scenarios such as **Human Resources, Product Management,
Manufacturing, Purchasing, Inventory, Sales, and Administration**.  
This analysis focuses specifically on the **Manufacturing and Inventory** domain.

**Microsoft Power BI** has been used to build an interactive dashboard by connecting to **SQL Server**.

---

## Data Source

The dataset used in this project is the **AdventureWorks sample database** provided by Microsoft for
learning and analytical purposes.

---

## Data Model

Defining an effective data structure is essential for building efficient dashboards.
A **Star Schema** data model was implemented to improve query performance and simplify analysis.

![Data Model](images/DataModel.png)

### Tables used in the model

- **Production Location** – Assembly locations and manufacturing stages  
- **Production Product** – Product details such as size, weight, and cost  
- **Production ProductCategory** – High-level product categories  
- **Production ProductSubcategory** – Detailed product subcategories  
- **Production ProductInventory** – Inventory quantity and stock data  
- **Production ScrapReason** – Manufacturing waste and defect reasons  
- **Production WorkOrder** – Production transaction records  
- **Production WorkOrderRouting** – Production scheduling and routing details  
- **Sales SalesOrderDetail** – Transactional sales data  

---

## Built With

- **Python**  
- **Power BI**  
- **SQL Server**

---

## Analysis

### Main Page

The dashboard is designed with an **app-like navigation interface**.
The main page provides navigation to **Production Overview** and **Inventory Overview** sections.

![Main Page](images/Main Page.png)

---

### Production Overview

![Production Overview Page](images/Production Overview Page.png)

The dashboard follows **fiscal year reporting**.
A custom **date table using DAX** was created to generate fiscal year segregation.

**Fiscal Year Assumption:**  
October 1st to September 30th.

This page provides a high-level overview of manufacturing performance using custom KPIs.

![Production Overview KPI](images/Production Overview KPI.png)

#### Charts on the page

**Cumulative Multiline Chart**  
Shows cumulative production totals by fiscal year and helps identify manufacturing bottlenecks.

**Donut Chart – Actual Cost by Assembly Location**  
Displays cost distribution across different assembly stages.

**Waste Cost by Year**  
Shows the trend of manufacturing waste cost over time.

![Waste Cost by Year](images/Waste cost by the Year.png)

---

### Category Analysis

The Category Analysis page enables deeper investigation into product-level and component-level
manufacturing issues.

![Production Category Analysis](images/Production Category Analysis.png)

#### Pareto Charts

Pareto charts are used to identify the **most significant components and products**
contributing to production volume and waste cost.

![Pareto Charts](images/Pareto_Charts.png)

#### Waste Cost – Product Matrix

This matrix visual highlights waste cost by:
- Waste reason  
- Bikes vs Components  

Conditional formatting emphasizes high-cost defect areas.

![Waste Cost Matrix](images/Waste_Cost_Matrix.png)

#### On-Time Production by Category

Displays the percentage of products completed on time across different categories.

![On-Time Production by Category](images/On_time_production_by_category.png)

---

### Inventory Overview

The Inventory Overview analyzes stock utilization and efficiency.
Due to limited supply chain data, the analysis assumes a **single inventory location**.

![Inventory Data Overview](images/Inventory data overview.png)

#### Inventory KPIs

![Inventory Overview KPI](images/Inventory Overview KPI.png)

- Inventory Quantity  
- Inventory Value  
- Inventory Turnover  

#### Inventory Analysis Charts

**Inventory Quantity & Value by Assembly Location**  
Shows where most inventory value is held.

**Inventory Turnover Multiline Chart**  
Compares inventory turnover across fiscal years.

![Inventory Turnover](images/Inventory_turnover_chart.png)

---

## Conclusion

This project demonstrates how **data analytics and visualization** can be applied to
manufacturing data to:

- Identify production inefficiencies  
- Reduce waste cost  
- Improve inventory utilization  
- Support data-driven decision making  

---

## Disclaimer

This project is created for **educational and portfolio purposes** using the publicly available
**AdventureWorks** dataset.  
All analysis, dashboards, and documentation have been independently developed.
