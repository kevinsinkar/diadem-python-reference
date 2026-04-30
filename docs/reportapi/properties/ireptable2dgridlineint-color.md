---
title: "IRepTable2DGridLineInt.Color"
description: "Specifies the color of the grid lines of a 2D table in DIAdem REPORT"
---

# IRepTable2DGridLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for 2DTableGridLine

Specifies the color of the grid lines of a 2D table in DIAdem REPORT

## Signature

```python
return_value = obj.Color
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
oMySettings = oMy2DTable.Settings
oMySettings.BorderLineColor.SetPredefinedColor(dd.eColorIndexBlue)
oMyGridHorSettings = oMy2DTable.Settings.GridHorizontal
oMyGridHorSettings.Visible = True
oMyGridHorSettings.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyGridVerSettings = oMy2DTable.Settings.GridVertical
oMyGridVerSettings.Visible = True
oMyGridVerSettings.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepTable2DGridLineInt.htm`*
