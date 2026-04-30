---
title: "IRepTable2DSettingsInt.GridVertical"
description: "Specifies the vertical grid of a 2D table in DIAdem REPORT."
---

# IRepTable2DSettingsInt.GridVertical

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: GridVertical for 2DTableSettings

Specifies the vertical grid of a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.GridVertical
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
oMySettings.UseXDoubleLine = False
oMySettings.UseYDoubleLine = False
oMySettings.BorderLineColor.SetPredefinedColor(dd.ePredefinedColorViolet)
oMyGridHorSettings = oMy2DTable.Settings.GridHorizontal
oMyGridHorSettings.Visible = False
oMyGridVerSettings = oMy2DTable.Settings.GridVertical
oMyGridVerSettings.Visible = False
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

*Source: `ReportApi/properties/Report_property_GridVertical_IRepTable2DSettingsInt.htm`*
