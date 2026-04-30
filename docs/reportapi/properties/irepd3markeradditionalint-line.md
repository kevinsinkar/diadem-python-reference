---
title: "IRepD3MarkerAdditionalInt.Line"
description: "Specifies the properties of the marker lines in the Points display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3MarkerAdditionalInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 3DAdditionalMarker

Specifies the properties of the marker lines in the Points display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapePoints, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyMarker = oMyShape.Settings.Marker
oMyMarker.Type = dd.eMarkerRhombus
oMyMarker.Line.UseCurveColor = False
oMyMarker.Line.Color.ColorIndex = dd.eColorIndexRed
oMyMarker.Filling.UseCurveColor = False
oMyMarker.Filling.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD3MarkerAdditionalInt.htm`*
