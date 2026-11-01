<div align="center">

# 🚆 UK Train Rides Analytics

**Turning railway transaction data into clear operational insights.**

![Python](https://img.shields.io/badge/Python-Data%20Analysis-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-Data%20Analysis-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-Database%20Queries-E34F26?style=for-the-badge&logo=databricks&logoColor=white)
![Status](https://img.shields.io/badge/DEPI-Data%20Analytics-8A2BE2?style=for-the-badge)

</div>

---

## 📌 Project Overview

UK Train Rides is a data analytics project focused on understanding railway ticket transactions and journey performance. The analysis explores travel demand, routes, ticket preferences, punctuality, delays, cancellations, refunds, and ticket-price patterns.

The project brief also asks for forecasting next-month ride volume, the daily ticket-value outlook, and demand across ticket classes. These are planned analytical deliverables and should only be marked complete after the forecasts are built and validated.

## 🎯 Project Objectives

- Examine transaction and journey trends over time.
- Identify popular routes, stations, ticket classes, and ticket types.
- Measure punctuality, delays, cancellations, and refund requests.
- Explore purchase channels and payment preferences.
- Prepare a reliable analytical model for Power BI reporting.
- Develop and validate the requested ride-volume and ticket-demand forecasts.

## 📊 Current Dataset Snapshot

| Metric | Observed result |
|---|---:|
| Ticket transactions | **31,653** |
| On-time transactions | **27,481 (86.82%)** |
| Delayed transactions | **2,292 (7.24%)** |
| Cancelled transactions | **1,880 (5.94%)** |
| Refund requests | **1,118 (3.53%)** |
| Average ticket Price field | **23.44** |

<sub>Coverage: 1 January 2024 – 30 April 2024. Counts are at ticket-transaction level, not unique train-service level. Currency is not documented, so the Price total is not presented as verified revenue.</sub>

## 🧭 Work Plan

| Phase | Main activities |
|---|---|
| 1. Data Preparation | Profile source data, handle missing values carefully, standardize selected labels, parse dates and times, and prepare clean outputs. |
| 2. Exploratory Analysis | Investigate routes, ticket types, ticket classes, purchase methods, payment methods, punctuality, delays, cancellations, and refunds. |
| 3. Forecasting | Build and validate next-month ride-volume, daily ticket-value, and ticket-class demand forecasts. |
| 4. Power BI Dashboard | Present key metrics, trends, route and ticket breakdowns, and interactive filters. |
| 5. Validation & Presentation | Reconcile dashboard measures, document assumptions, and prepare the final project presentation. |

## 👥 Team Members

| Name | Responsibility |
|---|---|
| Hessin Taha | Team Leader |
| Salma Sameh | Team Member |
| Yassin Athula | Team Member |
| Ziad Emam | Team Member |
| Ganna Amir | Team Member |

*Detailed individual task ownership can be added once confirmed by the team.*

## 👨‍🏫 Course Instructor

**Eng. Mohamed Ahmed Saad**

## 📈 Key Performance Indicators

- Total ticket transactions and monthly transaction trend.
- On-time, delay, and cancellation rates.
- Average delay minutes when valid scheduled and actual arrival times are available.
- Refund-request count and rate.
- Transaction volume by route, ticket class, and ticket type.
- Forecasted next-month rides and ticket-class demand, once validated.

## 🛠️ Tools & Technologies

- **Python** — data preparation, analysis, and validation.
- **Microsoft Power BI** — interactive dashboard and reporting.
- **Microsoft Excel** — spreadsheet-based data review and analysis.
- **Power Query** — data cleaning and transformation.
- **SQL** — querying and working with structured data.

## 📁 Project Structure

```text
UK-Train-Rides/
├── README.md
├── docs/
│   └── project_summary.md
├── data/
│   ├── source/
│   ├── clean/
│   └── dimensions/
├── reports/
└── powerbi/
```

*The structure above describes the intended organization. Only files actually committed to the repository should be considered submitted deliverables.*

## ⚠️ Data Notes & Limitations

- The available analysis covers four months only; it does not support reliable annual seasonality or year-over-year comparisons.
- No train-service identifier is available, so the analysis measures ticket transactions rather than unique train services.
- The currency and accounting treatment of the Price field are undocumented.
- Missing Railcard values are labelled **Not recorded**; they are not assumed to mean that a passenger had no Railcard.
- Standardized delay-reason labels use explicit mapping assumptions that should be reviewed with the data owner.
- The located handoff materials did not include a verified native Power BI `.pbix` file.

## 📄 Supporting Documentation

- [Project Summary](docs/project_summary.md)

---

<div align="center">

**DEPI · Data Analytics Project**

</div>
