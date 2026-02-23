# Exploratory Data Analysis (EDA)
## Brazilian E-Commerce – Orders Dataset

## Project Overview

This project presents an Exploratory Data Analysis (EDA) of the Brazilian E-Commerce (Olist) Orders dataset.  
The objective is to evaluate order trends and delivery performance using Python-based data analysis techniques.

The analysis focuses on understanding operational efficiency and identifying potential delays in order fulfillment.

---

## Dataset Used

- **File:** `olist_orders_dataset.csv`
- Contains order-level information including:
  - Order status
  - Purchase timestamps
  - Approval timestamps
  - Delivery timestamps
  - Estimated delivery dates

---

## Methodology

### 1. Data Inspection
- Checked dataset shape and structure  
- Evaluated missing values  

### 2. Data Preparation
- Converted timestamp columns to datetime format  
- Created a new feature: **delivery_time**
  - Calculated as the difference between purchase date and customer delivery date  

### 3. Analysis Performed
- Order status distribution analysis  
- Monthly order trend analysis  
- Statistical summary of delivery time  
- Delivery time distribution visualization  
- Outlier detection using the IQR method  

---

## Key Findings

- The majority of orders are successfully delivered.
- Order volume shows consistent growth over time.
- Average delivery time is approximately **12 days**.
- Delivery time distribution is right-skewed, indicating occasional delays.
- A small number of extreme delivery delays were identified using IQR-based outlier detection.

---

## Business Interpretation

Delivery time is a key operational performance metric.  
Analyzing delivery patterns and identifying extreme delays helps evaluate logistics efficiency and potential bottlenecks in the supply chain.

Understanding these patterns supports performance monitoring and service optimization.

---

## Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## Repository Structure

- `eda_brazilian_ecommerce.ipynb`  
- `olist_orders_dataset.csv`  
- `README.md`