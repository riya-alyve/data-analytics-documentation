<b><h1>Data Analytics Documentation Repository</h1></b>

<b>Purpose</b><br>
This repository serves as the central documentation hub for all published reports, queries, and logic alignment across the Data Analytics team.
It ensures consistency, transparency, and version control for all data-related assets.


**Repository Structure** <br>
data-analytics-documentation/<br>
│<br>
├── reports: Documentation for published reports<br>
├── queries: SQL queries with logic explanations<br>
├── data-source: Overview of databases, tables & joins<br>
└── guidelines: Standards for documentation & naming<br>


**How to Use This Repository** <br><br>
**1. Document a New Report**

Create a new Markdown file under reports/ using the format:
reports/<report_name>.md

Use the following template:   <br>
-> Report: <Report Name>         <br>
-> Owner: <Your Name>            <br>
-> Module: <Module or Domain>    <br>
-> Last Updated: <Date>          <br>
-> Status: Draft / Published     <br>

**Objective**
<br>Briefly describe the purpose of the report and the key business questions it answers.

**Data Sources**
| Source Name | Type (DB, API, etc.) | Tables/Views Used | Description |
|--------------|----------------------|-------------------|--------------|
| example_db   | Database             | sales_data, users | Main source of sales transactions |

**Key Metrics & Calculations** <br>
List the main KPIs or metrics displayed in the report, including formulas or logic if applicable.

| Metric Name | Definition / Formula | Notes |
|--------------|----------------------|-------|
| Revenue | SUM(sales_amount) | Excludes test transactions |

**Query Reference** <br>
Link to the corresponding query or logic file:  
[`queries/<module>/<query_name>.sql`](../queries/<module>/<query_name>.sql)

**Visualization / Dashboard** <br>
- Dashboard Link: [Add URL if applicable]  
- Screenshot (optional): *Embed or attach here*

**Validation Notes** <br>
Mention any data checks, validation results, or alignment feedback from the backend or product teams.

**Change Log**
| Date | Updated By | Description |
|------|-------------|-------------|
| YYYY-MM-DD | Name | Initial documentation created |
| YYYY-MM-DD | Name | Logic updated for new metric definition |


**2. Add or Update a Query**

Place SQL files under queries/<module_name>/<br>
Add a companion Markdown file (e.g., logic_explanation.md) to explain joins, filters, and business rules.

**3. Follow Documentation Standards**

Refer to the guidelines/documentation_guidelines.md for:
- Naming conventions
- Required metadata
- Versioning and review process

<br> **Collaboration**<br>
Branching: Create a new branch for documentation updates.<br>
Review: Submit a pull request for peer review before merging.<br>
Tags: Use tags like report, query, or data-source for easy navigation.
