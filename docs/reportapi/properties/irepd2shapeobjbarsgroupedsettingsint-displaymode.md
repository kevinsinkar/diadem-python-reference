---
title: "IRepD2ShapeObjBarsGroupedSettingsInt.DisplayMode"
description: "Specifies the the display mode of bars in a 2D axis system in the Special combination display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsGroupedSettingsInt.DisplayMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayMode for 2DGroupedBarsSettings

Specifies the the display mode of bars in a 2D axis system in the Special combination display mode in DIAdem REPORT.

## Signature

```python
obj.DisplayMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eBarsDisplayMode2D` | 0 | 2D display |
| `eBarsDisplayMode3D` | 1 | 3D display |

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
oMySettings.DisplayMode = dd.eBarsDisplayMode3D

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayMode_IRepD2ShapeObjBarsGroupedSettingsInt.htm`*
