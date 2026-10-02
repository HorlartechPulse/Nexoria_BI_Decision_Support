# Dimensional Data Model

## Star schema

```
           DimDate
              │
DimDivision ──┤
     │        │
DimProductLine┤──── FactFinance ──── DimRegion
              │
        DimScenario
```

## Relationships

| Fact column | Dimension | Cardinality |
|-------------|-----------|-------------|
| DateKey | DimDate[DateKey] | Many-to-one |
| DivisionKey | DimDivision[DivisionKey] | Many-to-one |
| ProductLineKey | DimProductLine[ProductLineKey] | Many-to-one |
| RegionKey | DimRegion[RegionKey] | Many-to-one |
| ScenarioKey | DimScenario[ScenarioKey] | Many-to-one |

**Hierarchy:** Division → Product Line (via DimProductLine.DivisionKey).

## Fact grain

One row per **Month × Product Line × Region × Scenario** with additive measures (Revenue, COGS, EBITDA, ActiveCustomers, Headcount) and semi-additive uptime (average).

## Source file

`data/Nexoria_BI_Source.xlsx` — sheets: DimDate, DimDivision, DimProductLine, DimRegion, DimScenario, FactFinance, KPI_Snapshot, Data_Dictionary.
