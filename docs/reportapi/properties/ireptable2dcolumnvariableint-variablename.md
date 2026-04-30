---
title: "IRepTable2DColumnVariableInt.VariableName"
description: "Specifies the variable of which DIAdem REPORT displays the value in a column in a 2D table."
---

# IRepTable2DColumnVariableInt.VariableName

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: VariableName for 2DTableColumnVariable

Specifies the variable of which DIAdem REPORT displays the value in a column in a 2D table.

## Signature

```python
obj.VariableName
```

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnVariable)
oMyColumn.VariableName = "CurrTime"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_VariableName_IRepTable2DColumnVariableInt.htm`*
