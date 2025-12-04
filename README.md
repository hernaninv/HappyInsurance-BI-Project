# 📘 Happy Insurance — Business Intelligence Project

A complete BI solution built using **Power BI**, **Power Pivot**, **Power Query**, and **DAX**, following the methodology taught in the Technion TCBDA27 Big Data Analysis Program.  
This project simulates a real-world BI workflow: from raw operational data → to semantic modeling → to analytical dashboards → to business insights.

---

## 🎯 Project Objective

The goal of this project is to transform raw operational data from a fictional insurance company (*Happy Insurance*) into actionable insights through:

- ETL (Power Query)
- Dimensional modeling (Power Pivot)
- Tabular modeling with DAX
- Interactive dashboards (Power BI)
- Business-driven storytelling

---

## 🗂 Repository Structure

Data/ → Source CSV/Excel files
PowerBI/ → PBIX file + images + model schema
DAX/ → DAX measures (AnalysisProject2.dax)
Presentation/ → Official slide deck (DataModeling.pptx)
README.md → Documentation

---

## 🧼 ETL Process (Power Query)

The ETL pipeline was implemented entirely in Power Query and includes:

- Full data cleansing (nulls, duplicates, incorrect types)
- Standardization of business fields
- Integration of **CSV + SQL Server** sources
- Logical corrections
- Construction of a complete **DimDate**
- Creation of clean dimensional tables (Star Schema–ready)

---

## ⭐ Dimensional Model — Star Schema

### 📐 Data Model

<img src="PowerBI/ModelSchema.png" width="600">

The tabular model includes:

### ▶ Fact Table  
**FactSales**  
(revenue, quantity, unit price, division, region, date)

### ▶ Dimension Tables  
- DimCustomer  
- DimDate  
- DimDivision  
- DimRegion  
- DimProduct  

### ▶ Additional Modeling Work  
- Correct one-to-many relationships  
- Calculated Columns (when required)  
- `DimTime` calculated table (where applicable)  
- Filtering propagation aligned with BI best practices  

---

## 🧮 DAX Measures

All DAX code was developed according to the project requirements.

Key functions used include:  
`CALCULATE()`, `FILTER()`, `SUMX()`, `RELATED()`, `ALL()`,  
`TOTALYTD()`, `TOTALQTD()`, `TOTALMTD()`, `SAMEPERIODLASTYEAR()`, `VAR`

📄 **Full DAX file:**  
`DAX/AnalysisProject2.dax`

---

## 📊 Power BI Dashboards

The dashboard suite implements all required Power BI functionalities:  

Charts, tables, maps, slicers, KPIs, custom color palette, drill-down, drill-through, custom tooltips, What-If parameters, and report-level filters.

### ⭐ Sample Screenshots (Representative Pages)

<img src="PowerBI/DashboardPreviews/Page1.png" width="600">

<img src="PowerBI/DashboardPreviews/Page2.png" width="600">

<img src="PowerBI/DashboardPreviews/Page3.png" width="600">

*(These three dashboards summarize the main analytical outputs of the report.  
Additional pages are included in the PBIX file.)*

---

## 🔑 Key Business Insights

Examples of insights derived from the model:

- **Life Insurance** is the company’s largest division.  
- **Health Insurance** is the fastest-growing division.  
- In Life Insurance, **APAC** has the highest revenue per unit sold.  
- In Health Insurance, **USA** is the dominant market.  
- Unit price for Life Insurance increased **34% from 2011 → 2012**.

These insights come directly from the semantic model and reflect the business logic of the dataset.

---

## 🎤 Project Presentation

The official slide deck (requirements, methodology, model diagrams, conclusions) is available at:

`Presentation/DataModeling.pptx`

---

## ✔ Conclusion

This repository demonstrates a full **end-to-end BI project**:

**data ingestion → transformation → modeling → DAX layer → visualization → business analysis**

It reflects industry-level best practices in:

- Data modeling  
- ETL (Power Query)  
- DAX development  
- Interactive report design  
- Analytical storytelling  

---

## 📧 Contact

For questions or collaboration, feel free to reach out via GitHub or LinkedIn.

