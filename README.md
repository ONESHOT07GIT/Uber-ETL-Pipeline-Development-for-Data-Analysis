# Uber-ETL-Pipeline-Development-for-Data-Analysis

This project demonstrates a modern data engineering pipeline using **Python**, **Mage**, and **Google Cloud Platform (GCP)**. The goal is to process, transform, and analyze **Uber-like datasets** with dimensional modeling to create a scalable data architecture.

---

## Architecture Overview

### **Pipeline Steps**
1. **Data Storage**: Raw data is stored on Google Cloud Storage.
2. **Data Transformation**: Python scripts deployed via Mage for data modeling and transformations.
3. **Data Warehouse**: Processed data is loaded into Google BigQuery.
4. **Visualization**: Dashboards created using Looker Studio (formerly Data Studio).

### **Technology Stack**
- **Mage**: Open-source data pipeline tool for orchestrating transformations.
- **Google Cloud Platform Services**:
  - Google Cloud Storage
  - Compute Engine
  - BigQuery
- **Python**: For data transformations.
- **Looker Studio**: For dashboards and analytics.

---

## Dataset

### **Source**
- **TLC Trip Record Data**: Contains fields like:
  - Pickup/drop-off dates and times.
  - Trip distances.
  - Fares and payment types.
  - Passenger counts.

- **Official Dataset**: [NYC TLC Trip Records](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- **Data Dictionary**: [TLC Data Dictionary (PDF)](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf)

---

## Project Steps

### 1. **Data Modeling**
- Data transformed into **Fact** and **Dimension** tables:
  - **Fact Table**: Contains metrics like `fare_amount`, `trip_distance`, etc.
  - **Dimension Tables**: Includes descriptive attributes like `payment_type`, `pickup_location`, etc.

### 2. **Pipeline Implementation**
- **Mage Integration**:
  - Data loader, transformation, and exporter blocks configured.
  - Transformation logic written in Python.
- **Data Upload**:
  - Processed data loaded to BigQuery via Mage.

### 3. **Querying and Analytics**
- SQL queries on BigQuery:
  - Average fare amounts by vendor.
  - Insights on passenger behavior based on payment types.

### 4. **Visualization**
- Looker Studio dashboards created to visualize metrics:
  - Total trips.
  - Hourly trends.
  - Payment preferences.

---

## Setup Instructions

### **Prerequisites**
1. **Basic Knowledge**:
   - Python, SQL, and Jupyter Notebook.
2. **Required Tools**:
   - Google Cloud Account with $300 free credits.
   - Installed Mage instance.

### **Steps**
1. **Clone Repository**:
   ```bash
   git clone <repository-url>
