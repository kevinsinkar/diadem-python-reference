---
title: "IRepTable2DColumnSettingsInt.BackgroundColor"
description: "Specifies the background color of the columns in a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnSettingsInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for 2DTableColumnSettings

Specifies the background color of the columns in a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
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
oMySettings = oMyColumn.Settings
oMySettings.Alignment = dd.eTableAlignmentDecimalPoint
oMySettings.Format = "d.dddd"
oMySettings.BackgroundColor.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepTable2DColumnSettingsInt.htm`*
