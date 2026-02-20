# 📦 Multi-Format ETL Pipeline (CSV, JSON, XML)

## 🚀 Project Overview

This project demonstrates the implementation of a structured ETL
(Extract, Transform, Load) pipeline capable of processing data from
multiple file formats including:

-   CSV
-   JSON
-   XML

The pipeline consolidates heterogeneous data sources into a unified
tabular format using Python and Pandas, simulating real-world data
engineering workflows.

------------------------------------------------------------------------

## 🏗️ Architecture Design

### 1️⃣ Data Acquisition

Download source files:

``` bash
wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0221EN-SkillsNetwork/labs/module%206/Lab%20-%20Extract%20Transform%20Load/data/source.zip
unzip source.zip
```

For extended practice:

``` bash
wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0221EN-SkillsNetwork/labs/module%206/Lab%20-%20Extract%20Transform%20Load/data/datasource.zip
```

------------------------------------------------------------------------

## 🛠️ Technology Stack

-   Python 3.11+
-   Pandas (data transformation)
-   XML parsing library
-   Glob (file discovery)
-   Datetime (logging timestamps)

Install required dependency:

``` bash
python3.11 -m pip install pandas
```

------------------------------------------------------------------------

## 🔄 ETL Workflow

### 🔹 Extract

-   Detect file formats dynamically using `glob`
-   Parse:
    -   `.csv` via Pandas
    -   `.json` via Pandas
    -   `.xml` via xml parsing library
-   Load extracted data into Pandas DataFrames

### 🔹 Transform

-   Standardize column names
-   Normalize data types
-   Handle missing values
-   Convert data into a consistent schema

### 🔹 Load

-   Merge cleaned datasets
-   Export unified dataset
-   Log execution timestamp using `datetime`

------------------------------------------------------------------------

## 📂 Project Structure

    ├── data/
    │   ├── csv_files/
    │   ├── json_files/
    │   ├── xml_files/
    ├── etl_script.py
    ├── logs.txt
    └── README.md

------------------------------------------------------------------------

## 📈 Engineering Capabilities Demonstrated

-   Multi-format data ingestion
-   Schema normalization
-   Modular ETL design
-   Logging and traceability
-   Automated file handling
-   Production-style scripting practices

------------------------------------------------------------------------

## 🎯 Real-World Applications

This ETL approach reflects real-world scenarios such as:

-   Enterprise data integration
-   Financial data consolidation
-   Business intelligence pipelines
-   Data lake ingestion preprocessing

------------------------------------------------------------------------

## 🚀 Execution

``` bash
python etl_script.py
```

------------------------------------------------------------------------

This project showcases practical data engineering skills aligned with
industry standards, emphasizing automation, reproducibility, and clean
data pipeline design.
