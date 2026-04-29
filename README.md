# Jagadeesh Kumar Linganti
### Senior Data Engineer | Azure | AWS | Snowflake | Databricks | PySpark | ETL/ELT

📍 **Location:** Stuttgart Region, Germany  
📧 **Email:** [lingantijagadeesh02@gmail.com](mailto:lingantijagadeesh02@gmail.com)  
🔗 **LinkedIn:** [linkedin.com/in/jagadeesh-linganti](https://www.linkedin.com/in/jagadeesh-linganti)

---

## 🚀 PROFESSIONAL SUMMARY
**Senior Data Engineer** with 5+ years of experience architecting cloud-native data ecosystems. Specialist in **Medallion Architectures**, **Real-Time Streaming**, and **Enterprise Data Governance**. Proven track record of reducing operational costs by 30% and improving pipeline performance by 40%. **Technical Lead** experienced in mentoring junior engineers, driving Agile sprints, and aligning data strategy with cross-functional business stakeholders.

---

## 🌟 FEATURED PROJECTS (DETAILED CASE STUDIES)

### 🔹 1. Enterprise Data Integration & Analytics Platform
**Company:** Wunderman Thompson (UK)  
**I/O Flow:** `[APIs/On-Prem]` ➡ `[ADF]` ➡ `[Databricks (PySpark)]` ➡ `[dbt]` ➡ `[Snowflake]` ➡ `[Power BI]`

## 🔄 End-to-End Pipeline Architecture 

![Architecture](https://github.com/jagadeesh472/jagadeesh-linganti-data-engineer-portfolio/blob/222ff55a222b0fa3d46a3c4444771d66b197547d/Enterprise%20Data%20Integration%20%26%20Analytics%20Platform/image/enterprise%20data%20ingestion.png)

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


## Logical Flow

![Logic Flow](https://github.com/jagadeesh472/jagadeesh-linganti-data-engineer-portfolio/blob/20924c7058f6327c34be4bb5c4ab409c73e41659/profitability_loss_Architecture/images/Jh9VileGMpQxgNhSddQxj5VuV7gvwP6eMoPUbdIm9Bw6zmKIsjxsMTT3i05aFYyXjyAg0Ui-xUqxPdELy5kW0eJoxaouCVtQGoqEnnRQXAg3gsyf086rkJyYNgnzICgE5-UHocsfvWwTGjScTZaJz_KIUxYYOUWlFmZJb0sEo5QXS6GOTEDMul6owEXdpEFp.jpeg)


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

## 🏗️ Architecture Overview

![Architecture](https://github.com/jagadeesh472/jagadeesh-linganti-data-engineer-portfolio/blob/0ca3ae2e246e19734be3a0f16a67e92b2c93c7a5/Disney%20Social%20Media%20Data%20Lakehouse%20Architecture.diagrames/image/vx0v4HJbaPvNpgcDMbnbKgWOxat4mDdkq9k5xj5S3lr4l9z4kfQOOF7z2GgyGesR7fS_MqmsVmmjXc2E4gaPcg3KiGRuWx_y2pntiyuDoW5E2h20cpSJdFqQ1JFFpvTbHy-petA7CBrQBmov1Du8KSmOkZ1hOcweK6uQino3YCAqZQ4rCsVfuRWZIvtD-ifv.jpeg)

## 📥 Data Ingestion

![Ingestion](https://github.com/jagadeesh472/jagadeesh-linganti-data-engineer-portfolio/blob/0ca3ae2e246e19734be3a0f16a67e92b2c93c7a5/Disney%20Social%20Media%20Data%20Lakehouse%20Architecture.diagrames/image/0rm9o22hz9ptHQ4Idr8d4k7O1GA8s5ZcuF638MUauA8PoOCBeI-7JEjxdArbYF4l_hSu33NuXu-56DIBddCF9G2qAcTi_AJVfGFTZFhK1E9KE5HEBZqL93Jpc6skAQTIaR6VJmGo_w0xEIDq_8ghGnsZyqDItkPm63DoiB47dAjxz34pXXaAA7Hd0iqknxQy.jpeg)


## ⚙️ Data Transformation (dbt)

![Processing](https://github.com/jagadeesh472/jagadeesh-linganti-data-engineer-portfolio/blob/0ca3ae2e246e19734be3a0f16a67e92b2c93c7a5/Disney%20Social%20Media%20Data%20Lakehouse%20Architecture.diagrames/image/vI26WfsyZqFsSIslA_hE6-WKQ_1PFyNX54Klt2aj5DxlNwumVewGJYsF3b6w4j1z2yX9fXfewa9DicnD2jj_JH5N7FpEOUQbSBTHUzgZoWX-BWt83xBoCDMRLW4Yt_b7KS_3BDxgWm2zj0cnUf3v6itYhZbJDlEH2ZSA9FfOAGvKbBvWZy8a_yEhVT_PH_4u.jpeg)

## 🥇 Medallion Architecture

![Medallion](https://github.com/jagadeesh472/jagadeesh-linganti-data-engineer-portfolio/blob/f21179550c7a8cdaa574de27b9b94ff9dc568dd3/Disney%20Social%20Media%20Data%20Lakehouse%20Architecture.diagrames/image/D64myjNAr4D7F1b8lSPPyJ8SoNs8KZwUxSJS9yPaQCC06eIlzXGzxG7H2AD6tJOXXOhbl7mrJQX4VSdhwbJZEnY346uGKCFzjWEXFDHgK6-W0GFYvmWRIFc5YNpz89RhuLwHoDGLxiv1k3SaR9FMWFq3zcN2z_puI74FeXCzfsEzNgf5xAQ4L2EZdMiHmXB2.jpeg)


#### 🏗️ Technical Deep Dive
* **Engineering Challenge:** Processing millions of complex, nested arrays within JSON events.
* **Solution:** Developed a recursive **PySpark flattening engine** that dynamically explodes nested structures. Combined with **Snowflake’s VARIANT** data type, this provided a "Schema-on-Read" capability that reduced processing time by **50%**.

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
