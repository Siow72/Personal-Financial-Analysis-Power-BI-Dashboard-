# Personal Finance Dashboard

**An interactive personal finance analytics dashboard built with Microsoft Power BI.**

This project brings everyday financial records into one place to help users understand their spending habits, monitor cash flow, evaluate budgets, track travel expenses, and follow progress toward savings goals. It focuses on turning raw transaction data into clear, actionable visuals through interactive reports and custom DAX measures.

> **Project status:** Work in progress — dashboard features and layouts are being refined.

## Dashboard Preview

![Financial overview dashboard](screenshots/Overview.png)

*Screenshot placeholder: add an image named `overview.png` in `docs/screenshots/` to display the dashboard here.*

## Dashboard Pages

| Page | Purpose | Highlights |
| --- | --- | --- |
| **Overview** | Provide an at-a-glance picture of personal finances | Financial KPIs, high-level summaries, and navigation |
| **Spending Analysis I** | Understand where money goes | Spending categories, expense patterns, and breakdowns |
| **Spending Analysis II** | Explore individual expenses in greater detail | Transaction history, category-level largest expenses, and spending frequency |
| **Cash Flow** | Understand incoming and outgoing money | Income, expenses, net cash flow, and period comparisons |
| **Budget** | Evaluate planned spending against actual spending | Budget utilization, remaining budget, and category comparisons |
| **Trip and Budget Analysis** | Track travel finances by trip | Trip selection, trip status, budgets, and spending analysis |
| **Goal** | Track progress toward financial goals | Goal selection, saving progress, and contribution trends |

The PBIX currently also contains a page named **Page 1**; this README focuses on the seven named reporting pages.

## Key Features

- **Interactive filtering:** Explore relevant financial information using date, category, trip, and goal selections.
- **Dynamic KPI calculations:** DAX measures respond to filter context and selected reporting periods.
- **Period-over-period comparisons:** Compare current and previous month values to understand changes.
- **Spending insights:** Analyze category performance, transaction details, and spending behavior.
- **Budget monitoring:** Compare budgets with actual expenses and identify overspending.
- **Trip expense tracking:** Review travel-related expenditure through trip-specific reporting.
- **Savings goal tracking:** Monitor financial targets and related contributions.
- **Consistent dashboard design:** A dark navy interface with blue and amber accents, navigation elements, and supporting icons.

## Tools and Technologies

| Tool | Usage |
| --- | --- |
| **Microsoft Power BI Desktop** | Dashboard development, data modeling, and visualizations |
| **DAX (Data Analysis Expressions)** | Calculated measures, period logic, dynamic labels, and KPIs |
| **Power Query** | Data import and preparation |
| **Microsoft Excel** | Source data and example financial records |
| **GitHub** | Version history, documentation, and portfolio presentation |

## Data Model

The dashboard uses financial records organized around several subject areas:

- **Transaction:** Dated financial activity, including transaction amount, type, category, and optional trip/goal references.
- **Budget:** Planned spending used to compare budgets against actual expenses.
- **Trip Budget:** Trip-specific budget and category information.
- **Goal:** Savings goals and related metadata.
- **DateTable:** Calendar attributes for time filtering, grouping, and analysis.

The exact relationship configuration and field definitions should be documented in [`docs/data-model.md`](docs/data-model.md) once finalized.

## DAX and Analytical Logic

Custom DAX measures support report interactions and financial analysis, including:

- Selected-month and previous-month calculations
- Income and expense summaries
- Month-over-month changes and formatted indicators
- Spending frequency and category analysis
- Budget-used and budget-remaining calculations
- Trip-specific filtering and status-dependent visuals
- Goal contribution and savings trends

For implementation notes and selected formulas, see [`docs/dax-measures.md`](docs/dax-measures.md) when added.

## Getting Started

1. **Clone or download** this repository.
   ```bash
   git clone https://github.com/Siow72/personal-finance-dashboard.git
   ```
2. **Install Power BI Desktop** if you do not already have it.
3. **Open** `dashboard/Personal-Finance-Dashboard.pbix` in Power BI Desktop.
4. **Configure the data source** in Power Query if the workbook path does not match your machine. When a sample workbook is available, point the queries to `data/sample/Money-Tracker-Sample.xlsx` and adapt the column mappings as needed.
5. **Refresh the report**, then use the dashboard's slicers and navigation to explore the visuals.

**Note:** Downloaded PBIX files may contain existing report data. Review the file and configure it for sample data **before publicly sharing the PBIX**.

## Future Improvements

- [ ] Finalize and test the Goal dashboard visuals.
- [ ] Refine goal contribution calculations and relationships.
- [ ] Add a realistic, privacy-safe sample Excel dataset.
- [ ] Upload screenshots of each dashboard page.
- [ ] Document the model relationships and important DAX measures.
- [ ] Add instructions for switching to the example dataset.
- [ ] Test filters, edge cases, and reports with missing data.
- [ ] Improve tooltip details and visual consistency.

## Privacy and Data Disclaimer

This repository is intended for **personal learning and portfolio demonstration**. Only fictional, anonymized, or explicitly approved datasets should be uploaded. Do not commit personal financial records, bank account information, credentials, or any other sensitive data.

The dashboard is a financial tracking and analysis tool, not professional financial advice.

## License

A license has not yet been selected. Add a `LICENSE` file once you decide how others may use, copy, and modify this project.

---

**Built with Microsoft Power BI, DAX, and Excel.**
