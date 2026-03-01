CSV to PostgreSQL Auto Loader

A Python-based data ingestion script that automatically reads all CSV files from a directory and loads each file into a separate PostgreSQL table.

This project demonstrates a simple but scalable raw data ingestion pattern commonly used in ETL and data engineering workflows.


Data Flow Diagram

<img width="820" height="636" alt="image" src="https://github.com/user-attachments/assets/05cf56ca-1e3f-4823-83ca-b4b1f7f09f6f" />

Overview

The script performs the following steps:

1. Scans a folder for .csv files
2. Cleans and converts each filename into a valid PostgreSQL table name
3. Infers column data types from the CSV
4. Creates a table (if it does not exist)
5. Bulk inserts the data into PostgreSQL

Each CSV file becomes its own table in the database
