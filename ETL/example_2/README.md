# Multi-Format ETL Pipeline (CSV, JSON, XML)

## Summary

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

### Data Acquisition

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

## Technology Stack

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

## ETL Workflow

### Extract

-   Detect file formats dynamically using `glob`
-   Parse:
    -   `.csv` via Pandas
    -   `.json` via Pandas
    -   `.xml` via xml parsing library
-   Load extracted data into Pandas DataFrames

### Transform

-   Standardize column names
-   Normalize data types
-   Handle missing values
-   Convert data into a consistent schema

### Load

-   Merge cleaned datasets
-   Export unified dataset
-   Log execution timestamp using `datetime`


------------------------------------------------------------------------

## Execution

``` bash
python extract_transform_load_code.py
```

