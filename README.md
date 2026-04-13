# 📊 D365-FO-Budget-Report-DAX-BI
Sample Power BI **Budget vs Expenditure report** for Microsoft D365 Finance & Operations (FO)  using standardized **Anonymized Sample DAX Patterns**.

This repository is dedicated to learning **DAX Design Techniques and Modeling Patterns**.
***
## 🎯 Purpose of This Repository

*   Demonstrate **Enterprise‑Grade DAX Patterns** for budget reporting
*   Provide reference implementations for:
    *   Budget ID wise Budget and Expenditure Summaries
    *   Budget Aggregation
    *   Cross‑Table filtering using `TREATAS`
*   Share reusable **Power BI & DAX Best Practices** in a privacy‑safe manner

This repository is intended for:

*   Power BI developers
*   BI architects
*   Finance & ERP reporting professionals
*   D365 FO reporting practitioners
***

## 🧠 What This Repository Demonstrates

*   ✅ Use of `SUMMARIZE` and `ADDCOLUMNS` for dimensional aggregation
*   ✅ Use of `TREATAS` for applying filters across fact tables
*   ✅ Budget line item counting and aggregation patterns
*   ✅ Filtering out zero‑value budget records
*   ✅ Clear separation of **dimension** and **fact** logic

All examples follow **star‑schema‑friendly** DAX patterns.

***

## 🧱 Logical Data Model (Abstracted)

The DAX patterns assume a simplified star schema:

***

DimBudgetTable
    |
    | (1:N via BudgetID)
    |
FactBudgetLineTable

***


### Abstracted Tables

*   `DimBudgetTable` → Budget master / header data
*   `FactBudgetLineTable` → Budget Category or line‑level data

> Note: Actual table and column names are intentionally anonymized.

***

## 🔍 Example Use Case

The included DAX demonstrates how to generate a **Budget Summary** that:

*   Groups by budget ID and date range
*   Counts related Budget Line Items
*   Calculates Budget ID wise Total Budgets and Total Expenditures 
*   Excludes zero‑value Budget Entries

This pattern is commonly used in:

*   Budget dashboards
*   Finance oversight reports
*   Management summary views

***

## 🔐 Data Privacy & Confidentiality

⚠️ **IMPORTANT**

*   This repository contains **no real data**
*   No actual organization's budget figures, project codes, donors, or cost centers are used
*   All identifiers are **synthetic and illustrative**
*   Shared strictly for **technical knowledge exchange**

For details, see:  
📄 docs/data\_privacy\_note.md

***

## 📁 Repository Structure

    ├── dax/
    │   └── budget_summary_sample.dax
    │
    ├── docs/
    │   └── data_privacy_note.md
    │
    ├── README.md

***

## 🚀 How to Use This Repository

1.  Review the DAX patterns in the `dax/` folder
2.  Adapt the logic to your own **Budget table and fact tables**
3.  Replace abstracted names with your model objects
4.  Ensure any real implementation complies with your organization’s data governance and security policies

***

## 👤 Author

**Syfur Rahaman Shohag**  
D365 FO Technical Expert | CE | Power Platform | Solution Architect |
FinTech & Banking | Trading Community | HealthTech & Research

Specializing in D365 FO Technical, Power BI, DAX, and D365 Finance reporting

***

## 🤝 Disclaimer

This repository represents **personal technical work** and learning samples.  
It does not represent official systems, datasets, or reports of any organization.

***
