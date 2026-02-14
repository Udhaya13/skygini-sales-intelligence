# SkyGeni – Sales Intelligence Challenge

## Overview
This repository contains my solution to the **SkyGeni Sales Intelligence Challenge** for the **Data Science / Applied AI Engineer** role.

The goal of this assignment is to investigate a decline in sales win rate despite healthy pipeline volume and to demonstrate how data-driven insights can help sales leaders take better decisions.

This project focuses on **business reasoning, clarity of insights, and decision intelligence**, not complex machine learning.

---

## Business Problem
A B2B SaaS company observes:
- Declining win rates over the last two quarters
- Healthy pipeline volume
- Lack of clarity on what is going wrong and what actions to take

The objective is to analyze sales deal data and surface insights that explain:
- Why deals are being lost
- Where risks exist in the pipeline
- What actions sales leadership should focus on

---

## Dataset
The dataset contains historical sales deal information with fields such as:
- deal_id
- created_date
- closed_date
- deal_stage
- deal_amount (ACV)
- sales_rep_id
- industry
- region
- product_type
- lead_source
- outcome (won / lost)

---

## Repository Structure
skygini-sales-intelligence/
│
├── data/
│ ├── skygini_sales_data.csv
│ └── processed/
│ └── cleaned_sales_data.csv
│
├── analysis/
│ └── eda.ipynb
│
└── README.md


---

## Analysis Approach
The analysis focuses on:
1. Understanding the structure and quality of the sales data
2. Identifying missing or inconsistent information
3. Performing basic data cleaning
4. Preparing a clean dataset for downstream decision analysis

The notebook intentionally keeps the analysis simple and interpretable, prioritizing business understanding over model complexity.

---

## Tools Used
- Python
- pandas
- numpy
- matplotlib
- Jupyter Notebook / Google Colab

---

## How to Run
1. Clone the repository:
git clone https://github.com/Udhaya13/skygini-sales-intelligence.git


2. Open the notebook:
analysis/eda.ipynb


3. Ensure the folder structure is unchanged so relative paths work correctly.

---

## Notes
- The notebook uses **relative paths**, making it portable across environments.
- The cleaned dataset is saved to `data/processed/cleaned_sales_data.csv`.
- The focus of this submission is on **clear thinking, clean structure, and business relevance**.

---



## Reflection

### Weakest Assumptions
The weakest assumption in this solution is that the provided sales data is complete, consistently recorded, and representative of real sales behavior. In real organizations, deal stages, outcomes, and timestamps are often inconsistently updated by sales teams, which can bias analysis and conclusions.

### Production Risks
In a real-world production environment, this approach could break due to:
- Missing or delayed data updates from CRM systems
- Changes in sales processes or deal stage definitions over time
- Data quality issues such as duplicate deals or incorrect close dates

Without strong data validation and monitoring, insights could become misleading.

### What I Would Build Next (1 Month Roadmap)
Given one additional month, I would:
- Build a win-rate driver analysis using interpretable models (e.g., logistic regression or tree-based models)
- Add deal risk scoring for open opportunities
- Create automated alerts for sudden drops in win rate by segment (region, product, rep)
- Implement data quality checks and anomaly detection on incoming CRM data

### Least Confident Area
The area I am least confident about is the causal interpretation of observed patterns. While EDA can surface correlations, determining true drivers of deal success or failure would require controlled experimentation, deeper behavioral data, and collaboration with sales stakeholders.

---

## Author
Udhaya R.
