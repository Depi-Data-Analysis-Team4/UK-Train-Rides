# UK Train Rides Analytics

An end-to-end data analytics project exploring UK railway ticket transactions and journey performance, with Python-based data preparation and a planned Microsoft Power BI dashboard.

## Project Name
UK Train Rides

## Project Idea
Analyze UK railway ticket transactions to understand journey demand, ticket-class preferences, route performance, punctuality, delays, cancellations, refunds, and ticket-price patterns. The project brief also calls for forecasting the number of rides for the following month, estimating the daily ticket-value outlook, and identifying expected demand across ticket classes.

The forecasting objectives are part of the project brief and must not be presented as completed until a forecasting model has been built and validated.

## Team Members
| Name | Role |
|---|---|
| Hessin Taha | Team Leader |
| Salma Sameh | Team Member |
| Yassin Athula | Team Member |
| Ziad Emam | Team Member |
| Ganna Amir | Team Member |

## Instructor
Mohamed Ahmed Saad

## Work Plan
1. **Data cleaning and preprocessing:** inspect the railway transaction source, profile missing values, standardize selected labels, parse dates and times, and prepare clean analytical outputs.
2. **Analysis questions and exploration:** analyze transaction volume, routes, ticket classes and types, purchase channels, payment methods, punctuality, delays, cancellations, refunds, and price patterns.
3. **Forecasting:** develop and validate a next-month ride-volume forecast, daily ticket-value outlook, and ticket-class demand analysis, subject to sufficient time coverage and documented assumptions.
4. **Power BI dashboard:** build an interactive report with KPIs, trend analysis, route and ticket breakdowns, filters, and clear metric definitions.
5. **Validation and presentation:** reconcile dashboard measures against independently calculated results, document limitations, and prepare the final presentation.

## Roles & Responsibilities
- **Hessin Taha — Team Leader:** coordinate the project, organize deliverables, track progress, and lead final integration.
- **Salma Sameh, Yassin Athula, Ziad Emam, and Ganna Amir — Team Members:** contribute to data preparation, analysis, dashboard development, validation, and documentation.
- Individual task ownership for each member has not yet been provided and should be updated when confirmed.

## KPIs
The available analysis report records the following transaction-level baseline:

| KPI | Observed result |
|---|---:|
| Ticket transactions | 31,653 |
| On-time transactions | 27,481 (86.82%) |
| Delayed transactions | 2,292 (7.24%) |
| Cancelled transactions | 1,880 (5.94%) |
| Refund requests | 1,118 (3.53%) |
| Average ticket Price field | 23.44 (currency not documented) |

Additional dashboard and forecasting KPIs:
- Total ticket transactions and monthly ride-volume trend.
- On-time, delay, and cancellation rates.
- Average delay minutes where actual and scheduled arrival timestamps are available.
- Refund-request count and rate.
- Transaction volume and demand by route, ticket class, and ticket type.
- Forecasted next-month rides and daily ticket-value outlook, once modelled and validated.

**Metric caution:** the source records ticket transactions, not unique train services. The sum of the Price field must not be labelled verified revenue because currency and accounting treatment are undocumented.

## Project Files
- `docs/project_summary.md` — detailed data scope, model structure, baseline findings, and limitations.
- `cleaning_pipeline.py` and prepared CSV/model outputs are part of the project working materials and can be added as repository assets in a subsequent upload.
- A native Power BI `.pbix` was not present in the located project artifacts; the analysis handoff report is not a deployed interactive dashboard.

## Data Scope & Limitations
- The located analysis covers 31,653 ticket transactions from 2024-01-01 through 2024-04-30.
- No train-service identifier is available, so counts and rates are transaction-level.
- The source does not document the currency or accounting treatment for Price; the sum is not verified revenue.
- Railcard nulls require confirmation from the data owner; they are retained as “Not recorded,” not assumed to mean “No railcard.”
- Some delay-reason labels were standardized using explicit mappings; these assumptions should be reviewed before official use.
- A native PBIX and interactive report behavior were not verified in the located artifacts.

## Tools
Python, pandas, NumPy, Microsoft Power BI.

---
Prepared for DEPI project submission.
