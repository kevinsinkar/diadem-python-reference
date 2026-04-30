---
title: "IRepD2ShapeObjBarsSettingsInt.DisplayMode"
description: "Specifies the display type of bars in a 2D axis system in the Bars display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsSettingsInt.DisplayMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayMode for 2DBarsSettings

Specifies the display type of bars in a 2D axis system in the Bars display mode in DIAdem REPORT.

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
dd.DataFileLoad("Example.tdm")
dd.Report.NewLayout()

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"

oMySettings = oMyShape.Settings
oMySettings.DisplayMode = dd.eBarsDisplayMode2D
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayMode_IRepD2ShapeObjBarsSettingsInt.htm`*
