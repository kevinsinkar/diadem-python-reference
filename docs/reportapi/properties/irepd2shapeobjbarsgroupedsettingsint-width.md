---
title: "IRepD2ShapeObjBarsGroupedSettingsInt.Width"
description: "Specifies the width of a bar in the bar group of a curve in the Grouped bars display mode in a 2D axis system in DIAdem REPORT. The percentage refers to the wid"
---

# IRepD2ShapeObjBarsGroupedSettingsInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for 2DGroupedBarsSettings

Specifies the width of a bar in the bar group of a curve in the Grouped bars display mode in a 2D axis system in DIAdem REPORT. The percentage refers to the width of the bar group.

## Signature

```python
obj.Width
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeGroupedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.YChannels.Add("[4]/[3]")

oMySettings = oMy2DCurve.Shape.Settings
oMySettings.BorderLine.LineType = dd.eLineTypeSolid
oMySettings.BorderLine.Color.ColorIndex = dd.eColorIndexDarkRed
oMySettings.Width = 55

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepD2ShapeObjBarsGroupedSettingsInt.htm`*
