# financial-due-diligence-analytics-platform

## Overview
simulates how transaction advisory and private equity analytics teams process fragmented financial and operational datasets during pre-acquisition due diligence.

## Tech Stack
- Activepieces
- DuckDB
- SQL
- dbt
- Power BI
- Git & GitHub

## Business Problem
A private equity firm is evaluating the acquisition of a multi-region retail business whose financial and operational data is fragmented across disconnected CSV exports, ERP reports, and invoice ledgers.

## Project Architecture
`Raw CSVs
   ↓
DuckDB Analytical Processing
   ↓
dbt Financial Data Models
   ↓
Power BI Executive Dashboard
   ↓
Automated Monitoring via Activepieces`

## Core Analytics Capabilities
- Rolling LTM revenue analysis
- Revenue concentration risk detection
- EBITDA trend monitoring
- DSO aging calculations
- Customer profitability segmentation
- Regional margin analysis
- Automated financial anomaly alerts

## Key Metrics
✅ LTM Revenue
✅ EBITDA Margin
✅ Revenue Concentration %
✅ Gross Margin Trend
✅ DSO
✅ Customer Retention
✅ Working Capital Health
✅ Top Client Dependency
✅ Profitability by Region
✅ Invoice Aging
