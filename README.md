# Dreamcatcher-Project
My firs Power BI project
# 📊 Dreamcatcher USA — Power BI Analytics Project

This repository contains my full end‑to‑end Power BI project built using enterprise BI standards.  
It demonstrates my ability to work with data modeling, ETL, DAX, business analysis, and dashboard design — skills relevant for Data Analyst, BI Analyst, and Finance roles in the United States.

---

## 🔍 Project Overview

The goal of this project was to analyze U.S. retail performance across:

- Sales  
- Profit  
- Profit Margin  
- Customers  
- Products  
- Geography  
- Discounts  

I followed a complete BI workflow:

1. Business objectives definition  
2. Data import  
3. ETL in Power Query  
4. Star-schema data modeling  
5. DAX measures creation  
6. Multi-page dashboard design  
7. Validation & QA  
8. Corporate Microsoft design standards  

---

## 🗂 Data Model

The report uses a **star schema**:

### **Fact Table**
- Sales (Orders)

### **Dimension Tables**
- Products  
- Customers  
- Calendar  
- Geography  

This structure improves performance, simplifies DAX, and ensures clarity in business logic.

---

## 🔧 ETL Process (Power Query)

### **Extract**
Imported source files into Power Query.

### **Transform**
- Verified data types  
- Removed invalid rows  
- Standardized columns  
- Cleaned missing values  
- Created new columns (e.g., Discount Band)

### **Load**
Loaded clean tables into the Power BI model.

---

## 🧮 DAX Measures

### **Main KPIs**
```DAX
Total Sales = SUM('Sales'[Sales])
Total Profit = SUM('Sales'[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Sales])
Average Discount = AVERAGE('Sales'[Discount])
