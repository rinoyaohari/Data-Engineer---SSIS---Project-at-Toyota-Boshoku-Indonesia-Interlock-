# 🚗 PT Toyota Boshoku Indonesia – Power BI Reporting Integration Project

## Project Overview
This project was developed for **PT Toyota Boshoku Indonesia** to support enterprise-level **Power BI reporting** by integrating data from multiple SAP modules and Mendix applications into a centralized reporting platform.

The project utilized output files generated from **SAP ABAP Programs** across several modules including:
- MM (Material Management)
- CO (Controlling)
- SD (Sales & Distribution)
- PP (Production Planning)

Additional data sources were also integrated from **Mendix** applications. All generated TXT files were stored in **AL11 shared folders** and processed using **SSIS (SQL Server Integration Services)** before being consumed by Power BI.

I worked primarily as a **Data Engineer**, while also supporting the **Project Manager** in project coordination, reporting, and delivery activities.

---

# Responsibilities

## Data Engineering Role

### Data Source Integration
- Integrated multiple SAP module outputs:
  - MM
  - CO
  - SD
  - PP
- Integrated additional TXT output from Mendix applications
- Retrieved all source files from AL11 shared folder

### ETL Development (SSIS)
- Built SSIS packages to process TXT files
- Managed source-to-reporting data flow
- Processed and standardized source data for reporting readiness
- Prepared data source structure for Power BI consumption

### Job Scheduling & Automation
- Configured automated ETL job schedules
- Maintained recurring SSIS execution process
- Ensured stable and reliable daily data refresh process

### Reporting Data Preparation
- Delivered processed datasets for Power BI dashboards
- Ensured data consistency and availability for reporting layer

---

## Project Management Support

### Project Coordination
- Assisted Project Manager in managing project activities
- Helped maintain project communication and coordination

### Documentation & Reporting
- Created and maintained weekly project reports
- Assisted in preparing project progress updates

### Meeting & Testing Support
- Scheduled and organized project meetings
- Moderated:
  - SIT (System Integration Testing)
  - UAT (User Acceptance Testing)

### Project Delivery
- Supported project handover and delivery process to customer
- Coordinated communication between technical team and stakeholders

---

# Technology Stack

| Technology | Purpose |
|---|---|
| SAP MM / CO / SD / PP | Source ERP Modules |
| ABAP | SAP Data Extraction Programs |
| Mendix | Additional Data Source |
| AL11 Shared Folder | TXT File Repository |
| SSIS | ETL Development |
| SQL Server | Reporting Data Storage |
| Power BI | Reporting & Dashboard |
| SQL | Data Processing |

---

# Project Workflow

```mermaid
flowchart TD

A[Business Requirement]
B[ABAP Program Output]
C[Mendix Output]
D[TXT Files in AL11]
E[SSIS ETL Process]
F[Data Transformation]
G[SQL Server Reporting Source]
H[Power BI Dashboard]
I[Daily Job Schedule]
J[SIT & UAT Support]
K[Weekly Project Report]
L[Project Delivery]

A --> B
A --> C
B --> D
C --> D
D --> E
E --> F
F --> G
G --> H
E --> I
A --> K
J --> L
K --> L
H --> L
