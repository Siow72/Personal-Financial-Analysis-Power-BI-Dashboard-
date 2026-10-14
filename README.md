# Personal Finance Dashboard

An interactive **Power BI** dashboard for tracking personal finances, exploring spending behaviour, monitoring budgets, and understanding monthly financial performance. The project uses **Microsoft Excel** for financial recordkeeping and **Power BI, Power Query, and DAX** for modelling, calculations, and visual reporting.

> **Project status:** In development. This README describes the current design and features discussed so far; screenshots and the latest `.pbix` release will be updated as pages are finalised.

## Overview

The dashboard aims to turn everyday financial transactions into clear, actionable insights. It combines monthly summaries with detailed analysis so users can see where money goes, how spending compares with previous months, and how closely actual expenses follow planned budgets.

**Design direction:** a dark charcoal/navy theme with sky-blue/aqua accents and amber highlights, consistent KPI cards, and month-based reporting.

## Features

- **Monthly filtering:** Review a selected month with comparisons to the previous month.
- **Financial KPIs:** Track income, expenses, net cash flow, transaction activity, and other financial indicators.
- **Spending analysis:** Explore expense categories, spending patterns, and changes across months.
- **Transaction details:** Inspect transaction history and identify the largest individual expense within each category.
- **Budget monitoring:** Compare planned budgets against actual spending, including budget usage and remaining amounts.
- **Dynamic DAX measures:** Support time-aware reporting, comparison text, and conditional status indicators.
- **Interactive reporting:** Use Power BI slicers, charts, KPI cards, and tooltips to navigate financial data.

## Dashboard Pages

| Page | Purpose | Development status |
| --- | --- | --- |
| **Overview** | High-level monthly financial snapshot and key metrics | In development |
| **Spending Analysis I** | Understand where money goes through category and spending-pattern analysis | In development |
| **Spending Analysis II** | Review transaction history, spending frequency, and largest transactions by category | In development |
| **Cash Flow** | Examine monthly inflows, outflows, and net cash flow | In development |
| **Budget** | Compare category-level budgets with actual spending and remaining balances | In development |
| **Net Worth** | Follow changes in assets, liabilities, and net worth | Planned / evolving |
| **Accounts** | Review balances across bank accounts and e-wallets | Planned |
| **Goals** | Monitor progress toward savings and other financial goals | Planned |

*Statuses are intentionally conservative until the latest report file and visuals are verified.*

## Technology Stack

| Tool | Role |
| --- | --- |
| **Microsoft Excel** | Source data entry and storage |
| **Power BI Desktop** | Data modelling and interactive visualisation |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Measures, time comparisons, and KPI logic |

## Data Structure

The Excel workbook is designed around the following core sheets:

| Sheet | Description |
| --- | --- |
| `Accounts` | Account identifiers and account information |
| `Transactions` | Income, expenses, transfers, dates, categories, and transaction details |
| `NetWorth` | Periodic net worth records |
| `Budget` | Planned spending by category and period |
| `Goals` | Financial goals and targets |
| `MonthlySnapshot` | Monthly financial snapshots where applicable |

Power BI also uses a calendar/date table for month selection and time-based comparisons. The actual table and field names may differ slightly between workbook versions.

## Repository Structure

```text
Personal-Finance-Dashboard/
├── dashboard/
│   └── Personal_Finance_Dashboard.pbix
├── data/
│   └── Sample_Finance_Data.xlsx
├── screenshots/
│   ├── overview.png
│   ├── spending_analysis_1.png
│   ├── spending_analysis_2.png
│   ├── cash_flow.png
│   └── budget.png
├── docs/
│   ├── data_model.md
│   └── dax_measures.md
├── .gitignore
├── LICENSE
└── README.md
```

> The structure above is a **suggested layout**. Add files and screenshots as they become ready; links are intentionally omitted until those assets exist.

## Getting Started

1. Install **Power BI Desktop**.
2. Clone or download this repository.
3. Open the `.pbix` report in the `dashboard/` directory **once it has been published**.
4. If prompted, update the Power Query data-source path to the sample workbook in `data/`.
5. Refresh the dataset, then explore the report using the month selector and visual filters.

## Development Roadmap

- [x] Establish the Excel-based finance data structure.
- [x] Define a navy/charcoal visual theme and accent palette.
- [x] Develop selected-month and previous-month DAX logic.
- [ ] Finalise and validate the Overview, Spending Analysis, Cash Flow, and Budget pages.
- [ ] Complete Net Worth, Accounts, and Goals reporting.
- [ ] Test filters, category handling, and measures across months with no transactions.
- [ ] Publish anonymised sample data, screenshots, and a reproducible report file.
- [ ] Document the final data model and key DAX measures.

## Data Privacy

**No actual personal financial information should be committed to this public repository.** Any publicly shared Excel workbook and Power BI report should use synthetic or anonymised data. Remember that a `.pbix` file can contain imported rows even when its original Excel source is not included.

## License

This project is intended to be shared under the **MIT License** if a `LICENSE` file is added to the repository. Until a license is actually included, do not assume permission to reuse the code or assets.
