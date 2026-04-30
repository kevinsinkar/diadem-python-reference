---
title: "IRepTable2DBackgroundColors.AlternatingBackgroundColor"
description: "Specifies the background color that DIAdem uses for every second row in a 2D table. DIAdem draws this background color over possible background colors of the ta"
---

# IRepTable2DBackgroundColors.AlternatingBackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AlternatingBackgroundColor for 2DTableItemBackgroundColor

Specifies the background color that DIAdem uses for every second row in a 2D table. DIAdem draws this background color over possible background colors of the table or rows. Use the setting Filling Effects to plot color shading.

## Signature

```python
return_value = obj.AlternatingBackgroundColor
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
oMyRow = oMy2DTable.Settings.RowBackground
oMyRow.BackgroundColor.ColorIndex = dd.eColorIndexGrey
oMyRow.AlternatingBackgroundColor.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AlternatingBackgroundColor_IRepTable2DBackgroundColors.htm`*
