---
title: "IRepTable2DSettingsInt.Palette"
description: "Specifies the palette properties of a 2D table in DIAdem REPORT."
---

# IRepTable2DSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DTableSettings

Specifies the palette properties of a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
dd.Report.NewLayout()
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable, "My2DTable")
oMyPosition = oMyReportObj.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyColumn = oMyReportObj.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[1]"
oMyColumn.Settings.Font.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyReportObj.Settings.Palette
oMyPalette.Count = 10
for i in range( 1, oMyPalette.Count+1):
    oMyPalette(i).Color.SetPredefinedColor(i)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepTable2DSettingsInt.htm`*
