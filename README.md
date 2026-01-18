## ✅ Day 1 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

I’ve successfully completed **Day 1** of the Databricks AI Challenge, and it was an exciting introduction to the **Databricks Lakehouse ecosystem**.

---

## 📘 What I Learned

- Why **Databricks** over traditional **Pandas / Hadoop**
- Fundamentals of **Lakehouse architecture**
- Overview of the **Databricks workspace structure**
- Real-world industry use cases:
  - Netflix  
  - Shell  
  - Comcast  

---



## ✅ Day 2 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

I’ve successfully completed **Day 2** of the Databricks AI Challenge, focusing on core **Apache Spark fundamentals**.

---

## 📘 Key Concepts Learned

### 🔹 Spark Architecture (Driver, Executors, DAG)

- **Driver** manages the Spark application lifecycle, builds the logical execution plan (**DAG**), schedules stages and tasks, and tracks execution progress.
- **Executors** are worker processes that execute tasks, perform computations, and cache data in memory for faster processing.
- The **DAG (Directed Acyclic Graph)** represents the sequence of transformations and is converted into a physical execution plan when an action is triggered.

### 🔹 DataFrames vs RDDs

- **RDDs** are low-level, immutable distributed collections offering fine-grained control but no automatic query optimization.
- **DataFrames** are high-level, schema-based abstractions with a SQL-like API and built-in optimizations via **Catalyst** and **Tungsten**, making them faster and easier for structured data.

### 🔹 Lazy Evaluation in Spark

- Transformations are recorded in a DAG but executed only when an action (e.g., `count`, `show`, `collect`) is called.
- This allows Spark to optimize the full pipeline, reducing shuffles and improving overall performance.

### 🔹 Databricks Notebook Magic Commands (`%sql`, `%python`, `%fs`)

- Enable seamless language switching and file system access within a single notebook, boosting productivity and workflow efficiency.


---

Grateful for the initiative and support from **Databricks**, **Codebasics**, and **Indian Data Club** 🙏

---

## ✅ Day 3 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

Successfully completed **Day 3**, focusing on a deep dive into **PySpark transformations** and how they compare to traditional data processing approaches.

---

## 📘 Key Concepts Learned

### 🔹 PySpark vs Pandas

- **PySpark** enables distributed, parallel processing for large-scale datasets.
- **Pandas** is optimized for in-memory, single-machine analysis.

### 🔹 Joins in PySpark

- Implemented **inner**, **left**, **right**, and **outer joins** to combine large datasets efficiently in a distributed environment.

### 🔹 Window Functions

- Used window functions for **running totals**, **rankings**, and **partition-based calculations** without collapsing data granularity.

### 🔹 User-Defined Functions (UDFs)

- Created **UDFs** to apply custom business logic when built-in Spark functions were insufficient.



---

## ✅ Day 4 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

Completed **Day 4**, focusing on an introduction to **Delta Lake** and how it brings **reliability and governance** to modern data lakes.

---

### 🔹 What is Delta Lake?
Delta Lake is an **open-source storage layer** that sits on top of data lakes (typically storing data in **Parquet** files) and adds reliability features such as **ACID transactions, schema enforcement, and time travel**.  
It helps transform a *raw data lake* into a **production-ready, database-like analytics platform** for both batch and streaming workloads.

---

### 🔹 ACID Transactions
Delta Lake provides **ACID guarantees** (Atomicity, Consistency, Isolation, Durability) for data operations, preventing **partial writes, inconsistent reads, and table corruption**, especially during concurrent writes.

---

### 🔹 Schema Enforcement
Delta Lake enforces schemas at write time by validating incoming data against a predefined structure, **rejecting invalid or mismatched data** early to keep pipelines stable.

---

### 🔹 Delta Lake vs Parquet
**Parquet** is an efficient columnar storage format.  
**Delta Lake** builds on Parquet by adding a **transaction log and table semantics**, enabling **updates, deletes, time travel, ACID transactions, and higher data reliability**.

--- 

## ✅ Day 5 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

Completed **Day 5**, diving into **advanced Delta Lake concepts** that are critical for building reliable, high-performance data pipelines.

---

### 📘 Key Concepts Learned

#### 🔹 Time Travel (Version History)
Enables querying **previous versions** of Delta tables, supporting **experiment reproducibility, data debugging, and safe rollbacks** after faulty updates.

---

#### 🔹 MERGE Operations (Upserts)
Allows **atomic updates and inserts** in a single operation, making it ideal for **incremental data ingestion** and maintaining clean, consistent feature tables.

---

#### 🔹 OPTIMIZE & ZORDER
- **OPTIMIZE** compacts many small files into larger ones to improve query performance.  
- **ZORDER** colocates related data on disk, significantly speeding up queries that filter on key columns.

---

#### 🔹 VACUUM (Cleanup)
Removes obsolete files that are no longer required, helping **control storage costs** while keeping Delta tables clean and efficient.

---

## ✅ Day 6 Completed – Databricks 14 Days AI Challenge
Sponsored by Databricks

Completed Day 6, focusing on the Medallion Architecture and how it enables scalable, reliable, and maintainable data pipelines in modern data platforms.

