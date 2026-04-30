---
title: "IRepMarkerFillingInt.RGB"
description: "Specifies the RGB values of the curve marker filling in a 2D or a 3D axis system in DIAdem REPORT. First assign the value eColorIndexOtherColors to the property"
---

# IRepMarkerFillingInt.RGB

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RGB for MarkerFilling

Specifies the RGB values of the curve marker filling in a 2D or a 3D axis system in DIAdem REPORT. First assign the value eColorIndexOtherColors to the property ColorIndex . You also can use the SetRGBColor method to specify individual colors.

## Signature

```python
obj.RGB
```

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
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyMarker.Repetition.NValue = 20
oMyMarkerFilling = oMyMarker.Filling
oMyMarkerFilling.UseCurveColor = False
oMyMarkerFilling.ColorIndex = dd.eColorIndexOtherColors
oMyMarkerFilling.RGB = dd.RGB(147,33,32)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RGB_IRepMarkerFillingInt.htm`*
