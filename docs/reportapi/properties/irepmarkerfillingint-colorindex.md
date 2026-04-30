---
title: "IRepMarkerFillingInt.ColorIndex"
description: "Specifies the color of the curve marker filling in a 2D or a 3D axis system in DIAdem REPORT. DIAdem only includes the property ColorIndex if you assign the val"
---

# IRepMarkerFillingInt.ColorIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColorIndex for MarkerFilling

Specifies the color of the curve marker filling in a 2D or a 3D axis system in DIAdem REPORT. DIAdem only includes the property ColorIndex if you assign the value FALSE to the UseCurveColor property.

## Signature

```python
obj.ColorIndex
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorIndexNone` | 0 | None |
| `eColorIndexBlack` | 1 | Black |
| `eColorIndexRed` | 2 | Red |
| `eColorIndexGreen` | 3 | Green |
| `eColorIndexBlue` | 4 | Blue |
| `eColorIndexViolet` | 5 | Violet |
| `eColorIndexTurquoise` | 6 | Turquoise |
| `eColorIndexGrey` | 7 | Gray |
| `eColorIndexYellow` | 8 | Yellow |
| `eColorIndexDarkRed` | 9 | Dark red |
| `eColorIndexDarkGreen` | 10 | Dark green |
| `eColorIndexDarkBlue` | 11 | Dark blue |
| `eColorIndexDarkViolet` | 12 | Dark violet |
| `eColorIndexDarkTurquoise` | 13 | Dark turquoise |
| `eColorIndexDarkGrey` | 14 | Dark gray |
| `eColorIndexDarkYellow` | 15 | Dark yellow |
| `eColorIndexWhite` | 16 | White |
| `eColorIndexOtherColors` | 17 | Other colors |
| `eColorIndexPalette` | 18 | Palette |
| `eColorIndexGlobalColorPalette1` | 19 | Global palette 1 |
| `eColorIndexGlobalColorPalette2` | 20 | Global palette 2 |
| `eColorIndexGlobalColorPalette3` | 21 | Global palette 3 |
| `eColorIndexFillEffects` | 22 | Filling effects |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.ColorIndex = dd.eColorIndexBlue
oMySetting.Line.Width = dd.eLineWidth0100
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyMarker.Repetition.NValue = 20
oMyMarkerFilling = oMyMarker.Filling
oMyMarkerFilling.UseCurveColor = False
oMyMarkerFilling.ColorIndex = dd.eColorIndexRed
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColorIndex_IRepMarkerFillingInt.htm`*
