<h1 align="center">Hi 👋, I'm Rina Adibah</h1>

<h3 align="center">
Data Analyst • Analytics Engineering • AI Automation • Business Intelligence • Internal Tools
</h3>

<p align="center">
I build production analytics, automation, and operational systems that turn messy business processes into reliable data workflows, dashboards, and internal tools.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/BigQuery-669DF6?style=for-the-badge&logo=googlebigquery&logoColor=white"/>
  <img src="https://img.shields.io/badge/Looker%20Studio-4285F4?style=for-the-badge&logo=googleanalytics&logoColor=white"/>
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white"/>
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white"/>
</p>

---

## 👋 About Me

I'm a **Data Analyst and AI Automation Builder at Segari**, working across analytics, Business Intelligence, finance operations automation, and internal operational systems.

My work sits between **data analytics, automation, and software-enabled operations**. I design and build systems from the underlying data layer through business rules, workflow automation, monitoring, dashboards, and operational interfaces.

Some of the systems I built, maintain, and currently work on include:

- **Accounts Payable automation** processing 7,000+ supplier emails and approximately 14,000–28,000 documents per month
- **Accounts Receivable automation** using OCR/AI extraction and SKU-level validation against internal Sales Order data
- A production **Midmile Operations Web App** supporting controller and driver workflows
- **BigQuery Single Source of Truth (SoT)** pipelines powering operational BI dashboards across 11 Fulfillment Centres and 1 Processing Centre
- Automated reporting and operational workflows integrating **PostgreSQL, BigQuery, Google Sheets, Gmail, APIs, n8n, and BI tools**

I focus on building systems that are not only automated, but also **traceable, validated, maintainable, and usable by operational teams**.

---

# 🚀 Selected Production Systems

## 1️⃣ Accounts Payable Automation

**Tech:** n8n · OCR · LLM / AI Extraction · Gmail · Google Sheets · BigQuery · SQL

Designed, built, and maintain a production Accounts Payable automation system that processes supplier documents from email intake through validation and exception handling.

### What the system does

- Processes **7,000+ supplier emails per month**
- Handles approximately **14,000–28,000 documents per month**
- Performs document eligibility screening and classification
- Extracts structured information from supplier documents using **OCR + AI**
- Validates extracted information against internal business data
- Automatically responds to suppliers when documents are incomplete or inconsistent
- Routes exceptions for manual review instead of requiring every document to be checked
- Includes monitoring, retry handling, exception management, and operational traceability

### Impact

Approximately **74% straight-through processing for eligible AP documents**, allowing valid submissions to proceed without additional manual document checking.

---

## 2️⃣ Accounts Receivable Document Automation

**Tech:** n8n · OCR · AI Extraction · PostgreSQL · SQL · Google Sheets · APIs

Owned the end-to-end design, development, testing, and maintenance of an Accounts Receivable automation workflow for Sales Order supporting documents.

### Core workflow

**Operational Documents**

→ OCR & AI extraction  
→ SKU-level structured data  
→ Quantity validation  
→ Sales Order reconciliation  
→ Duplicate prevention  
→ Eligibility checks  
→ Structured storage  
→ Reviewer / exception routing

The system validates extracted document information against internal data before documents reach AR reviewers.

### Impact

Approximately **70% straight-through processing for eligible AR documents**, reducing repetitive checking while maintaining validation and exception controls.

---

## 3️⃣ Midmile Internal Operations Web App

**Tech:** Next.js · TypeScript · Tailwind CSS · Supabase PostgreSQL · Supabase Auth · Supabase Storage · Looker Studio

Owned, Designed, built, and launched an internal operational application for Segari's midmile transportation workflow as an individual contributor, covering product design, implementation, testing, deployment, and stakeholder alignment.

### Controller workflows

- Create and assign trips
- Configure routes and stops
- Assign drivers and vehicles
- Monitor trip execution
- Review trip history
- Cancel invalid trips safely
- Access driver operational evidence
- Export operational travel-leg data

### Driver workflows

- Vehicle checklist
- Trip start
- Sequential stop execution
- GPS capture
- Arrival / departure tracking
- Odometer capture and validation
- Toll cost recording and receipt evidence
- Fuel purchase information and receipt evidence
- Trip completion

### System design

The application uses:

- **Supabase Auth** for authenticated role-based access
- **PostgreSQL + RLS/RPCs** for transactional business rules and data integrity
- **Supabase Storage** for operational photo and receipt evidence
- **PostgreSQL → Looker Studio** for operational reporting

The project evolved from an operational requirement into a production system with authentication, workflow guards, evidence handling, validation rules, reporting, and production recovery paths.

---

## 4️⃣ Business Intelligence & Single Source of Truth

**Tech:** BigQuery · SQL · Looker Studio · Metabase · Google Sheets

Built a reusable **Single Source of Truth (SoT)** data layer that serves as the backbone for recurring operational reporting and Business Intelligence.

The system consolidates operational datasets into curated analytical structures instead of rebuilding business logic independently inside each dashboard.

### Coverage

**11 Fulfillment Centres + 1 Processing Centre**

Processing:

