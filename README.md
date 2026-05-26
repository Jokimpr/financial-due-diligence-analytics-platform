# Financial Due Diligence Analytics Platform

## 📊 Overview
This platform simulates how transaction advisory and private equity analytics teams ingest, clean, and process fragmented financial and operational datasets from enterprise systems during pre-acquisition due diligence. By transforming raw, cryptic ERP databases into structured analytical models, this platform accelerates deal-vetting and risks assessment workflows.

---

## 🛠️ Tech Stack
* **Data Transformation Layer:** dbt-Core (Data Build Tool)
* **Analytical Database Engine:** DuckDB (High-performance local OLAP engine)
* **Data Ingestion & Source Data System:** SAP ERP Financial & Sales Transaction Ledgers
* **Data Visualization Platform:** Power BI Executive Dashboard
* **Workflow Automation:** Activepieces (Automated monitoring & anomaly alerts)
* **Version Control & CI/CD Pipeline:** Git & GitHub Actions Automated Testing

---

## 💼 Business Problem
A private equity firm is evaluating the target acquisition of a multi-region enterprise retail business. However, the target company's financial records are locked behind highly fragmented, raw SAP database schemas, disconnected billing ledger files, and general accounting entries. 

To prevent overvaluation, the transaction team requires automated, repeatable analytics to audit historical earnings stability, revenue concentration risks, and operational cash flow health prior to closing the deal.

---

## 🏗️ Project Architecture & Data Flow
[Raw SAP ERP Tables]          ➔ Ingested into local DuckDB storage
(VBAK, VBAP, BSEG, BKPF)
↓
[dbt Staging Views]           ➔ Re-casting, field decoding, and line-ending normalization
(stg_sap_orders, stg_ledgers)
↓
[dbt Financial Data Marts]    ➔ Complex multi-layered CTE processing & window calculations
(fct_ltm_revenue, dim_clients)
↓
[Power BI Dashboard]          ➔ Executive visualization of M&A KPIs & Diligence Metrics
↓
[Activepieces Automation]     ➔ Triggered anomaly detection and automated variance alerts

---

## 📈 Core Analytics Capabilities & Financial Engineering
* **Rolling LTM (Last Twelve Months) Revenue:** Multi-year trend parsing to evaluate absolute baseline revenue momentum.
* **Revenue Concentration Risk Detection:** Evaluating top-client dependencies to uncover underlying customer churn risks.
* **EBITDA Margin Analytics:** Granular analysis of operational cost scaling by extracting structural expense segments from general ledger balances.
* **DSO (Days Sales Outstanding) Aging Calculations:** Benchmarking cash collection velocities across varied retail territories.

---

## 🎯 Key Verified Metrics
* ✅ **LTM Revenue Trend**
* ✅ **EBITDA Margin Analysis**
* ✅ **Customer Retention Metrics**
* ✅ **Top Client Revenue Dependency %**
* ✅ **Regional Margin Performance**
* ✅ **Invoice Aging Breakdown (DSO)**