---
title: "IRepMarkerFillingInt.Transparency"
description: "Specifies the percentaged transparency of the curve marker filling in a 2D or a 3D axis system in DIAdem REPORT. The value 100 specifies a completely transparen"
---

# IRepMarkerFillingInt.Transparency

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Transparency for MarkerFilling

Specifies the percentaged transparency of the curve marker filling in a 2D or a 3D axis system in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 specifies a completely opaque display.

## Signature

```python
obj.Transparency
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
oMyMarkerFilling.SetPredefinedColor(dd.eColorIndexRed)
oMyMarkerFilling.Transparency = 70
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Transparency_IRepMarkerFillingInt.htm`*
