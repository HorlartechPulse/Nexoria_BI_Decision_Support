# KPI Definitions & Calculation Rules

| KPI | Business definition | Formula / rule | Grain | Good direction |
|-----|---------------------|----------------|-------|----------------|
| **Actual Revenue** | Recognised management revenue | `SUM(Revenue)` where Scenario=Actual | Month × Div × PL × Region | Higher vs Budget |
| **Actual EBITDA** | Operating profit proxy | `SUM(EBITDA)` Scenario=Actual | same | Higher vs Budget |
| **Gross Margin %** | Profitability after direct cost | `(Revenue − COGS) / Revenue` | same | Higher vs Budget |
| **Active Customers** | Customers with qualifying activity | Distinct / period-active count from CRM | Month × Region | Higher YoY |
| **Headcount Actual** | Filled FTE / headcount | `SUM/AVG(Headcount)` Actual | Month × Division | Near Budget |
| **System Uptime** | Platform availability | `AVERAGE(SystemUptime)` | Month × Tech | ≥ Budget/target (~0.99) |

## Variance measures

| Measure | Rule |
|---------|------|
| Revenue vs Budget % | `(Actual − Budget) / Budget` |
| EBITDA vs Budget % | `(Actual − Budget) / Budget` |
| Gross Margin vs Budget (pp) | `Actual GM% − Budget GM%` |
| Headcount Variance | `(Actual − Budget) / Budget` |
| Uptime Variance (pp) | `Actual − Budget` |

## Targets illustrated on Executive Summary (reference design)

| KPI | Illustrative value |
|-----|-------------------|
| Actual Revenue | ~$20bn |
| Actual EBITDA | ~$5bn |
| Gross Margin | ~55% |
| Active Customers | ~187,015 |
| Headcount | ~53,775 |
| System Uptime | 1.00 (rounded) |

*Sample model totals are generated to approximate this executive scale.*