📘 Key Concepts Learned

🔹 Medallion Architecture (Bronze → Silver → Gold)
A layered data design where:

Bronze stores raw, immutable ingested data

Silver applies cleaning, enrichment, and deduplication

Gold contains business-ready, aggregated data optimized for analytics

🔹 Best Practices for Each Layer

Bronze: Append-only ingestion with minimal transformations

Silver: Data quality checks, schema enforcement, and deduplication

Gold: Optimized for BI, reporting, and analytics use cases

🔹 Incremental Processing Patterns
Processes only new or changed data, improving performance and reducing costs. Techniques like MERGE operations and watermarks enable reliable, scalable pipelines.

---

## ✅ Day 7 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

Completed **Day 7**, focusing on **Workflows & Job Orchestration in Databricks** and how they help build **reliable, automated data pipelines**.

---

## 📘 Key Concepts Learned

### 🔹 Databricks Jobs vs Notebooks

- **Notebooks**
  - Interactive environments
  - Used for development, experimentation, data exploration, and debugging

- **Jobs**
  - Production-ready executions of notebooks or scripts
  - Designed to run automatically using schedules or event triggers

---

### 🔹 Multi-task Workflows

- A **workflow** is a pipeline composed of multiple dependent tasks
- Allows complex data pipelines to be:
  - Broken into smaller steps
  - More manageable
  - Reusable and modular

---

### 🔹 Parameters & Scheduling

- **Parameters**
  - Allow the same notebook or job to run with different inputs  
    (e.g., dates, file paths, model versions)

- **Scheduling**
  - Enables automatic execution at fixed intervals:
    - Hourly
    - Daily
    - Weekly

---

### 🔹 Error Handling

- Detects and logs job or workflow failures
- Prevents silent failures
- Improves overall pipeline reliability

## ✅ Day 8 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

Completed **Day 8**, focusing on **Unity Catalog Governance** and how it enables **secure, centralized data governance** across the Databricks Lakehouse.

---

## 📘 Key Concepts Learned

### 🔹 Catalog → Schema → Table Hierarchy

- Unity Catalog organizes data using a **three-level structure**:
  - **Catalog** – Top-level container
  - **Schema** – Database
  - **Table** – Actual data storage

---

### 🔹 Access Control (GRANT / REVOKE)

- Defines **who can read or modify data**
- Uses fine-grained permissions such as:
  - `SELECT`
  - `MODIFY`
- **Example**: Granting analysts read access to a sales table

---

### 🔹 Data Lineage

- Tracks how data flows across:
  - Tables
  - Views
  - Jobs
- Helps understand:
  - Data origins
  - Downstream impact of changes

---

### 🔹 Managed vs External Tables

- **Managed Tables**
  - Fully controlled by Databricks
  - Data lifecycle managed automatically

- **External Tables**
  - Data stored in external storage (e.g., S3, ADLS)
  - Databricks manages metadata only
## ✅ Day 9 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

Completed **Day 9**, focusing on **SQL Analytics & Dashboards** and how **SQL Warehouses** power fast, interactive analytics in Databricks.

---

## 📘 Key Concepts Learned

### 🔹 SQL Warehouses

- Enable scalable, high-performance execution of SQL queries
- Optimized for:
  - BI workloads
  - Analytical queries
  - Interactive reporting

---

### 🔹 Complex Analytical Queries

- Wrote advanced SQL using:
  - Joins
  - Window functions
  - Aggregations
  - Common Table Expressions (CTEs)
- Used to derive meaningful **business insights**

---

### 🔹 Dashboard Creation

- Built interactive dashboards to analyze:
  - Revenue trends
  - Conversion funnels
  - Top-performing products

---

### 🔹 Visualizations & Filters

- Used:
  - Charts
  - Filters
  - Scheduled refreshes
- Enabled dynamic, self-service analytics for stakeholders

## ✅ Day 10 Completed – Databricks 14 Days AI Challenge  
**Sponsored by Databricks**

Completed **Day 10**, focusing on **performance optimization techniques** to improve **query efficiency and scalability** in Databricks.

---

## 📘 Key Concepts Learned

### 🔹 Query Execution Plans

- Learned how Spark SQL converts queries into:
  - Logical plans
  - Physical plans
- Helps identify performance bottlenecks such as:
  - Costly joins
  - Data shuffles
  - Full table scans

---

### 🔹 Partitioning Strategies

- Applied partitioning on large tables to:
  - Reduce scanned data
  - Improve query performance
- Ensures only **relevant partitions** are read during query execution

---

### 🔹 OPTIMIZE & ZORDER

- **OPTIMIZE**
  - Compacts many small files into fewer large files
  - Reduces file scan overhead

- **ZORDER**
  - Colocates related data on disk
  - Significantly speeds up filtered queries

---

### 🔹 Caching Techniques

- Cached frequently accessed tables
- Benefits:
  - Reduces recomputation
  - Improves performance for iterative and repeated workloads


### 🔖 Hashtags
`#Databricks` `#AIChallenge` `#ApacheSpark` `#PySpark` `#BigData` `#DataEngineering` `#DatabricksWithIDC`



