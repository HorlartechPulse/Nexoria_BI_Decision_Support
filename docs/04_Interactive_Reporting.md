# Interactive Reporting Design — Executive KPI Dashboard

## Theme (match reference UI)

| Token | Value |
|-------|--------|
| Background | Deep purple `#1A0F2E` / `#24123D` |
| Cards | `#2D1B4E` |
| Accent bars | Lavender → cyan gradient |
| Positive variance | `#12B886` |
| Font | Segoe UI / Inter |

## Page: Executive Summary

### KPI card row (6)

1. Actual Revenue + vs Budget %  
2. Actual EBITDA + vs Budget %  
3. Gross Margin % + vs Budget pp  
4. Actual Active Customers + YoY %  
5. Headcount Actual + vs Budget  
6. System Uptime + vs Budget pp  

### Visual row 2

| Visual | Fields |
|--------|--------|
| Revenue Performance vs Budget & Forecast | Clustered columns + line by Year; Actual/Budget/Forecast |
| Revenue & EBITDA by Division | Clustered columns; drill-through to Product Line |
| EBITDA Trend vs Budget | Columns Actual + line/budget by Year |

### Visual row 3

| Visual | Fields |
|--------|--------|
| Gross Margin % Monthly Trend vs Budget | Column or combo by MonthYear |
| Global Revenue Distribution | Map bubble by DimRegion (Lat/Lon), size = Revenue |

### Filters / chrome

- Tabs: Executive Summary · Regional Performance · Org & Operations  
- Executive Owner: COO · CRO · CTO (filters Division via OwnerRole)  
- Reset filters button (bookmark)

## Page: Regional Performance

- Revenue ranking by region  
- Margin by region  
- Customer density  

## Page: Org & Operations

- Headcount by division vs budget  
- Uptime trend  
- EBITDA margin by operations product lines  

## Build options

1. **Power BI Desktop** — import Excel, model relationships, DAX from `/dax`, implement pages above.  
2. **Excel** — use `KPI_Snapshot` + charts as offline executive pack.  
