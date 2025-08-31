# 🏞️ Flood Hazard Index Classification – Uttar Pradesh

## 📌 Project Overview

This project focuses on extracting, cleaning, and classifying flood hazard data for districts in Uttar Pradesh using the *Flood Hazard Atlas*. The goal is to transform raw flood metrics into a structured, interpretable dataset that supports vulnerability modeling and policy planning.

## 🎯 Problem Statement

Flood risk data in the Atlas is presented in fragmented PDF tables and lacks categorical interpretation. Without a clean, labeled dataset, it's difficult to assess regional vulnerability or integrate flood hazard into broader demographic analyses.

## ✅ Objectives

- Extract district-level flood data from PDF tables
- Calculate the **Flood Hazard Index (FHI)** using the formula: `H × A × F`
- Classify FHI values into five hazard categories based on official thresholds
- Create a clean, mentor-friendly dataset for further analysis

## 🧪 Methodology

1. **Data Extraction**: Used `tabula-py` and `pandas` to extract flood metrics from PDF tables
2. **Data Cleaning**: Handled duplicate columns, misaligned headers, and non-numeric values
3. **Index Calculation**: Computed FHI and ensured numeric integrity
4. **Categorization**: Applied classification logic from Table 15 to label hazard levels
5. **Export**: Saved the cleaned dataset for reproducibility and future merging

## 📊 Flood Hazard Categories

| FHI Range     | Category     |
|---------------|--------------|
| > 95          | Very High    |
| 46 to 95      | High         |
| 31 to 45      | Moderate     |
| 16 to 30      | Low          |
| ≤ 15          | Very Low     |

## 📁 Output

A cleaned CSV file with the following columns:
- `District`
- `Total_Flood_Area_Ha`
- `Inundated_Area_Ha`
- `Flood_Hazard_Pct`
- `Flood_Hazard_Index`
- `Flood_Hazard_Category`

## 🚀 Next Steps

- Merge with demographic and infrastructure data
- Model flood vulnerability across districts
- Visualize hazard distribution using charts or maps

## 👨‍💻 Author

**Sumit** – AI ML Intern at **Edunet Foundation**  
Focused on building reproducible, mentor-friendly data science workflows
**Sumit** – AI Intern at **Pinnacle Labs Pvt Ltd**  
Focused on building reproducible, mentor-friendly data science workflows
