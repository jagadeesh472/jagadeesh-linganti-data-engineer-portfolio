# Jagadeesh Kumar Linganti  
## Senior Data Engineer | Azure | AWS | Snowflake | Databricks | PySpark | ETL/ELT

📍 Germany | 📧 lingantijagadeesh02@gmail.com  

---

# 🚀 PROFESSIONAL SUMMARY

Senior Data Engineer with 5+ years of experience designing and delivering scalable, cloud-native data platforms across Azure, AWS, and GCP.

Expert in building high-performance ETL/ELT pipelines, real-time data processing systems, and enterprise-grade data architectures with strong focus on **data quality, governance, and cost optimization**.

---

# 🌟 FEATURED PROJECTS (DETAILED CASE STUDIES)

---

## 🔹 1. Enterprise Data Integration & Analytics Platform  
**Company:** Wunderman Thompson (UK)  

### 📌 Business Problem
Organizations had fragmented data across multiple platforms (marketing, sales, customer systems), making it difficult to generate unified insights and real-time analytics.

---

### 🏗️ Solution Architecture
Designed and implemented a **centralized enterprise data platform** using:
- Azure Data Factory for ingestion  
- Azure Databricks (PySpark) for processing  
- Snowflake for scalable data warehousing  
- dbt for transformation and testing  

Created a **multi-layer architecture**:
➡ Raw Layer → Transform Layer → Curated Layer  

---

### ⚙️ Key Contributions
- Built end-to-end ETL pipelines integrating APIs, on-prem, and cloud sources  
- Optimized PySpark workloads → improved performance by **40%**  
- Implemented automated data quality checks → reduced issues by **60%**  
- Designed Snowflake optimization strategies (clustering, materialized views)  
- Developed Power BI semantic models for executive dashboards  
- Enforced GDPR compliance and RBAC security  

---

### 📈 Business Impact
- Enabled **real-time analytics across global teams**  
- Improved decision-making with reliable, high-quality data  
- Reduced operational inefficiencies and data inconsistencies  

---

## 🔹 2. Financial Analytics & Profitability Platform  
**Company:** Janus Henderson  

🔹 Project: Real-Time Financial Profitability & Loss (P&L) Platform
Company: Janus Henderson Investors

Role: Senior Data Engineer

📌 Business Problem
The finance and investment teams lacked a "single source of truth" for real-time profitability. Manual data consolidation across diverse asset classes and global regions caused delays, leading to outdated P&L insights and reactive rather than proactive decision-making.

🏗️ Solution Architecture: The Unified Hybrid Lakehouse
I architected a high-performance, hybrid data platform that leverages the best of both worlds: Databricks for heavy-duty engineering and Snowflake for executive-level serving.

Ingestion: Used Informatica and ADF to pull raw financial transactions and General Ledger data into a Data Lake (Bronze Layer).

Processing (Silver Layer): Engineered PySpark pipelines in Databricks to perform complex financial currency conversions, deduplication, and multi-asset reconciliations.

Modeling (Gold Layer): Implemented a Daily Snapshot/SCD Type 2 strategy (as shown in the sample data) in Snowflake to track historical profitability changes over time.

Governance: Applied PII masking and Row-Level Security (RLS) to ensure global compliance with financial regulations.

⚙️ Key Technical Contributions
Temporal Data Modeling: Designed the primary key structure (DATE_KEY + CLIENT_PK) to enable "Point-in-Time" reporting, allowing the business to view P&L metrics as they existed on any historical date.

Performance Engineering: Optimized Snowflake compute by implementing Clustering Keys on high-volume financial tables, reducing query wait times for analysts from minutes to seconds.

Data Validation Gates: Built automated "Quality Shields" between the Bronze and Silver layers to catch data drift or missing transaction records before they hit the P&L dashboards.

📈 Business Impact
Real-Time Visibility: Shifted P&L reporting from a "monthly lag" to near real-time, enabling faster capital allocation.

Audit Readiness: The snapshot-based architecture provided a 100% transparent audit trail for every financial figure.

Scalability: The platform now handles millions of daily transactions with zero manual intervention. 

---

🔹 3. Disney Social Media Data Migration & Analytics
Company: Wunderman Thompson

📌 Business Problem
Massive volumes of high-velocity social media telemetry (Twitter, TikTok, etc.) were arriving in unstructured formats. The existing infrastructure could not scale to ingest millions of daily events, resulting in "dark data" that provided no marketing value.

🏗️ Solution: The Social Intelligence Lakehouse
Designed a scalable engine to transform volatile JSON/CSV social streams into high-value analytical assets.

