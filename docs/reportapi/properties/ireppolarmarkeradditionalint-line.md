---
title: "IRepPolarMarkerAdditionalInt.Line"
description: "Specifies the properties of a polar curve marker line in DIAdem REPORT."
---

# IRepPolarMarkerAdditionalInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for PolarAdditionalMarker

Specifies the properties of a polar curve marker line in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[5]/[1]"
oMyShape.YChannel.Reference = "[5]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyExtension = oMyShape.Extensions
oMyExtension.Marker.Type = dd.eMarkerCircle
oMyExtension.Marker.Size = 3
oMyExtension.Marker.Repetition.Mode = dd.eMarkerRepetitionEveryNthPoint
oMyExtension.Marker.Repetition.NValue = 50
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

*Source: `ReportApi/properties/Report_property_Line_IRepPolarMarkerAdditionalInt.htm`*
