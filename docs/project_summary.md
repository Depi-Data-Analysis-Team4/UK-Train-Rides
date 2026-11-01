# UK Train Rides — Project Summary

## Data scope
The located UK Train Rides analysis covers 31,653 source rows and 31,653 distinct transaction IDs across 2024-01-01 to 2024-04-30. The fact-table grain is one row per ticket transaction, not one row per unique train service.

## Baseline findings
- On time: 27,481 transactions (86.82%).
- Delayed: 2,292 transactions (7.24%).
- Cancelled: 1,880 transactions (5.94%).
- Refund requests: 1,118 (3.53%).
- Average Price field: 23.44; currency is not documented.

These are observed descriptive results, not forecasts. The sum of Price is not described as verified revenue.

## Analytical model
The prepared model contains one transaction fact table and six dimensions:
- DimDate — 121 rows.
- DimRoute — 65 rows.
- DimTicket — 24 rows.
- DimPurchase — 6 rows.
- DimJourneyStatus — 3 rows.
- DimDelayReason — 6 rows.

Use single-direction, one-to-many relationships from each dimension to the fact table. The audit reports all dimension keys resolving for all fact rows.

## Data-quality notes
- Railcard is missing on 20,918 rows (66.09%). Nulls are represented as “Not recorded”; they are not assumed to mean no railcard.
- Actual Arrival Time is missing on 1,880 rows (5.94%), aligning with cancelled transactions in the source profile.
- Reason for Delay is missing on 27,481 rows (86.82%), aligning with on-time transactions in the source profile.
- No exact duplicate rows or duplicate transaction IDs were reported in the audit.
- Date parsing and fact/dimension validation passed the 20 recorded automated checks.

## Forecasting and Power BI status
The project brief calls for a next-month ride forecast, daily ticket-value outlook, and ticket-class demand forecast. The located report does not establish that these forecasts have been trained or validated. It also states that no native PBIX was created and that report navigation, bookmarks, slicers, reset behavior, and DAX execution were not tested in Power BI Desktop.

## Important limitations
- Only four months of journey history are available, so annual seasonality and year-over-year analysis are not supported.
- No train-service ID is available.
- Currency and accounting treatment are undocumented.
- Delay-reason mappings and Railcard null semantics require owner confirmation.
