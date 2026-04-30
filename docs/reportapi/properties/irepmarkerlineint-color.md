---
title: "IRepMarkerLineInt.Color"
description: "Specifies the color of the curve marker line in a 2D or a 3D axis system in DIAdem REPORT. DIAdem only includes the property Color if you assign the value FALSE"
---

# IRepMarkerLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for MarkerLine

Specifies the color of the curve marker line in a 2D or a 3D axis system in DIAdem REPORT. DIAdem only includes the property Color if you assign the value FALSE to the UseCurveColor property.

## Signature

```python
return_value = obj.Color
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
oMyMarkerLine = oMyMarker.Line
oMyMarkerLine.UseCurveColor = False
oMyMarkerLine.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyMarkerLine.Width = dd.eLineWidth0100
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepMarkerLineInt.htm`*
