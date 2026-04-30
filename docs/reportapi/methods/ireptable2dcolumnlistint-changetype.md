---
title: "IRepTable2DColumnListInt.ChangeType"
description: "Changes the data type in the column of a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnListInt.ChangeType

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ChangeType for 2DTableColumns

Changes the data type in the column of a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.ChangeType(Index, NewType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Expression` | 2 | e2DTableColumnExpression |

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
dd.Report.Refresh()
dd.Pause(5)
oMyColumn = oMy2DTable.Columns.ChangeType(1,dd.e2DTableColumnVariable)
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

*Source: `ReportApi/methods/Report_method_ChangeType_IRepTable2DColumnListInt.htm`*
