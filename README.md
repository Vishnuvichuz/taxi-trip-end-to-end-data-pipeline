# 🚕 Taxi Trip End-to-End Data Pipeline

An end-to-end **Big Data Engineering pipeline** designed to process and transform **112+ million taxi trip records** using **PySpark, Databricks, SQL, Apache Airflow, Docker, and Delta Lake**.

The project implements the **Medallion Architecture** to ingest, validate, clean, transform, and organize large-scale taxi trip data into structured Delta tables for efficient analysis.

---

## 📌 Project Overview

This project demonstrates how to build and orchestrate a scalable data pipeline for processing large volumes of taxi trip data.

The pipeline performs:

- Extraction and processing of **112+ million records**
- Data quality checks and validation
- Data cleaning and transformation using **PySpark**
- Storage of processed data in **Delta Tables**
- Data organization using **Medallion Architecture**
- SQL-based transformation and creation of category-specific tables
- Pipeline orchestration and scheduling using **Apache Airflow**
- Containerized execution using **Docker**

---

## 🏗️ Architecture

The project follows the **Medallion Architecture**:

```text
                Taxi Trip Dataset
                       │
                       ▼
              ┌─────────────────┐
              │   Bronze Layer  │
              │  Raw Data       │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │   Silver Layer  │
              │ Cleaned &       │
              │ Validated Data  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │    Gold Layer   │
              │ Business /      │
              │ Category Tables │
              └────────┬────────┘
                       │
                       ▼
                 Data Analysis
```

---

## 🔄 Data Pipeline Workflow

### 1. Data Extraction

The pipeline extracts a large-scale taxi trip dataset containing **112+ million records**.

### 2. Data Quality Checks

The raw data is analyzed to identify data quality issues such as:

- Missing values
- Invalid records
- Duplicate records
- Incorrect or inconsistent data
- Invalid data types

### 3. Data Cleaning

**PySpark** is used to clean and transform the dataset.

The cleaning process prepares the data for reliable downstream processing and analysis.

### 4. Delta Table Storage

The processed data is stored as **Delta Tables** in Databricks.

Delta Lake provides a reliable storage layer for the transformed datasets.

### 5. SQL Transformations

**SQL** is used to transform the processed dataset and create different category-based tables for analytical purposes.

### 6. Pipeline Orchestration

**Apache Airflow** is used to orchestrate the pipeline and schedule the execution of the data processing workflow.

### 7. Docker Environment

**Docker** is used to provide a consistent environment for running the Airflow-based orchestration workflow.

---

## 🥉 Medallion Architecture

### 🥉 Bronze Layer

Contains the raw taxi trip data after ingestion.

**Purpose:**
- Store raw data
- Preserve the original dataset
- Provide the initial layer for processing

### 🥈 Silver Layer

Contains cleaned and validated taxi trip data.

**Processing includes:**
- Data quality validation
- Missing-value handling
- Data cleaning
- Data type transformations
- Record-level validation

### 🥇 Gold Layer

Contains transformed and structured data designed for analytical use.

SQL transformations are used to create different category-based tables from the processed dataset.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Python** | Pipeline development and data processing |
| **PySpark** | Distributed processing of large-scale data |
| **Databricks** | Data engineering and Spark execution environment |
| **SQL** | Data transformation and analytical tables |
| **Delta Lake** | Reliable storage of processed data |
| **Apache Airflow** | Pipeline orchestration and scheduling |
| **Docker** | Containerized execution environment |

---

## 📊 Dataset

The project uses a large-scale **Taxi Trip Dataset** containing:

- **112+ million records**
- Taxi trip-related information
- Multiple attributes suitable for data quality validation and analytical transformations

The large dataset is used to demonstrate **distributed data processing and Big Data engineering concepts**.

---

## 🚀 Key Features

- ⚡ Processes **112+ million records**
- 🔍 Performs data quality checks
- 🧹 Cleans and transforms large-scale datasets
- 🏗️ Implements **Medallion Architecture**
- 🔥 Uses **PySpark** for distributed data processing
- 🗄️ Stores processed data in **Delta Tables**
- 📊 Creates analytical tables using **SQL**
- ⏱️ Automates pipeline execution with **Apache Airflow**
- 🐳 Uses **Docker** for containerized orchestration
- ☁️ Uses **Databricks** as the data processing platform

---

## ⚙️ How to Run

### Prerequisites

Make sure you have:

- Python
- Databricks account/workspace
- Apache Airflow
- Docker
- SQL knowledge
- PySpark environment

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
cd Taxi-Trip-End-to-End-Data-Pipeline
```

### Step 2: Configure Databricks

Configure your Databricks environment and provide the required dataset and connection details.

### Step 3: Start Docker

Start the Docker environment used for the Airflow orchestration setup.

```bash
docker compose up
```

### Step 4: Configure Airflow

Place the pipeline DAG files in the Airflow `dags` directory and configure the required connections.

### Step 5: Run the Pipeline

Trigger the Airflow DAG to execute the pipeline.

```text
Airflow
   ↓
Extract Data
   ↓
Data Quality Checks
   ↓
PySpark Processing
   ↓
Bronze
   ↓
Silver
   ↓
Gold
   ↓
SQL Transformations
   ↓
Analytical Tables
```

---

## 🎯 Learning Outcomes

This project helped demonstrate practical experience with:

- Big Data processing
- Distributed data processing with PySpark
- Databricks
- Delta Lake
- Medallion Architecture
- Data quality and validation
- SQL transformations
- Workflow orchestration
- Apache Airflow
- Docker
- End-to-end data pipeline development

---

## 🔮 Future Improvements

- Add automated data quality testing
- Implement pipeline monitoring and alerting
- Add incremental data processing
- Implement partitioning and optimization strategies
- Add automated testing for pipeline components
- Integrate visualization tools for analytical dashboards

---

## 👨‍💻 Author

**Vishnu Prasad**

B.Tech Computer Science Engineering Graduate

**Focus Areas:** Data Engineering | Big Data | Cloud | Data Pipelines

---

## ⭐ Project Highlights

> **112+ Million Records | PySpark | Databricks | Delta Lake | SQL | Apache Airflow | Docker | Medallion Architecture**
