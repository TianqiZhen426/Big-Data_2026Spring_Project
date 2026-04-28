# Airline Delay Analysis

## Overview

This project focuses on analyzing large-scale U.S. domestic airline on-time performance data using Big Data technologies. The goal is to identify meaningful patterns in flight delays, compare airline operational performance, evaluate airport congestion, analyze seasonal and hourly delay trends, and explore the main causes of delays.

The project uses **Apache Spark / PySpark**, **Spark SQL**, and **Python data visualization tools** to process and analyze millions of airline records efficiently.

This repository contains the complete data pipeline including:

- Raw data ingestion
- Data cleaning and preprocessing
- Feature engineering
- SQL-based analytics
- Visualization
- Exploratory predictive modeling

---

# Project Objectives

The main objectives of this project are:

1. Analyze large-scale flight delay patterns across the United States.
2. Compare delay performance among major airlines.
3. Identify airports with high traffic congestion and delay rates.
4. Study delay trends by month, season, weekday, and departure hour.
5. Investigate the primary causes of delays.
6. Build a basic predictive model for flight delays.

---

# Dataset Information

## Primary Data Source

U.S. Bureau of Transportation Statistics (BTS)

**Dataset Name:**  
On-Time Reporting Carrier On-Time Performance (1987–Present)

**Official Link:**  
https://www.transtats.bts.gov/

## Data Used in This Project

This project uses **2024 monthly airline performance data**, combined into one large dataset.

### Approximate Size

- **Rows:** 7,000,000+ flight records
- **Columns:** 110 original columns
- **Working dataset after cleaning:** selected core columns for analysis

### Key Columns Used
#### Time Features
Year
Quarter
Month
DayofMonth
DayOfWeek
FlightDate
CRSDepTime
CRSArrTime
#### Airline Features
Reporting_Airline
DOT_ID_Reporting_Airline
#### Airport Features
Origin
OriginCityName
Dest
DestCityName
#### Delay Features
DepDelayMinutes
ArrDelayMinutes
CarrierDelay
WeatherDelay
NASDelay
SecurityDelay
LateAircraftDelay
#### Flight Status
Cancelled
Diverted

---

# Technologies Used
## Big Data Tools
Apache Spark
PySpark
Spark SQL
## Programming Language
Python 3
## Libraries
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
## Development Platform
Google Colab
Jupyter Notebook

---

# Repository Structure

```text
Big-Data-Airline-Project/
│
├── data/
│   ├── raw_data/
│   ├── cleaned_data/
│   └── parquet/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_sql_analysis.ipynb
│   ├── 03_visualization.ipynb
│   └── 04_prediction_model.ipynb
│
├── scripts/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   └── helper_functions.py
│
├── outputs/
│   ├── figures/
│   ├── tables/
│   └── reports/
│
└── README.md
