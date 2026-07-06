# Production Efficiency & Cost Optimization Dashboard

## Overview

This project analyzes a simulated manufacturing dataset to identify production inefficiencies, downtime patterns, defect issues, and profitability differences across production lines, shifts, and product types.

The objective was to build a data-driven operations dashboard using Excel and Power BI, then estimate the financial impact of reducing downtime in the weakest production area.

## Project Objective

The main goals of this project were to:

- Analyze production efficiency across production lines
- Identify downtime and defect-related bottlenecks
- Compare profitability by line, shift, month, and product type
- Build an Excel dashboard for operational analysis
- Build an interactive Power BI dashboard for executive reporting
- Estimate potential recovered profit from reducing downtime

## Dataset Overview

The dataset contains 1,656 production records covering:

- 3 production lines
- 3 shifts
- 3 product types
- July–December 2026 production period

Main fields include:

- Planned Production
- Actual Production
- Defective Units
- Good Units
- Downtime Minutes
- Revenue
- Total Cost
- Profit
- Production Efficiency
- Defect Rate
- Profit Margin
- Cost per Good Unit

## Key KPIs

The following KPIs were calculated and analyzed:

- Good Units = Actual Production - Defective Units
- Production Efficiency = Actual Production / Planned Production
- Defect Rate = Defective Units / Actual Production
- Downtime Rate = Downtime Minutes / 480
- Revenue = Good Units × Selling Price per Unit
- Profit = Revenue - Total Cost
- Profit Margin = Profit / Revenue
- Cost per Good Unit = Total Cost / Good Units
- Good Units per Operating Minute = Good Units / Operating Minutes
- Profit per Good Unit = Profit / Good Units

## Tools Used

- Microsoft Excel
- Excel Tables
- PivotTables
- PivotCharts
- Power BI
- Power Query
- DAX Measures
- Dashboard Design
- Executive Reporting

## Dashboard Preview

![Power BI Dashboard](images/powerbi-dashboard.png)

## Key Findings

- Line 2 was identified as the weakest production line, with the lowest average production efficiency, highest average downtime, and lowest total profit.
- Line 3 was the strongest production line, with the highest average efficiency and highest total profit.
- Product B had the highest average defect rate, indicating a quality issue.
- Product C had the highest average profit margin.
- Monthly profit remained relatively stable, but November showed the lowest profit during the analysis period.
- Line 2 Night shift was identified as the main bottleneck.

## Savings Opportunity

A savings opportunity model was created for Line 2 Night shift.

The model compares Line 2 Night shift downtime with the factory average downtime and estimates the profit that could be recovered if downtime were reduced to the average level.

Estimated recovered profit:

**₺55.6K over the 6-month period**

Formula used:

```text
Estimated Recovered Profit =
Recoverable Minutes × Avg Good Units per Operating Minute × Avg Profit per Good Unit × Number of Shifts
