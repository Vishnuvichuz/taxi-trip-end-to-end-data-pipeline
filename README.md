# 🚕 Taxi Trip End-to-End Data Pipeline

An end-to-end **Big Data Engineering pipeline** designed to process **112+ million taxi trip records** using **PySpark, Databricks, SQL, and Delta Lake**.

The project focuses on data quality checking, cleaning, transformation, and storage of large-scale taxi trip data using **PySpark** and the **Medallion Architecture**.

---

## 📌 Project Overview

This project demonstrates how to process and transform a large-scale taxi trip dataset using distributed data processing technologies.

The pipeline performs:

- Processing of **112+ million taxi trip records**
- Data quality checking using **PySpark**
- Data cleaning and transformation
- Loading processed data into **Delta Tables**
- Implementation of **Medallion Architecture**
- SQL-based transformation and creation of category-based tables
- Large-scale data processing using **Databricks**

---

## 🏗️ Architecture

The project follows the **Medallion Architecture**:

```text
                  Taxi Trip Dataset
                         │
                         ▼
                ┌─────────────────┐
                │  Bronze Layer   │
                │    Raw Data     │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │  Silver Layer   │
                │ Quality Check   │
                │ Cleaned Data    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │   Gold Layer    │
                │ Transformed &   │
                │ Category Tables │
                └────────┬────────┘
                         │
                         ▼
                   Data Analysis
```

---

## 🔄 Data Pipeline Workflow

### 1. Data Ingestion

The project uses a large-scale taxi trip dataset containing **112+ million records**.

The dataset is loaded into the Databricks environment for processing.

### 2. Data Quality Checking

**PySpark** is used to check the quality of the dataset before performing further transformations.

The data is examined for issues such as:

- Missing values
- Duplicate records
- Invalid records
- Incorrect data types
- Inconsistent data

### 3. Data Cleaning

PySpark is used to clean the dataset and handle identified data quality issues.

The cleaned dataset is prepared for downstream processing and analysis.

### 4. Delta Table Loading

After cleaning and transformation, the processed data is loaded into **Delta Tables**.

```text
Raw Dataset
     ↓
PySpark Quality Check
     ↓
Data Cleaning
     ↓
Transformation
     ↓
Delta Table
```

### 5. SQL Transformation

**SQL** is used to query the processed Delta data and create different category-based tables for analytical purposes.

### 6. Databricks Processing

**Databricks** is used as the data processing environment for executing PySpark and SQL workloads.

---

## 🥉 Medallion Architecture

### 🥉 Bronze Layer

Contains the raw taxi trip dataset.

**Purpose:**

- Store raw data
- Preserve the original dataset
- Provide the initial layer for processing

### 🥈 Silver Layer

Contains cleaned and validated taxi trip data.

**Processing includes:**

- Data quality checking
- Missing-value handling
- Duplicate handling
- Data cleaning
- Data type transformations

### 🥇 Gold Layer

Contains transformed and structured data for analytical use.

SQL transformations are used to create different category-based tables from the processed dataset.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **PySpark** | Data quality checking, cleaning, and transformation |
| **Databricks** | Data processing and execution environment |
| **SQL** | Data transformation and analytical tables |
| **Delta Lake** | Storage of processed data |

---

## 📊 Dataset

The project uses a large-scale **Taxi Trip Dataset** containing:

- **112+ million records**
- Taxi trip-related information
- Multiple attributes for data quality checking and analysis

The large dataset demonstrates the use of distributed processing for **Big Data Engineering** workloads.

---

## 🚀 Key Features

- ⚡ Processes **112+ million taxi trip records**
- 🔍 Performs data quality checks using PySpark
- 🧹 Cleans and transforms large-scale datasets
- ⚡ Uses PySpark for distributed data processing
- 🏗️ Implements **Medallion Architecture**
- 🗄️ Stores processed data in **Delta Tables**
- 📊 Uses SQL for analytical transformations
- ☁️ Uses Databricks for scalable data processing

---

## 🔁 Pipeline Flow

```text
┌──────────────────────┐
│  Taxi Trip Dataset   │
│   112+ Million Rows  │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   Bronze Layer       │
│      Raw Data        │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ PySpark Data Quality │
│       Checks         │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   Data Cleaning &    │
│   Transformation     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   Silver Layer       │
│   Cleaned Data       │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Gold Layer        │
│ Category-Based Tables│
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Delta Tables      │
└──────────────────────┘
           │
           ▼
      SQL Analysis
```

---

## 📁 Project Structure

```text
Taxi-Trip-End-to-End-Data-Pipeline/
│
├── databricks/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── sql/
│   └── transformations/
│
├── README.md
└── requirements.txt
```

> Update the folder structure according to your actual GitHub repository.

---

## ⚙️ How to Run

### Prerequisites

Make sure you have:

- Databricks account/workspace
- PySpark
- SQL
- Python

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Taxi-Trip-End-to-End-Data-Pipeline
```

### 2. Configure Databricks

Upload or connect the taxi trip dataset to your Databricks environment.

### 3. Run PySpark Processing

Execute the PySpark workflow to:

```text
Load Dataset
     ↓
Check Data Quality
     ↓
Clean Data
     ↓
Transform Data
     ↓
Load into Delta Table
```

### 4. Run SQL Transformations

Execute the SQL queries to create the required category-based tables from the processed Delta data.

---

## 🎯 Learning Outcomes

This project provided practical experience with:

- Big Data processing
- Processing **112+ million records**
- PySpark
- Databricks
- Delta Lake
- Medallion Architecture
- Data quality checking
- Data cleaning
- SQL transformations
- Large-scale data processing
- End-to-end data pipeline development

---

## 🔮 Future Improvements

- Implement incremental data processing
- Add automated data quality testing
- Optimize Delta Tables using partitioning
- Implement Delta Lake optimization techniques
- Add data visualization dashboards
- Add pipeline monitoring

---

## 👨‍💻 Author

**Vishnu Prasad**

B.Tech Computer Science Engineering Graduate

**Focus Areas:** Data Engineering | Big Data | Cloud | Data Pipelines

---

## ⭐ Project Highlights

> **112+ Million Records | PySpark | Databricks | SQL | Delta Lake | Medallion Architecture**
