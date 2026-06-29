# Hi there, I'm Yana Kel! 👋

<p align="left">
  <a href="https://linkedin.com" target="_blank">
    <img src="https://shields.io" alt="LinkedIn">
  </a>
  <a href="mailto:k.y.kel.yana@gmail.com">
    <img src="https://shields.io" alt="Email">
  </a>
</p>

### 👩‍💻 Professional Profile
Analytics Engineer with hands-on experience in integrating multiple data sources, building ETL/ELT pipelines, and delivering end-to-end analytics. Built and optimized data warehouses, data marts, and data models with a focus on data quality, performance, and reliability. Experienced in implementing validation checks, monitoring, and business logic controls to support enterprise analytics and reporting.

---

### 🛠️ Technical Stack & Tools

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🔹 Core Analytics & Storage</h4>
      <img src="https://shields.io" alt="SQL">
      <img src="https://shields.io" alt="PostgreSQL">
      <img src="https://shields.io" alt="Greenplum"><br>
      <img src="https://shields.io" alt="ClickHouse">
      <img src="https://shields.io" alt="Pandas">
    </td>
    <td width="50%" valign="top">
      <h4>🔹 Orchestration & Infrastructure</h4>
      <img src="https://shields.io" alt="Airflow">
      <img src="https://shields.io" alt="Docker"><br>
      <img src="https://shields.io" alt="Git">
      <img src="https://shields.io" alt="DBeaver">
    </td>
  </tr>
</table>

---

### 🚀 Featured Projects & Architecture

#### 🚖 [High-Load NYC Taxi Analytics Pipeline & MPP Architecture](https://github.com)
*   **Objective:** Built an automated multi-stage ELT/ETL pipeline to process, clean, and visualize **7.6 million rows** of New York taxi transactional data.
*   **Implementation:** 
    *   Designed a 3-layer architecture: **RAW** (PostgreSQL) ──► **CORE** (Greenplum MPP) ──► **MARTS** (ClickHouse) [^3^].
    *   Automated orchestration using **Apache Airflow**, implementing strict Data Quality (DQ) filters inside SQL layers to eliminate anomalies (broken taximeters, incorrect timestamps, zero-amount transactions) [^3^].
    *   Optimized cross-database data delivery by implementing **PXF (Platform Extension Framework) Writable External Tables**, achieving high-speed direct streaming from Greenplum MPP directly into ClickHouse `MergeTree` tables without staging memory overhead [^3^].
    *   Delivered business insights via interactive dashboards inside **Apache Superset** [^3^].
*   **Stack:** Greenplum MPP, ClickHouse, PostgreSQL, Apache Airflow, Docker, Apache Superset, SQL, Pandas [^3^].

#### 💼 [Corporate Banking Analytics & MPP Warehouse Architecture](https://github.com)
*   **Objective:** Designed an analytical data mart inside an MPP environment to calculate **Net Interest Income (NII)** and portfolio profitability.
*   **Implementation:** Deployed a local Greenplum cluster using Docker. Optimized query performance by setting appropriate distribution keys (`DISTRIBUTED BY`) for huge transactional fact tables and broadcasting small flat dimensions (`DISTRIBUTED REPLICATED`), achieving zero-network overhead via **Local Joins**.
*   **Stack:** Greenplum Database, Advanced SQL, Docker, DBeaver.

#### 🛡️ [Data Quality Framework & Automated ETL Monitoring](https://github.com)
*   **Objective:** Built a scalable data lineage pipeline with built-in financial data validation checks.
*   **Implementation:** Implemented business logic controls, row-count tracking, and null-value monitoring inside staging layers to support executive-level regulatory reporting.
*   **Stack:** PostgreSQL, Apache Airflow, Docker.

---

### 📊 GitHub Activities & Insights

<p align="left">
  <img src="https://vercel.app" alt="Yana's GitHub Stats" width="48%" />
  <img src="https://vercel.app" alt="Top Languages" width="48%" />
</p>

---

### 🤝 Contact & Collaboration
I am always open to discussing data infrastructure optimization, robust business control implementations, or analytical modeling:
*   **LinkedIn:** [Connect with me](https://linkedin.com)
*   **Email:** k.y.kel.yana@gmail.com
