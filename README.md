
This repository contains a Power BI project analyzing Mayo Clinic’s clinical throughput and financial performance across key medical departments (Cardiology, Neurology, Oncology, and Orthopedics). The project integrates historical (2022–2025) and current (2026) datasets, applying Python ETL automation, live SQL storage, and executive Power BI dashboards to deliver insights into operational billing, ward efficiency, patient volume, and Average Length of Stay (ALOS). Dashboards are designed to help hospital administrators and healthcare stakeholders understand facility capacity, clinical bottlenecks, and revenue momentum in real time.

🔄 Pipeline Workflow

* **New Data Arrival** → Healthcare encounter files (CSV/Excel) containing hospital names, clinical departments, stay durations, and gross billing.
* **Python ETL Script** → Cleans raw text rows, normalizes date formats, and standardizes data types.
* **SQL Table Update** → Centralized live local MySQL storage for historical and current patient encounter data.
* **Power BI Refresh** → Star schema update linking `Dim_Calendar` to fact tables for rapid DAX aggregation.
* **Dashboard Updated** → Real-time clinical throughput and financial insights available instantly.
📊 Analytics by Period

**Historical Operations (2022–2025)**

* Long-term revenue momentum and seasonal intake tracking.
* Departmental efficiency and historical Average Length of Stay (ALOS) trends.
* Root-cause billing variance between primary and satellite facilities.
* Year-over-year financial performance tracking across specialized wards.

**Current Operations (2026 YTD)**

* Daily patient encounter and admission volume.
* Real-time ward capacity and discharge velocity.
* Current gross operational billing versus operational targets.
* Average revenue generated per patient by department.

🚀 Key Features

* Automated ingestion and cleaning of clinical patient encounter data.
* Premium dark-mode KPI dashboards tracking Total Operational Billing ($6.36M), ALOS (5.42 Days), and Patient Volume.
* Advanced interactive visuals including Revenue Momentum area charts, Year-Over-Year line charts, and Revenue Build waterfall charts.
* Custom Star Schema data modeling with explicit DAX measures for dynamic time-intelligence reporting.
* Executive-grade UI optimized for high-contrast presentation and root-cause variance analysis.

🛠️ Tools & Technologies

* **Python** (Pandas) for ETL scripting, raw text cleaning, and data standardization.
* **SQL** (MySQL Server) for structured clinical storage and live database engine connectivity.
* **Power BI Desktop** for executive visualization, DAX modeling, and dashboard deployment.

📌 Future Enhancements

* Predictive analytics for seasonal patient volume and bed-shortage forecasting.
* Cloud-native database integration (Azure/AWS) for live, hospital-wide data streams.
* Incremental refresh configuration for scaling large, multi-year clinical datasets.
* Drill-through reporting pages for specialized physician performance and hourly throughput insights.

🖼️ Screenshots & Demos

* **Dashboard Snapshot – Healthcare Operations Analytics:** [Insert your GitHub image link here, e.g., `[https://github.com/YourUsername/Mayo-Clinic-Operations-Analytics/blob/main/dashboard_snapshot.png](https://github.com/YourUsername/Mayo-Clinic-Operations-Analytics/blob/main/dashboard_snapshot.png)`]
* **Pipeline Flow:** CSV → Python ETL → SQL → Power BI → Dashboard