Caption: Technical architecture illustrating the flow from API ingestion to a structured Snowflake warehouse.

[Twitter API]   [TikTok API]   [Social Feeds]
        │             │              │
        └─────────────┴──────────────┘
                     │
          [Azure Data Factory]
       (API Ingestion + Scheduling)
                     │
                     ▼
        [Snowflake - Raw Stage]
     (JSON / CSV - Unprocessed Data)
                     │
                     ▼
        [Databricks - PySpark]
   - JSON Flattening
   - Data Enrichment
   - Deduplication
                     │
                     ▼
              [dbt Layer]
   - Transformation Models
   - Schema Validation Tests
   - Data Quality Checks
                     │
                     ▼
         [Snowflake Warehouse]
   - Fact: Engagement, Impressions
   - Dim: Campaign, User
   - Clustering (timestamp, campaign_id)
                     │
                     ▼
             [Power BI]
   - Campaign ROI Dashboard
   - Trend Analysis


Ingestion: Automated multi-source API ingestion using ADF, landing raw telemetry into a Snowflake staging area.

Transformation: Utilized Databricks (PySpark) for heavy-duty parsing of nested JSON structures and dbt for modular, version-controlled SQL modeling.

Storage: Implemented a layered schema in Snowflake to separate raw social feeds from refined engagement metrics.

⚙️ Key Technical Contributions
Semi-Structured Data Handling: Developed efficient PySpark scripts to flatten deeply nested JSON arrays, significantly reducing processing complexity.

Storage Optimization: Optimized Snowflake storage costs by implementing appropriate clustering keys on high-cardinality columns like timestamp and campaign_id.

Data Reliability: Built dbt tests to catch "schema drift"—ensuring that if a social platform changed its API response format, the pipeline would alert the team before downstream dashboards broke.

📈 Business Impact
Actionable Intelligence: Provided the marketing team with real-time ROI metrics, allowing for mid-campaign adjustments.

Audience Growth: Increased audience engagement by identifying high-performing content trends via automated Power BI dashboards.

----

🔹 4. Retail Cloud Migration (On-Prem → AWS)
📌 Business Problem
Legacy on-premise SQL servers were struggling with peak holiday traffic, causing severe latency in inventory updates and preventing real-time analytics for store managers.

🏗️ Solution: Serverless Speed Layer
Led a full-scale migration to a decoupled, cloud-native architecture on AWS.


                 🔴 REAL-TIME LAYER
[POS Systems] → [Amazon Kinesis]
                     │
                     ▼
         [Spark Streaming - Glue]
         (Real-time Processing)
                     │
                     ▼
                 [S3 - Processed]

                 🔵 BATCH LAYER
[On-Prem SQL Server]
         │
         ▼
      [AWS Glue ETL]
         │
         ▼
      [S3 Data Lake]

                 ⬇ MERGED ⬇

              [Amazon Athena]
        (Serverless Query Engine)
                     │
                     ▼
              [QuickSight]
        (Retail Dashboards)

The "Speed Layer": Implemented Amazon Kinesis to capture real-time Point-of-Sale (POS) transactions.

The "Batch Layer": Used AWS Glue for massive historical data migrations from on-prem to S3.

The Query Layer: Leveraged Amazon Athena for serverless ad-hoc analysis and QuickSight for visual reporting.

⚙️ Key Technical Contributions
Hybrid Migration Strategy: Architected a "Parallel Run" strategy where on-prem and AWS lived together during a 3-month transition to ensure zero downtime.

Spark Streaming: Developed Spark Streaming jobs within AWS Glue to process Kinesis shards, ensuring inventory levels were updated within seconds of a sale.

Cost Management: Utilized S3 Lifecycle policies and Parquet partitioning to minimize storage and query costs in Athena.

📈 Business Impact
99.9% Scalability: The platform now scales automatically to handle 10x spikes in traffic during Black Friday sales.

Cost Reduction: Reduced infrastructure overhead by 30% by moving from fixed servers to serverless compute.

---

🔹 5. Finance Data Fabrication Platform
Company: L2B Cloud

📌 Business Problem
Inconsistent financial reporting due to "Data Silos." Fragmented systems (ERP, CRM, Banking) led to conflicting numbers, creating a lack of trust in enterprise-wide reporting.

🏗️ Solution: The Single Source of Truth (SSOT)
Built a centralized platform designed for high-integrity financial fabrication and reporting.


