# Power Query load notes

1. Get Data → Excel → `Nexoria_BI_Source.xlsx`
2. Load DimDate, DimDivision, DimProductLine, DimRegion, DimScenario, FactFinance
3. Set data types: Date as date; keys as Whole Number; money as Decimal
4. Mark DimDate as date table
5. Create relationships as in `docs/03_Dimensional_Model.md`
6. Optional: filter FactFinance to Scenario in report via slicer rather than PQ
