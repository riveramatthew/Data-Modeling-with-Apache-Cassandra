# Data Modeling with Cassandra - Sparkify

## Project Overview

This project focuses on designing a **NoSQL database using Apache Cassandra** for Sparkify, a startup music streaming service. Sparkify wants to analyze user activity and song play data from their app. Currently, the data resides in CSV files, making it difficult to generate analytics.

As a data engineer, your role is to create a Cassandra database, design tables to support specific queries from the analytics team, and implement an **ETL pipeline in Python** to process and load the data.

The project applies concepts of **denormalization, query-based table design, and ETL pipelines** using Python and Cassandra.

---

## Datasets

You will be working with a dataset of user activity logs (`event_data`), partitioned by date. Examples of file paths:

event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv

These CSV files contain user activity events such as song plays, and are used to create a denormalized dataset for Cassandra.

---

## Project Template

A Jupyter Notebook template is provided to structure the project. The notebook includes:

1. Processing the `event_datafile_new.csv` dataset to create a **denormalized CSV file**.
2. Designing Cassandra tables to support analytics queries.
3. Loading data into Cassandra tables using Python.
4. Running **SELECT queries** to test the tables and ensure they return correct results.

---

## Project Steps

### 1. Data Modeling with Cassandra

- **Design tables** based on the queries provided in the template.
- Write **Cassandra `CREATE KEYSPACE`** and **`SET KEYSPACE`** statements.
- Develop **`CREATE TABLE` statements** for each query, including:
  - `IF NOT EXISTS` clause.
  - Optionally, `DROP TABLE` statements for testing purposes.
- Insert processed data using **`INSERT` statements**.
- Test your tables using **SELECT queries** with appropriate `WHERE` clauses.

### 2. ETL Pipeline

- Implement Python logic to:
  - Iterate through each CSV file in `event_data`.
  - Process and combine data into a **single denormalized CSV file**.
- Edit the ETL notebook to include:
  - Cassandra **CREATE TABLE** statements.
  - **INSERT statements** to load processed records.
- Test the pipeline by querying the database and verifying expected results.

---

## Technologies Used

- **Apache Cassandra** – NoSQL database for query-based modeling
- **Python** – ETL pipeline development
- **Jupyter Notebook** – Project development environment
- **CSV** – Source dataset format

---

## Project Deliverables

1. **Cassandra Keyspace and Table Definitions** – ready for production queries.
2. **ETL Pipeline** – Python scripts to process CSV files and load into Cassandra.
3. **Test Queries** – to validate table design and ETL process.
4. **Processed CSV Dataset** – denormalized data ready for ingestion.

---

## Getting Started

1. Clone the repository.
2. Launch the provided Jupyter Notebook.
3. Ensure Cassandra is installed and running on your local environment.
4. Follow the notebook steps:
   - Run the ETL pipeline.
   - Create keyspace and tables in Cassandra.
   - Insert data and validate with SELECT queries.

---

## References

- [Apache Cassandra Documentation](https://cassandra.apache.org/doc/latest/)
- [Sparkify Project Guidelines - Udacity](https://www.udacity.com/course/data-engineer-nanodegree--nd027)
