

# **Brazilian E-commerce Data Engineering Pipeline**

This repository showcases a complete, production-style **PySpark-based data engineering pipeline** built on the **Olist Brazilian E-commerce Public Dataset**.
The project mirrors real-world enterprise workflows — covering ingestion, cleaning, transformation, integration, optimization, and data serving — demonstrating both data engineering fundamentals and scalable Spark practices.

---

## 🔗 **Dataset**

**Dataset:** Brazilian E-commerce Public Dataset by Olist
**Source:** Kaggle
**Link:** [https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

The dataset includes real commercial transactions from Olist, a major Brazilian e-commerce marketplace, spanning customers, sellers, orders, payments, reviews, and delivery performance.

---

## 💻 **Technology Stack**

* **PySpark** — Distributed compute engine
* **Python** — Core programming language
* **Jupyter Notebook** — Development and experimentation
* **File Formats:** Parquet, CSV, Hive-compatible tables
* **Performance Techniques:** Caching, bucketing, partitioning, broadcast joins, skew handling

---

## 📂 **Project Structure (Modules)**

The pipeline is divided into five structured modules, each representing a stage of the data engineering lifecycle.

---

### **1. `Module 1 - Data Ingestion.ipynb`**

Initial setup and ingestion of raw datasets into Spark.

**Key Activities:**

* Creating and configuring **SparkSession**
* Loading all raw CSV files into Spark DataFrames
* Performing initial schema review and validation
* Preparing raw inputs for the cleaning stage

---

### **2. `Module 2-Data Cleaning & Transfomation.ipynb`**

Raw data is standardized, cleaned, and made analytics-ready.

**Key Activities:**

* Fixing schema issues and data types
* Handling **missing values**, outliers, and invalid records
* Removing duplicates and ensuring **data quality**
* Standardizing categorical/text fields
* Feature transformations and enrichment
* Storing cleaned layers for integration

---

### **3. `Module 3 - Data integration & Aggregation.ipynb`**

Combining cleaned datasets and deriving business insights.

**Key Activities:**

* Efficient joins across orders, customers, payments, items, reviews
* Aggregations such as:

  * Total revenue
  * Monthly sales trends
  * State-wise order distribution
  * Delivery performance metrics
* Adding derived features (e.g., weekday/weekend tagging)
* Using caching and persistence for performance gains

---

### **4. `Module 4- Property Optimization.ipynb`**

Advanced performance optimization for real-world scalability.

**Key Activities:**

* Tuning key Spark properties (shuffle partitions, memory configs)
* **Broadcast Joins** for small–large DataFrame joins
* **Partitioning** and **Bucketing** (e.g., bucketing by `customer_id`)
* **Skew Join Optimization** to prevent slow tasks
* General best practices for high-volume workloads

---

### **5. `Module 5 - Data serving.ipynb`**

Final output layer for analytics, reporting, and ML pipelines.

**Key Activities:**

* Saving processed datasets in efficient formats (Parquet / Hive / CSV)
* Organizing final tables into structured directories
* Ensuring compatibility with downstream BI tools
* Preparing long-term storage layers (silver/gold layers)

---

## 🚀 **Getting Started**

### **Prerequisites**

You need a working PySpark environment (local or cloud).

Install:

* Python 3.x
* PySpark
* Jupyter Notebook

### **Execution Steps**

1. **Download the Dataset:**
   Get all Olist CSV files from Kaggle.

2. **Set Up Spark:**
   Configure Spark according to the optimization guidelines shown in
   `Module 4 - Property Optimization.ipynb`.

3. **Run Modules Sequentially:**
   Execute from **Module 1 → Module 5**, as each stage depends on the previous output.
   This reflects a real ETL pipeline flow.




## 📬 **Contact**

**👤 Name:** Trisita Ghosh
**📍 Location:** Roorkee, Uttarakhand
**📧 Email:** **[trishitaheli@gmail.com](mailto:trishitaheli@gmail.com)**
**🔗 LinkedIn:** [https://www.linkedin.com/in/trisitaghosh/](https://www.linkedin.com/in/trisitaghosh/)
**💻 GitHub:** [https://github.com/trishita-26](https://github.com/trishita-26)





