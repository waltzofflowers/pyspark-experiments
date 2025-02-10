# PySpark Experiments

This repository contains a collection of Jupyter Notebook files for personal experimentation and learning with PySpark.

## Contents

1. **spark-learning.ipynb**: This notebook serves as a reminder for PySpark concepts.
2. **spark-aggregation.ipynb**: This notebook contains practices for PySpark functions, focusing on aggregation.
3. **try.ipynb**: This notebook covers the data insertion part of the experiments.

## PySpark

PySpark is the Python API for Apache Spark. It allows you to write Spark applications using Python, which can interact seamlessly with both Python and Spark.

## Differences Between ODBC and JDBC Drivers

- **ODBC (Open Database Connectivity)**: A standard API for accessing database management systems (DBMS). It allows applications to communicate with any DBMS regardless of the DBMS platform or SQL dialect.
- **JDBC (Java Database Connectivity)**: A Java-based API specifically designed for connecting Java applications to a wide range of databases. It allows Java applications to interact with databases in a platform-independent manner.

## Usage

1. **spark-learning.ipynb**: Use this notebook to review and revise PySpark concepts.
2. **spark-aggregation.ipynb**: Experiment with various aggregation functions in PySpark.
3. **try.ipynb**: Understand and implement data insertion techniques using PySpark.

## Prerequisites

- Jupyter Notebook
- PySpark
- Python (with required libraries)

## Additional Setup Instructions

### Find Spark Absolute Path and Add .JAR File to PySpark Jar Folder

Since we want to use Spark, we need the JDBC (Java Database Connectivity) driver. 

In this case, we use MS-SQL, so the MS-SQL JDBC Driver is needed, which can be downloaded from Microsoft.

#### Microsoft SQL Server JDBC Driver

[Download Microsoft JDBC Driver for SQL Server](https://docs.microsoft.com/en-us/sql/connect/jdbc/download-microsoft-jdbc-driver-for-sql-server?view=sql-server-ver17)

Consider picking a version that matches the Java version installed on your machine. PySpark and Spark generally works well with Java 8 and Java 11. Since Java 11 was my choice, that version was used.

### Initialization with findspark

After finding its location where you use your pyspark and made your choice you need to put your .jar file into path that you find

```python
import findspark
findspark.init()
findspark.find()
```

## Data Download

This project uses the NYC Yellow Taxi trip data for January 2023.

You can download the data from the following link:

    [NYC Yellow Taxi Trip Data (PARQUET)](https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2023-01.parquet)

## Contributing

Feel free to copy and paste this into your README.md file. Let me know if you need any more adjustments or additional sections! 😊