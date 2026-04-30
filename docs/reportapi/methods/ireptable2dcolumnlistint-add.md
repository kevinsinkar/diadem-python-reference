---
title: "IRepTable2DColumnListInt.Add"
description: "Creates a column in a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for 2DTableColumns

Creates a column in a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(ColumnType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Expression` | 2 | e2DTableColumnExpression |

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMy2DTable.Position.ByBorder.Top = 30
oMy2DTable.Position.ByBorder.Bottom = 20
oMy2DTable.Position.ByBorder.Left = 20
oMy2DTable.Position.ByBorder.Right = 30
oMyCol = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyCol.Channel.Reference = "[1]/[1]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepTable2DColumnListInt.htm`*