- **100K+ operational records**
- **20K+ planogram records**

Supporting analysis for:

- Warehouse utilization
- Slot and capacity planning
- Inventory monitoring
- Product allocation
- Fulfillment Centre performance
- Operational KPI reporting

### Architecture

**Operational Sources**

→ SQL transformation & validation  
→ BigQuery Single Source of Truth  
→ Curated reporting datasets  
→ Looker Studio / Metabase dashboards  
→ Operational decision making

This architecture also provides a reusable data backbone for future automation and reporting workflows.

---

# 🧠 How I Build Systems

I approach analytics and automation as production systems rather than isolated scripts or dashboards.

My typical workflow:

**Business Process**

→ Understand operational rules  
→ Define data contract & validation  
→ Build data / automation pipeline  
→ Add exception handling  
→ Store structured results  
→ Monitor system health  
→ Expose data through dashboards or internal tools  
→ Iterate using production feedback

I pay particular attention to:

- Data quality and reconciliation
- Idempotency and duplicate prevention
- Business-rule validation
- Failure and recovery paths
- Exception handling
- Monitoring and observability
- Operational usability
- Maintainable data models
- Clear ownership between automation and human review

---

# 🛠️ Tech Stack

<div align="center">

### Analytics & Databases

![SQL](https://img.shields.io/badge/SQL-4479A1.svg?style=flat-square&logo=postgresql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1.svg?style=flat-square&logo=postgresql&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6.svg?style=flat-square&logo=googlebigquery&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1.svg?style=flat-square&logo=mysql&logoColor=white)

### Business Intelligence

![Looker Studio](https://img.shields.io/badge/Looker_Studio-4285F4.svg?style=flat-square&logo=googleanalytics&logoColor=white)
![Metabase](https://img.shields.io/badge/Metabase-509EE3.svg?style=flat-square&logo=metabase&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811.svg?style=flat-square&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627.svg?style=flat-square&logo=tableau&logoColor=white)

### Automation & AI

![n8n](https://img.shields.io/badge/n8n-EA4B71.svg?style=flat-square&logo=n8n&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat-square&logo=python&logoColor=white)
![OCR](https://img.shields.io/badge/OCR-Document_Extraction-blue?style=flat-square)
![LLM](https://img.shields.io/badge/LLM-AI_Extraction-purple?style=flat-square)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853.svg?style=flat-square&logo=googlesheets&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail_API-EA4335.svg?style=flat-square&logo=gmail&logoColor=white)

### Internal Applications

![Next.js](https://img.shields.io/badge/Next.js-000000.svg?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6.svg?style=flat-square&logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E.svg?style=flat-square&logo=supabase&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000.svg?style=flat-square&logo=vercel&logoColor=white)

### Data Analysis

![Pandas](https://img.shields.io/badge/Pandas-150458.svg?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243.svg?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C.svg?style=flat-square)

</div>

---

# 📚 Earlier Data Science Projects

Before focusing primarily on production analytics and automation systems, I also built several end-to-end analytics and machine learning projects.

### Customer Retention Strategy — Churn Prediction

**Python · Machine Learning · Tableau · Streamlit**

Built an end-to-end churn analytics pipeline including model benchmarking, business analysis, dashboarding, and deployment.

- Churn recall: **0.83**
- Included retention strategy simulation
- Deployed using Streamlit

### E-Commerce Customer Churn Prediction

**Python · XGBoost · SHAP · LIME**

Built a machine learning pipeline using **5,630 customer behavior records**.

- F2 Score: **0.9617**
- ROC-AUC: **0.9974**
- Included SHAP and LIME model explainability

### AWS SaaS Sales Analysis

**Python · SQL · Business Analytics**

Analyzed B2B SaaS sales performance across customer segments, geographic regions, and discount behavior to identify growth opportunities and improve resource allocation.

---

# ✍️ Writing

1. [Simplify Machine Learning with H2O AutoML](https://medium.com/@rina.adibah.011/simplify-machine-learning-with-h2o-automl-a-beginners-guide-b9da809a0eaa)
2. [Enhancing Data Visualization with Altair](https://medium.com/@rina.adibah.011/enhancing-data-visualization-with-altair-multi-dimensional-sales-analysis-2d1cc3443d9b)
3. [Python GUI for Beginners](https://medium.com/@rina.adibah.011/a-complete-guide-to-creating-gui-applications-in-python-for-beginners-looping-vs-event-handling-e0a4db969562)

---

# 🤝 Connect With Me

<div align="center">

<a href="https://www.linkedin.com/in/rina-adibah/" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2.svg?style=flat-square&logo=linkedin&logoColor=white"/>
</a>
&nbsp;&nbsp;

<a href="https://medium.com/@rina.adibah.011" target="_blank">
  <img src="https://img.shields.io/badge/Medium-000000.svg?style=flat-square&logo=medium&logoColor=white"/>
</a>
&nbsp;&nbsp;

<a href="mailto:rina.adibah.011@gmail.com">
  <img src="https://img.shields.io/badge/Email-D14836.svg?style=flat-square&logo=gmail&logoColor=white"/>
</a>

</div>
