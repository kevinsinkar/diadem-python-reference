---
title: "IRepTable2DInt.Position"
description: "Specifies the position of a 2D table in a DIAdem REPORT worksheet."
---

# IRepTable2DInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for 2DTable

Specifies the position of a 2D table in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepTable2DInt.htm`*
