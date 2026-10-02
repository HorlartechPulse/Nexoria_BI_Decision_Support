# Business Requirements — Nexoria Group Executive DSS

## 1. Purpose

Provide the **Executive Leadership Team** (CEO, COO, CRO, CTO, CFO) with a single decision-support view of enterprise performance versus budget and forecast, with the ability to drill from group KPIs to division, product line, and region.

## 2. Stakeholders

| Role | Primary questions |
|------|-------------------|
| CEO | Are we on track for revenue, profitability, and strategic growth? |
| CRO | Which commercial motions and regions drive or drag revenue? |
| CTO | Is Technology division EBITDA and uptime healthy? |
| COO | Are operations efficient (margin, headcount, delivery)? |
| CFO | Budget variance, margin trend, forecast reliability |

## 3. Functional requirements

| ID | Requirement | Priority |
|----|-------------|----------|
| BR-01 | Display Actual vs Budget for Revenue, EBITDA, Gross Margin | Must |
| BR-02 | Show Active Customers and YoY-style growth indicator | Must |
| BR-03 | Show Headcount vs Budget and System Uptime vs target | Must |
| BR-04 | Revenue performance by year vs Budget & Forecast | Must |
| BR-05 | Revenue & EBITDA by Division with drill to Product Line | Must |
| BR-06 | EBITDA trend vs Budget by year | Must |
| BR-07 | Gross Margin % monthly trend vs Budget | Must |
| BR-08 | Global revenue distribution by region (map) | Should |
| BR-09 | Filter by Executive Owner (COO / CRO / CTO) | Should |
| BR-10 | Pages: Executive Summary, Regional Performance, Org & Operations | Should |
| BR-11 | Reset filters control | Could |

## 4. Non-functional requirements

- Refresh: daily after finance close window  
- Performance: Executive Summary interactive filters < 3 seconds  
- Security: role-based access; executive owner bookmark views  
- Audit: KPI definitions versioned in data dictionary  

## 5. Scope boundaries

**In scope:** Management P&L KPIs, customers, headcount, uptime, dimensional drill paths.  
**Out of scope (phase 2):** Full statutory consolidation, tax, detailed project P&L, real-time streaming.
