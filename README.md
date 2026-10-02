# Nexoria Group — BI Decision Support System

**Case study:** Management reporting and performance monitoring  
**Dashboard concept:** Executive KPI Dashboard (Revenue, EBITDA, Margin, Customers, Headcount, Uptime)

---

## Deliverables

| Deliverable | Path |
|-------------|------|
| Business requirements | `docs/01_Business_Requirements.md` |
| KPI definitions & rules | `docs/02_KPI_Definitions.md` |
| Dimensional data model | `docs/03_Dimensional_Model.md` |
| Data dictionary + source | `data/Nexoria_BI_Source.xlsx` |
| Interactive reporting design | `docs/04_Interactive_Reporting.md` |
| DAX measures | `dax/measures.dax` |
| Recommendations (metric-tied) | `docs/05_Recommendations.md` |

---

## What’s in the data model

- **Dims:** Date, Division (Commercial / Technology / Operations), Product Line, Region (global), Scenario (Actual / Budget / Forecast)
- **Fact:** Monthly Revenue, COGS, EBITDA, Active Customers, Headcount, System Uptime
- **Sample scale:** ~$20bn revenue · ~$5bn EBITDA · ~55% gross margin (generated to match executive UI)

---

## How to use

### Excel (immediate)

Open `data/Nexoria_BI_Source.xlsx` → sheet **KPI_Snapshot** for cards + charts.

### Power BI (interactive)

1. Import Excel tables  
2. Build relationships (star schema)  
3. Add DAX from `dax/measures.dax`  
4. Implement pages per `docs/04_Interactive_Reporting.md` (purple executive theme)

---

## Executive owner lens

| Button | Filters divisions |
|--------|-------------------|
| CRO | Commercial |
| CTO | Technology |
| COO | Operations |

---

## Author

**Abdulwaheed Toheeb Olanrewaju**  
Portfolio — BI · Decision Support · Executive Reporting
