---
title: "IRepD3ShapeObjBarsExtensionsInt.Marker"
description: "Specifies the curve marker properties in the Bars display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObjBarsExtensionsInt.Marker

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Marker for 3DBarsExtensions

Specifies the curve marker properties in the Bars display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Marker
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeBars, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.dd"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 2
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Marker_IRepD3ShapeObjBarsExtensionsInt.htm`*
