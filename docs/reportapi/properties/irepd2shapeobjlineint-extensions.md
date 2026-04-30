---
title: "IRepD2ShapeObjLineInt.Extensions"
description: "Specifies the extended properties of a curve in the Line display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjLineInt.Extensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Extensions for 2DLine

Specifies the extended properties of a curve in the Line display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Extensions
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyExtensions = oMyShape.Extensions
oMyExtensions.Marker.Type = dd.eMarkerCircle
oMyExtensions.Marker.Repetition.Mode = dd.eMarkerRepetitionEveryNthPoint
oMyExtensions.Marker.Repetition.NValue = 50
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Extensions_IRepD2ShapeObjLineInt.htm`*
