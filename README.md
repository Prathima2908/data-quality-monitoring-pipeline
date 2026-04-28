# Data Quality Monitoring & Validation Framework

## Overview

This project implements a production-style data quality framework designed to validate, monitor, and improve the reliability of incoming data. It simulates real-world data engineering pipelines where raw data often contains inconsistencies, missing values, and invalid formats.

The framework applies rule-based validation, calculates data quality scores, and generates clean and rejected datasets along with analytical insights.

---

## Key Features

* Data ingestion and preprocessing
* Rule-based data validation engine
* Data quality scoring system
* Identification of invalid and inconsistent records
* Automated separation of clean and rejected data
* Data quality reporting and metrics
* Advanced visualizations for monitoring data health

---

## Dataset

A synthetic dataset was generated to simulate real-world enterprise data, including:

* Customer information (Age, Email, Phone)
* Financial data (Transaction Amount, Account Balance, Credit Score)
* Behavioral data (Login Attempts, Device, Activity Status)
* Temporal data (Signup Date, Transaction Date)

The dataset intentionally includes:

* Missing values
* Invalid formats (email, phone)
* Outliers and negative values
* Logical inconsistencies

---

## Validation Rules Implemented

* Age must be between 18 and 65
* Email must follow valid format
* Phone number must be 10 digits
* Transaction amount must be positive
* Credit score must be between 300 and 850
* Transaction date must be after signup date

---

## Data Quality Metrics

A **Data Quality Score** is computed for each record based on the number of validation failures.

* Score = 0 → Clean record
* Higher score → More data issues

---

## Visualizations

* Data Quality Score Distribution
* Data Issue Correlation Heatmap
* Data Quality Issue Breakdown
* Clean vs Rejected Data Ratio
* Data Quality Score by Country
* Time-based Data Quality Trends
* Top 10 Worst Records Visualization

---

## Output Files

* `raw_data_quality_data.csv` → Raw dataset
* `clean_data.csv` → Cleaned dataset
* `rejected_data.csv` → Invalid records
* `data_quality_summary.csv` → Summary report

---

## Tech Stack

* Python (Pandas, NumPy)
* Visualization (Matplotlib, Seaborn)
* Data Validation (Custom Rule Engine)
* Google Colab

---

## Business Impact

* Improves data reliability and accuracy
* Detects and isolates bad data early in the pipeline
* Enables better downstream analytics and decision-making
* Provides visibility into data quality issues

---

## How to Run

1. Open the notebook in Google Colab
2. Run all cells sequentially
3. Review outputs, visualizations, and generated files

---

## Future Enhancements

* Integrate with real-time data pipelines
* Implement automated alerting for data issues
* Use frameworks like Great Expectations for validation
* Deploy as a scheduled data quality monitoring job

---

## Author

Prathima Chinnabathini

---

## Conclusion

This project demonstrates how a structured data quality framework can be implemented to ensure data reliability in modern data engineering pipelines. It highlights the importance of validation, monitoring, and reporting in handling real-world data challenges.
