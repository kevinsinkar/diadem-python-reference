---
title: "IRepTable2DColumnBaseInt.Settings"
description: "Specifies the properties of a 2D table column in DIAdem REPORT."
---

# IRepTable2DColumnBaseInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DTableColumn

Specifies the properties of a 2D table column in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
```

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMy2DTable.Position.ByBorder.Top = 30
oMy2DTable.Position.ByBorder.Bottom = 20
oMy2DTable.Position.ByBorder.Left = 20
oMy2DTable.Position.ByBorder.Right = 30
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

*Source: `ReportApi/properties/Report_property_Settings_IRepTable2DColumnBaseInt.htm`*
