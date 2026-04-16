🏥 Hospital Emergency Room Dashboard

An end-to-end data analytics project built in Microsoft Excel, covering the complete data analyst workflow — from raw data ingestion and cleaning to data modelling, DAX calculations, and an interactive dashboard.



Project Overview

This project analyzes **9,216 Emergency Room patient records across 2023 to 2024 ** to uncover trends in patient volume, wait times, satisfaction scores, admission status, and departmental referrals. The goal was to build a dynamic, interactive dashboard that helps hospital management make data-driven decisions.



Project Workflow

 Steps : 

 1  **Business Requirement Gathering** — Defined KPIs and questions the dashboard should answer 
 2  **Understanding the Data** — Explored structure, columns, and data quality issues 
 3  **Data Connection via Power Query** — Imported both datasets into Excel using Power Query 
 4  **Data Cleaning & Quality Check (Power Query)** — Standardized gender values (M → Male, F → Female), removed            duplcate column (Patient Admission Flag.1), handled nulls, fixed date formats 
 5  **Calendar Table (Power Query)** — Built a custom Calendar Table from the dataset using M language in Power             Query, used for time-based analysis 
 6  **Data Modelling in Power Pivot** — Loaded datasets into the Data Model and built a **one-to-many relationship**        between tables 
 7  **DAX Calculations** — Created calculated columns and measures using DAX formulas in Power Pivot 
 8  **Pivot Tables** — Loaded data from the Data Model into Pivot Tables in an existing sheet 
 9  **Dashboard Development** — Built an interactive dashboard using charts, slicers, sparklines, area charts, bar          charts, donut chart, and KPI visuals 
 10  **Insights Generation** — Derived key findings from the complete dataset 


Dashboard KPIs Covered

 KPI | Status 
-----|--------
 Total Number of Patients 
 Average Wait Time 
 Patient Admission Status (Admitted / Not Admitted) 
 Patient Age Distribution 
 Gender Analysis 
 Department Referrals 
 % of Patients Seen Within 30 Minutes 


 Key Insights
 > **Insights are based on the default full-year view. Numbers update dynamically based on slicer selections (month/year)**

- **More than half of all patients experienced delays** — the majority of ER visitors waited longer than 30 minutes, highlighting a significant operational bottleneck in patient flow
- **Average wait time exceeds 30 minutes** — with a wide range across days, suggesting inconsistent staffing or triage processes that could be improved
- **Admission rate is nearly split 50/50** — a large proportion of ER cases could potentially be redirected to outpatient or urgent care services, reducing pressure on the ER
- **The 30–39 age group is the most frequent visitor** — the ER serves a predominantly young-to-middle-aged population, which should inform care and resource planning
- **General Practice receives the highest referrals by a significant margin** — nearly double the next highest department, indicating potential capacity pressure
- **Average satisfaction score sits just below the midpoint** — patient experience needs improvement, and the data suggests a direct link between longer wait times and lower satisfaction scores
- **Patient volume varies noticeably by month** — certain months see higher footfall, making them useful indicators for seasonal staffing and resource planning

---

 Tools & Techniques Used

- **Microsoft Excel** — Primary tool
- **Power Query** — Data import, cleaning, transformation, and Calendar Table creation
- **Power Pivot** — Data Model, one-to-many relationship between datasets
- **DAX** — Calculated columns and measures (e.g. age groups, attend status, admission flag)
- **Pivot Tables** — Loaded from Data Model into existing sheets
- **Charts** — Area charts, bar charts, donut chart, sparklines
- **Slicers** — Interactive filtering on the dashboard



Raw Dataset Overview

| Column | Description |
|--------|-------------|
| Patient Id | Unique identifier |
| Patient Admission Date | Date and time of ER visit |
| Patient First Initial / Last Name | Patient name |
| Patient Gender | Male / Female |
| Patient Age | Age in years |
| Patient Race | Patient ethnicity |
| Department Referral | Department referred to (if any) |
| Patient Admission Flag | Whether patient was admitted |
| Patient Satisfaction Score | Score out of 10 (nullable) |
| Patient Waittime | Wait time in minutes |

**Total records:** 9,216 | **Time period:** 2023



 File Structure

| Sheet | Description |
|-------|-------------|
| `Pivot Report` | All pivot tables powering the dashboard |
| `Dashboard` | Interactive visual dashboard with charts and slicers |
| `Total ER Patients Count` | Daily trend — patient volume |
| `Avg. Wait Time Daily Trend` | Daily trend — average wait time |
| `Satisfaction Score Daily Trends` | Daily trend — satisfaction scores |

> **Note:** Raw and cleaned data were loaded directly into the **Power Pivot Data Model** via Power Query and are not visible as separate sheets. This is intentional — the Data Model stores and manages the data, powering all pivot tables and DAX calculations.



Data Model

A **one-to-many relationship** was built in Power Pivot between the two source datasets. See the data model screenshot --> uploaded



 Skills Demonstrated

- End-to-end data analyst project workflow
- Data cleaning and transformation with Power Query
- Relational data modelling (one-to-many) in Power Pivot
- DAX formula writing for calculated columns and measures
- Calendar Table creation from raw data
- Interactive dashboard design in Excel
- Data storytelling and insight generation



