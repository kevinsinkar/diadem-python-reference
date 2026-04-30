---
title: "IRepD2MarkerAdditionalInt.Size"
description: "Specifies the size of the marker symbols as a percentage of the worksheet in a 2D axis system in DIAdem REPORT."
---

# IRepD2MarkerAdditionalInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for 2DAdditionalMarker

Specifies the size of the marker symbols as a percentage of the worksheet in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Size
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyExtension = oMyShape.Extensions
oMyExtension.Marker.Type = dd.eMarkerCircle
oMyExtension.Marker.Size = 3
oMyExtension.Marker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyExtension.Marker.Repetition.NValue = 20
oMyExtension.Marker.Line.UseCurveColor = False
oMyExtension.Marker.Line.Color.SetPredefinedColor(dd.eColorIndexYellow)
oMyExtension.Marker.Line.Width = dd.eLineWidth0280
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Size_IRepD2MarkerAdditionalInt.htm`*
