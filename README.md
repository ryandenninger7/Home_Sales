# Spark Home Sales Analysis Project

## Overview
This project utilizes Apache Spark to analyze home sales data. We perform several operations including data loading, querying, performance optimization through caching, and data storage in the Parquet format. The analysis aims to extract insights such as average home prices based on various criteria, demonstrating Spark's capability for handling big data processing tasks.

## Environment Setup
Apache Spark 3.5.1
Java OpenJDK 11
Python 3.7 or later
Py4J (for Python to JVM interaction)
Findspark (for initializing Spark in Python notebooks)

## Installation Steps
Install Java Development Kit (JDK) and set the JAVA_HOME environment variable.
Download and set up Apache Spark, configuring the SPARK_HOME environment variable.
Use pip to install Py4J and Findspark:
"pip install py4j findspark"

## Data
The dataset used is a CSV file containing home sales records, including fields like date sold, date built, price, number of bedrooms and bathrooms, square footage, and more.

## Key Operations
Data Loading: Load the CSV data into a Spark DataFrame and create a temporary view for SQL queries.
Data Analysis: Perform SQL queries to analyze the data, such as calculating the average price of homes based on various attributes.
Performance Optimization: Use caching to improve the performance of repeated queries.
Data Storage: Partition the data by the "date_built" field and store it in Parquet format for efficient access.
Caching Management: Manage the caching of data to optimize memory usage.

## Analysis Queries
Average price of four-bedroom homes sold per year.
Average price of homes built each year with specific features (e.g., 3 bedrooms, 3 bathrooms).
Analysis of home prices by view rating, with performance comparisons between cached and uncached data.

## Running the Project
Ensure Spark and Java are correctly set up and accessible from your Python environment. Execute the Python script or notebook that contains the Spark session setup, data loading, analysis queries, and caching management commands.

## Conclusion
This project demonstrates the powerful capabilities of Apache Spark for processing and analyzing large datasets, with a focus on real estate data. By leveraging Spark's in-memory computing and efficient data storage formats like Parquet, we can derive meaningful insights from the data at high speed.

