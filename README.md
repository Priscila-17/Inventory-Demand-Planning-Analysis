🇺🇸 English | 🇧🇷 [Versão em Português](README_pt-BR.md)

# Supply Chain Analysis — Inventory Demand Planning Evaluation

## Overview

This project presents an Exploratory Data Analysis (EDA) of an inventory demand planning dataset, with the objective of evaluating the consistency, behavior, and operational patterns of the replenishment process.

Dataset used:  
https://www.kaggle.com/datasets/veeralakrishna/inventory

---

## Objectives

The analysis was structured to answer the following questions:

* Is the planning consistent with lead time requirements?  
* Is demand stable or variable? How stable or variable is it?  
* Is it possible to identify critical components?  
* Do different production strategies behave differently?  
* Are there trends or patterns over time?  

---

## Tools Used

* Python (Pandas, Matplotlib) for data analysis and visualization  
* SQL (DuckDB) for querying and aggregation  
* Jupyter Notebook as the development environment  
* Power BI for visualization of results  

---

## Available Files

- Complete Notebook (.ipynb): Full analysis, including data processing, visualizations, and insights  
- Dashboard (.pbix): Developed to visualize key indicators and identified patterns  

![Dashboard Preview](Inventory Demand Planning Analysis Dashboard.png)  
![Dashboard Preview](Inventory Demand Planning Analysis Graph.png)

---

## Data Processing

During the processing stage, the following steps were performed:

* Date standardization  
* Organization of planning vs demand relationship  
* Creation of an operational classification:

  * On Schedule → meets lead time requirements  
  * Delayed → planned before demand but with insufficient time  
  * Emergency → planned after demand  
  * Undefined → inconsistent data (not observed in this dataset)  

---

## Key Insights

* Planning consistency    
  * Approximately 94% of demands are classified as On Schedule  
   Indicates strong alignment with lead time and good operational organization  

* Operational behavior  
  * Data suggests a routine and recurring process  
  * Evidence of cyclic operation (possibly weekly or batch-based)  

* High presence of zero-quantity records  
  * Evidence suggests they are part of operational routines, not actual demand  

* Demand variability  
  * Some components show recurring high peaks  
  * Indicates the existence of critical items or specific demand events  
