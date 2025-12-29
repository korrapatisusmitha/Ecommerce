# 🛒 E-Commerce Data Pipeline using PySpark & Databricks

## 📌 Project Overview
This project demonstrates an **end-to-end batch data engineering pipeline** for an e-commerce use case using **Databricks, PySpark, Spark SQL, and Delta Lake**, following the **Medallion Architecture (Bronze–Silver–Gold)**.

The pipeline processes **3 months of CSV-based transactional data**, transforms it into analytics-ready datasets, and showcases how a **unified lakehouse platform** simplifies modern data engineering workflows.

---

## 🎯 Objective
This project solves challenges associated with **legacy data architectures**, such as:
- 💸 High service and infrastructure costs  
- 🔗 Scattered ETL logic across multiple tools  
- 🧩 Complex and non–beginner-friendly setups  
- 📉 Limited scalability and inefficient cloud usage  

### Why Databricks?
Databricks was chosen as it represents a **best-practice unified platform** widely adopted across the data industry:
- ⚡ Highly scalable and cloud-native  
- 🧠 Supports **Data Engineers, Analysts, and AI/ML Engineers** on the same platform  
- 🛠️ Handles **cluster lifecycle management**, allowing focus on **code and business logic**  
- 🧱 Provides powerful features like **Delta Lake**, **Time Travel**, **Unity Catalog**, and ACID transactions  

---

## 📊 Data Description
- **Source**: CSV files (synthetic e-commerce data)
- **Time Range**: 3 months (monthly data)
- **Tables**:
  - 🏷️ `brands`
  - 📂 `category`
  - 👤 `customers`
  - 📅 `date`
  - 🛒 `order_items`
  - 📦 `product`

---

## 🏗️ Architecture
The project follows the **Medallion Architecture** implemented using **Delta Lake**.


### 🥉 Bronze Layer (Raw)
- Raw CSV ingestion
- Minimal transformations
- Schema enforcement using Delta tables

### 🥈 Silver Layer (Cleansed & Transformed)
- Data cleaning and standardization
- Deduplication
- Joins across multiple tables
- Business-level transformations

### 🥇 Gold Layer (Analytics Ready)
- Aggregated datasets
- Business KPIs and metrics
- Optimized for analytics and reporting

---

## 🧰 Technologies Used
- 🚀 Databricks  
- 🐍 PySpark  
- 📜 Spark SQL  
- 💾 Delta Lake  
- 🏗️ Medallion Architecture  

---

## 🔄 Key Transformations & Logic
- 🔗 Joining fact and dimension tables  
- 🧹 Data cleansing and deduplication  
- 📊 Aggregations to generate:
  - Total revenue  
  - Order counts  
  - Product-level performance  

---

## 📈 Output & Use Cases
- 📊 Analytics-ready Gold tables  
- 👩‍💼 Can be consumed by:
  - Data Analysts (BI & reporting)
  - Business stakeholders
  - Downstream ML pipelines

---

## ▶️ How to Run the Project
- 📓 Notebook-based implementation in Databricks
- Upload CSV files to Databricks File System (DBFS)
- Run notebooks in sequence:
  1. Bronze ingestion
  2. Silver transformations
  3. Gold aggregations

---

## 🚀 Future Enhancements
- 🔄 Incremental data loading
- 🌊 Structured Streaming
- 📊 BI dashboard integration
- 🤖 Machine learning use cases

---

## 📚 What I Learned
- 🧱 Designing scalable pipelines using **Medallion Architecture**
- ⚡ Writing efficient **PySpark and Spark SQL** transformations
- 💾 Leveraging **Delta Lake** features such as ACID transactions and Time Travel
- ☁️ Understanding how Databricks abstracts infrastructure complexity
- 🏗️ Building projects aligned with **real-world data engineering best practices**

---

## 🧾 Conclusion
This project strengthened my understanding of **modern data engineering workflows** and demonstrated how Databricks enables teams to build **scalable, maintainable, and cost-effective lakehouse solutions**.

Using a unified platform allowed me to focus on **data modeling and business logic**, while Databricks handled infrastructure management, scalability, and performance optimization.

---

✨ *This project is designed as a portfolio-ready implementation aligned with real-world data engineering practices.*
