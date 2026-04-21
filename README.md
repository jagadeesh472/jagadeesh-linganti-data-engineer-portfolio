# Jagadeesh Kumar Linganti
### Senior Data Engineer | Azure | AWS | Snowflake | Databricks | PySpark | ETL/ELT

📍 **Location:** Stuttgart Region, Germany  
📧 **Email:** [lingantijagadeesh02@gmail.com](mailto:lingantijagadeesh02@gmail.com)  
🔗 **LinkedIn:** [linkedin.com/in/jagadeesh-linganti](https://www.linkedin.com/in/jagadeesh-linganti)

---

## 🚀 PROFESSIONAL SUMMARY
**Senior Data Engineer** with 6+ years of experience architecting cloud-native data ecosystems. Specialist in **Medallion Architectures**, **Real-Time Streaming**, and **Enterprise Data Governance**. Proven track record of reducing operational costs by 30% and improving pipeline performance by 40%. **Technical Lead** experienced in mentoring junior engineers, driving Agile sprints, and aligning data strategy with cross-functional business stakeholders.

---

## 🌟 FEATURED PROJECTS (DETAILED CASE STUDIES)

### 🔹 1. Enterprise Data Integration & Analytics Platform
**Company:** Wunderman Thompson (UK)  
**I/O Flow:** `[APIs/On-Prem]` ➡ `[ADF]` ➡ `[Databricks (PySpark)]` ➡ `[dbt]` ➡ `[Snowflake]` ➡ `[Power BI]`

#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Managing "Schema Drift" from external marketing APIs that frequently changed output formats.
* **Solution:** Implemented **Databricks Autoloader** with schema evolution to incrementally ingest data. Used **dbt** for the Gold layer to enforce strict schema validation and modular SQL tests, ensuring downstream dashboards remained stable.

#### 📈 Impact, Scalability & Audit
* **Business Impact:** Reduced data quality issues by **60%**, enabling reliable real-time global analytics.
* **Audit Readiness:** Integrated **Azure Purview** for end-to-end data lineage and documentation.
* **Scalability:** Optimized PySpark shuffle partitions, resulting in a **40% performance gain**.

---

### 🔹 2. Real-Time Financial P&L Platform
**Company:** Janus Henderson Investors  
**I/O Flow:** `[Fin. Trans]` ➡ `[ADF]` ➡ `[Bronze Lake]` ➡ `[Databricks (SCD2)]` ➡ `[Snowflake (Gold)]`

## 🏗️ Architecture
![Architecture](https://github.com/jagadeesh472/jagadeesh-linganti-data-engineer-portfolio/tree/c00a22637d09a49b0b6b5726d14e77bf060650fb/profitability_loss_Architecture/images)

#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Enabling "as-of" date reporting for any historical point in time.
* **Solution:** Architected a **Slowly Changing Dimension (SCD) Type 2** strategy. Developed PySpark logic to compare daily records against the master, closing old records with a `VALID_TO` timestamp and opening new ones, allowing "point-in-time" financial views.

#### 📈 Impact, Scalability & Audit
* **Business Impact:** Shifted reporting from "monthly" to "near real-time," accelerating capital cycles.
* **Audit Readiness:** Provided a 100% transparent audit trail for financial regulators (**SEC/FCA**).
* **Scalability:** Implemented **Snowflake Clustering Keys** on transaction dates to maintain sub-second query speeds.

---

### 🔹 3. Social Media Intelligence Lakehouse (Disney)
**Company:** Wunderman Thompson  
**I/O Flow:** `[Social APIs]` ➡ `[ADF]` ➡ `[Databricks (Flattening)]` ➡ `[dbt]` ➡ `[Snowflake]`

#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Processing millions of complex, nested arrays within JSON events.
* **Solution:** Developed a recursive **PySpark flattening engine** that dynamically explodes nested structures. Combined with **Snowflake’s VARIANT** data type, this provided a "Schema-on-Read" capability that reduced processing time by **50%**.

---

### 🔹 4. Retail Cloud Migration (On-Prem ➡ AWS)
**I/O Flow:** `[POS]` ➡ `[Kinesis]` ➡ `[AWS Glue (Streaming)]` ➡ `[S3]` ➡ `[Athena]` ➡ `[QuickSight]`

#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Moving terabytes of historical data with zero downtime.
* **Solution:** Implemented a **Lambda Architecture**. The Batch Layer (Glue) migrated historical data to S3 Parquet, while the Speed Layer (Kinesis + Spark Streaming) processed live transactions in 60-second micro-batches.

---

### 🔹 5. Finance Data Fabric (SSOT)
**Company:** L2B Cloud  
**I/O Flow:** `[ERP/Banking]` ➡ `[Kafka]` ➡ `[ADLS Gen2]` ➡ `[Databricks]` ➡ `[Synapse]`

#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Reconciling conflicting data values across different source systems.
* **Solution:** Built a **Master Data Management (MDM) Survivorship engine** in Databricks. It assigned "Source Confidence Scores" to resolve discrepancies and create a single high-integrity record.

---

### 🔹 6. AML Transaction Monitoring (Compliance)
**I/O Flow:** `[Trans. Systems]` ➡ `[ADF]` ➡ `[Azure SQL DWH]` ➡ `[T-SQL Detection]` ➡ `[Alerts]`

#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Legacy fraud detection was too slow to stop transactions in real-time.
* **Solution:** Migrated logic into **optimized, set-based T-SQL Stored Procedures** within Azure Synapse. Reduced the "Transaction-to-Alert" window from minutes to **under 15 seconds**.

---

### 🔹 7. E-Commerce Real-Time Delta Lake
**I/O Flow:** `[Web/Clickstream]` ➡ `[Kafka]` ➡ `[Databricks (Streaming)]` ➡ `[Delta Lake]` ➡ `[Snowflake]`

#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Handling "Late-Arriving Events" that skewed real-time session metrics.
* **Solution:** Implemented **Spark Streaming Watermarking** (10-min threshold). Used **Delta Lake Z-Ordering** on `customer_id` and `timestamp` for lightning-fast read performance.

---

## 🏆 KEY METRICS SUMMARY

| Pillar | Achievement |
| :--- | :--- |
| **Pipeline Performance** | 40% Improvement through Spark/Snowflake tuning. |
| **Data Quality** | 60% Reduction in incidents via automated dbt/Delta checks. |
| **Cost Savings** | 30% Reduction using serverless and lifecycle policies. |
| **Leadership** | Lead Agile teams and mentored junior engineers in PySpark best practices. |

---

## 🎓 CERTIFICATIONS & LANGUAGES

* **Microsoft Certified: Power BI Developer** | Verify: C1824C-8C38MA
* **Microsoft Certified: Azure Fundamentals** | Verify: 81R618-4F60B1
* **Microsoft Certified: Azure Developer Associate** | Verify: FDI030-81EDCB
* **Languages:** English (Fluent), **German (Elementary A1 - Currently pursuing)**, Telugu (Native).
