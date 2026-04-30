---
title: "IRepD2ShapeObjBarsHorizontalSettingsInt.DisplayMode"
description: "Specifies the display type of bars in a 2D axis system in the Horizontal bars display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsHorizontalSettingsInt.DisplayMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayMode for 2DBarsHorizontalSettings

Specifies the display type of bars in a 2D axis system in the Horizontal bars display mode in DIAdem REPORT.

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

oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBarsHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"

oMySettings = oMyShape.Settings
oMySettings.DisplayMode = dd.eBarsDisplayMode3D
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexRed)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayMode_IRepD2ShapeObjBarsHorizontalSettingsInt.htm`*
