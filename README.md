# Vehicle Repairs Data Analysis

## 📌 Overview
This repository contains an Exploratory Data Analysis (EDA) of a **vehicle repairs dataset**. The dataset consists of **100 records and 52 columns**, capturing detailed information about vehicle repair transactions. The goal is to uncover trends, frequent issues, and potential improvements based on the data.

---

## 📂 Dataset Description

- **File Name**: `vehicle_repairs.csv`
- **Records**: 100  
- **Columns**: 52  

### 🔑 Key Columns
- `VIN`: Vehicle Identification Number  
- `TRANSACTION_ID`: Unique repair transaction ID  
- `CORRECTION_VERBATIM`: Description of the repair done  
- `CUSTOMER_VERBATIM`: Customer's issue description  
- `REPAIR_DATE`: Date of repair  
- `CAUSAL_PART_NM`: Part responsible for the issue  
- `GLOBAL_LABOR_CODE_DESCRIPTION`: Type of repair performed  
- `PLATFORM`: Vehicle platform (e.g., Full-Size Trucks, BEV)  
- `BODY_STYLE`: Body style (e.g., Crew Cab, 4 Door Utility)  
- `REPORTING_COST`, `TOTALCOST`, `LBRCOST`: Cost-related metrics  
- _...and many more_

---

## 📊 Analysis Highlights

### 🔍 Data Exploration
- Examined dataset shape, data types, and missing values  
- Generated descriptive statistics for numerical and categorical columns  
- Identified unique values and frequent patterns  

### 🧹 Data Cleaning
- Replaced missing categorical values with `"Unknown"`  
- Substituted corrupted characters with `"Corrupt Value"`  
- Filled missing `TOTALCOST` values using `REPORTING_COST` for consistency  

### 💡 Key Insights
- **Common Repairs**: Steering wheel-related issues were most frequent  
- **Platform Trends**: Full-Size Trucks had the highest repair count  
- **Cost Distribution**: Repair costs varied significantly; a few were high-cost outliers  
- **Geographical Patterns**: Most repairs occurred in the US, especially in CA and TX  

---
## 💾 Output Files

- `cleaned_steering_repair_data.csv`: Final cleaned version of the dataset after preprocessing  
- `generated_repair_tags.csv`: Extracted tags from `CORRECTION_VERBATIM` and `CUSTOMER_VERBATIM` columns for downstream use  

## 📁 Files

- `eda.ipynb`: Jupyter notebook containing all EDA steps—loading, cleaning, exploration, and visualization  
- `vehicle_repairs.csv`: The original dataset in csv format
- `cleaned_vehicle_repairs.csv`: Cleaned dataset with consistent and processed values  
- `generated_tags.csv`: Tags generated from free-text fields (correction/customer verbatim)  

---

## 🧠 Notes
This analysis can support further research on repair cost optimization, predictive maintenance, and customer experience improvements.

---
