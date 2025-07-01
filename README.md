# RetailPerformanceOptimization
🚀 Project Objective
This project aims to support strategic decision-making in supply chain and logistics management by analyzing sales and delivery performance. Using BI tools, we identify optimal regions for freight allocation to enhance operational efficiency and reduce return rates.

## 📊 Datasets Used
We used the publicly available dataset from the TikTok "Unlock Operation Insights – Analyze Supply Chain Data!" challenge.
[Download Dataset](https://drive.google.com/drive/folders/19do1f_oSnW5n3GEqgwAUZLF-eLEpb5J-?usp=sharing)

Size: 29 columns × ~10,000 records

Key features:

- Customer details (Region, Segment)

- Order info (Sales, Profit, Quantity, Returned status)

- Product hierarchy (Category, Sub-Category)

- Shipping details (Mode, Cost, Delivery Days)

## 📈 Dashboard Preview
![image](https://github.com/user-attachments/assets/1af7d16e-b8c5-42ab-87e6-20e19ed589dd)

## 🧠 Methodology
ETL Process:
- Developed in SSIS
- Extracted data from flat files → transformed → loaded into a star-schema Data Warehouse
OLAP Cube Construction:
- Designed star schema (Fact + Dimensions)
- Built cube in SSAS, defined hierarchies (e.g., Category → Sub-Category), measures (Sales, Cost, Profit)
Analytical Queries:
- Used MDX for slicing/dicing metrics
- Created Power BI dashboards & Excel Pivot Tables to explore KPIs
Data Mining:
- Applied Random Forest and CNN to predict order returns

## Results: Best States for Freight Allocation
- Key Insight: Regions like California, New York, Texas showed highest return volumes.
- Recommended Action: Shift freight allocation to regions with lower return rates but strong demand, such as Arizona, Florida, Illinois.
Return Rate Analysis:
- Higher return rates often associated with products in Office Supplies > Art and long delivery times.
- Customers in Corporate Segment had higher average order values but also slightly higher return risk.

## 🛠️ Technologies Used
| Tool         | Purpose                                | Example |
|--------------|-----------------------------------------|---------|
| SSIS         | ETL: Extract, Transform, Load           | ETL pipeline from CSV to DW |
| SSAS         | Build OLAP Cube & define measures       | Sales cube by region        |
| Power BI     | Visualization & Dashboard               | Sales trend chart           |
| Python (RF)  | Predict return orders using ML          | RandomForestClassifier      |


## Report
A detailed report (in Vietnamese) describing the methodology, pipeline, visuals, and predictive models is available here:
[View Full Report (Google Drive)](https://drive.google.com/drive/folders/19do1f_oSnW5n3GEqgwAUZLF-eLEpb5J-?usp=sharing)
