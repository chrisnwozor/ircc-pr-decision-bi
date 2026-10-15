# IRCC PR Decision Intelligence System

### End-to-End Business Intelligence & Data Warehousing Project

**Technologies:** SQL Server | SSIS | SSAS | SSRS | Power BI | SQL | ETL | Dimensional Modelling

**Project Status:** In Development

## Project Overview

The IRCC PR Decision Intelligence System is a personal Business Intelligence and Data Warehousing project designed to transform publicly available Canadian immigration data into structured, accessible, and meaningful insights.

The project focuses on building a data pipeline that extracts, transforms, stores, models, and visualizes immigration-related information using Microsoft Business Intelligence technologies.

The goal is to help users explore historical immigration trends while demonstrating real-world data engineering, analytical modelling, and reporting techniques.

## Business Problem

Canadian immigration information is distributed across multiple datasets and reports. Comparing immigration programs, invitation trends, provinces, and Comprehensive Ranking System (CRS) score distributions can be challenging.

This project explores how a centralized data warehouse and interactive reporting system can make historical immigration information easier to understand.

**Key analytical questions include:**

- How have immigration invitation trends changed over time?
- How do immigration programs compare across reporting years?
- What CRS score ranges appear in historical invitation data?
- How do reported totals vary across Canadian provinces?
- How can immigration datasets be integrated into a consistent reporting model?

## Technology Stack

| Technology | Purpose |
|---|---|
| SQL Server | Data storage, staging, and warehousing |
| SSIS | ETL pipelines and data integration |
| SSAS | Analytical and semantic modelling |
| SSRS | Structured and paginated reporting |
| Power BI | Interactive dashboards and visualization |
| SQL | Data transformation, validation, and analysis |
| Visual Studio | BI solution development |
| GitHub | Version control and project documentation |

## System Architecture

The project follows a traditional Microsoft Business Intelligence architecture.

**1. Data Sources**

Publicly available IRCC immigration datasets provide the source information for analytical reporting.

↓

**2. Data Integration — SSIS**

SSIS packages support data extraction, cleaning, transformation, and loading into SQL Server.

↓

**3. Data Warehouse — SQL Server**

Structured staging, dimension, and fact tables support consistent analytical reporting.

↓

**4. Analytical Model — SSAS**

A semantic model organizes business measures and dimensions for analysis.

↓

**5. Reporting — SSRS & Power BI**

SSRS and Power BI provide reporting and interactive visualizations.

## Data Warehouse Design

The analytical model uses dimensional modelling concepts, separating descriptive information into dimension tables and numerical measurements into fact tables.

**Dimensions include:**

- Dim Province
- Dim Year
- Dim Program
- Dim Score Range
- Dim Occupation
- Dim Education Level
- Dim Invitation Category

**Reporting fact areas include:**

- ITA Score
- Occupation
- Education
- Destination

This structure supports filtering, aggregation, and comparisons across reporting dimensions.

## Data Engineering Workflow

The development process covers several core data engineering activities:

1. **Data ingestion:** Organizing and loading source datasets.
2. **Data cleaning:** Addressing inconsistent values, missing information, and data type issues.
3. **Transformation:** Preparing data for reporting and analysis.
4. **Data warehousing:** Structuring analytical tables in SQL Server.
5. **Dimensional modelling:** Organizing facts and dimensions.
6. **Semantic modelling:** Exposing reusable analytical measures.
7. **Visualization:** Creating reports and dashboards that communicate useful insights.

## Power BI Dashboard

The Power BI reporting work includes:

**Program Trends**

Historical reporting comparisons across immigration programs and years.

**Provincial Analysis**

Geographic visualization and comparisons of reported totals across Canadian provinces and territories.

**CRS Score Distribution**

Analysis of reported data across CRS score ranges.

**Reporting Trends**

Time-based analysis of historical immigration statistics.

The dashboard is developed in Power BI Desktop. Power BI Service deployment and connectivity are still being configured.

## Repository Structure

The repository currently contains:

- **IRCC_ETL/** — SSIS ETL project files.
- **raw/** — Source data files used during development.
- **.gitignore** — Git tracking exclusions.

Additional SQL scripts, analytical models, reports, dashboard files, and documentation may be added as development continues.

## Project Development Status

This is an evolving portfolio project.

Current development areas include SQL Server data preparation, ETL workflows, dimensional modelling, SSAS analysis, SSRS reporting, and Power BI visualization.

**Planned improvements:**

- Strengthen automated data quality checks.
- Improve ETL error handling and logging.
- Add more reproducible deployment instructions.
- Expand dashboard documentation and screenshots.
- Improve cloud accessibility and report deployment.
- Explore cloud-based data engineering architectures.

## What I'm Learning

Building this project is helping me develop practical skills in:

- Designing ETL pipelines.
- Building and maintaining relational data warehouses.
- Applying dimensional modelling principles.
- Creating analytical models and reusable measures.
- Validating data quality across transformation stages.
- Building reports for business decision support.
- Troubleshooting connectivity, deployment, and reporting issues.

It also reinforces the importance of understanding the entire data lifecycle rather than focusing only on visualizations.

## Data Sources

The project uses publicly available Canadian immigration reporting information.

**Primary reference:** [Immigration, Refugees and Citizenship Canada (IRCC)](https://www.canada.ca/en/immigration-refugees-citizenship.html)

## Important Disclaimer

This is an independent educational and portfolio project. It is not affiliated with or endorsed by Immigration, Refugees and Citizenship Canada.

Historical immigration statistics do not guarantee future invitations, permanent residence eligibility, or application outcomes. The dashboards should not be treated as official immigration advice or individualized eligibility assessments.

## Author

Developed as a hands-on Business Intelligence and Data Engineering portfolio project.

**GitHub:** [chrisnwozor](https://github.com/chrisnwozor)

**LinkedIn:** [Christopher Nwozor](https://www.linkedin.com/in/christophernwozor/)

---

*Turning raw data into structured information, reliable reporting, and actionable insights.*
