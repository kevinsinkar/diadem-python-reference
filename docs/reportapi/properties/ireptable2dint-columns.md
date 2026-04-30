---
title: "IRepTable2DInt.Columns"
description: "Returns a collection of all columns in a 2D table in DIAdem REPORT."
---

# IRepTable2DInt.Columns

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Columns for 2DTable

Returns a collection of all columns in a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.Columns
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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMyColumn.Settings.Alignment = dd.eTableAlignmentDecimalPoint
oMyColumn.Settings.Format = "d.dddd"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Columns_IRepTable2DInt.htm`*