[ERP]   [CRM]   [Banking APIs]
   │       │         │
   └───────┴─────────┘
           │
   ┌───────────────┐
   │ Ingestion     │
   │ ADF (Batch)   │
   │ Kafka (Stream)│
   └───────────────┘
           │
           ▼
   [Azure Data Lake Gen2]
   - Raw Layer
   - Processed Layer
   - Curated Layer
           │
           ▼
   [Databricks]
   - ETL Pipelines
   - Streaming Processing
           │
           ▼
   [Synapse Analytics]
   - Financial Models
   - Reporting Tables

   🔐 Governance Layer (Overlay)
   - Data Lineage
   - RBAC
   - PII Masking

           ▼
   [BI / Finance Dashboards]

Unified Lakehouse: Used Azure Data Lake Storage (ADLS) Gen2 as the foundation, with Synapse Analytics and Databricks for processing.

Streaming Integration: Integrated Kafka to handle real-time cash flow updates and banking signals.

⚙️ Key Technical Contributions
Data Lineage & Governance: Implemented end-to-end lineage tracking to ensure every financial figure could be traced back to its raw source for audit compliance.

Security & PII: Applied advanced PII masking and Role-Based Access Control (RBAC) to protect sensitive client financial data while remaining GDPR compliant.

Automated Reconciliation: Built automated reconciliation scripts to identify discrepancies between different source systems in real-time.

📈 Business Impact
Data Trust: Achieved 100% reporting consistency, enabling executives to make confident, data-driven financial decisions.

Audit Efficiency: Reduced internal audit preparation time by 50% through improved data traceability.

---

🔹 6. Transaction Monitoring System (AML)
📌 Business Problem
A critical need to detect and prevent money laundering (AML) activities by identifying suspicious transaction patterns in real-time.

🏗️ Solution: Automated Compliance Engine
Developed a robust monitoring system focused on high-performance detection and reporting.

Orchestration: Used Azure Data Factory to schedule high-frequency transaction polls.

Logic Engine: Leveraged Azure SQL DWH and complex T-SQL logic to run fraud-detection algorithms.

⚙️ Key Technical Contributions
Optimized Stored Procedures: Rewrote legacy fraud detection logic into high-performance T-SQL stored procedures, reducing detection time from minutes to seconds.

Pattern Recognition: Designed automated pipelines that flag transactions exceeding specific risk thresholds or originating from high-risk jurisdictions.

Data Migration: Engineered seamless data migration pathways to move historical records into long-term cold storage for regulatory record-keeping.

📈 Business Impact
Reduced Risk: Significantly strengthened the firm’s AML compliance posture, preventing potential regulatory fines.

Operational Speed: Improved the efficiency of compliance officers by automating the "Red Flag" notification process.

---

🔹 7. E-Commerce Data Platform
📌 Business Problem
Retail analytics required a platform that could handle both high-volume batch updates and low-latency streaming of customer clickstream data.

🏗️ Solution: The Delta Lake Advantage
Built a cloud-native platform utilizing the Delta Lake format to ensure ACID transactions on a data lake.

Processing: Azure Databricks handled the transformation of raw events into structured Delta tables.

Streaming: Used Kafka for real-time customer behavior tracking.

Analytics: Served the final, curated data into Snowflake for high-concurrency BI reporting.

⚙️ Key Technical Contributions
Schema Enforcement: Utilized Delta Lake’s schema enforcement to prevent "bad data" from corrupting the production tables.

Real-time KPIs: Implemented streaming pipelines that calculated live conversion rates and cart abandonment metrics.

Performance Tuning: Applied Z-Ordering and file compaction in Databricks to maintain high query performance as the data lake grew.

📈 Business Impact
Real-time Personalization: Enabled the marketing team to trigger real-time offers based on live customer behavior.

Operational Efficiency: Streamlined the retail supply chain by providing real-time inventory visibility across all e-commerce channels.

---

# 🏆 KEY ACHIEVEMENTS

- 🚀 Improved data pipeline performance by **40%**  
- 📉 Reduced data quality issues by **60%**  
- 💰 Delivered cost-optimized cloud solutions  
- 📊 Built real-time analytics systems  
- 🔐 Ensured GDPR-compliant data governance  

---

# 🎓 Certifications                              Certification Number

- Microsoft Certified: Power BI Developer        | C1824C-8C38MA
- Microsoft Certified: Azure Fundamentals        | 81R618-4F60B1
- Microsoft Certified: Azure Developer Associate | FDI030-81EDCB

---

# 🤝 CONTACT

🔗 LinkedIn: https://www.linkedin.com/in/jagadeesh-linganti  
📧 Email: lingantijagadeesh02@gmail.com  

---
