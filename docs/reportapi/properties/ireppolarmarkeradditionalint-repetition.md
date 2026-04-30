---
title: "IRepPolarMarkerAdditionalInt.Repetition"
description: "Specifies how DIAdem REPORT repeats the markers of a polar curve."
---

# IRepPolarMarkerAdditionalInt.Repetition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Repetition for PolarAdditionalMarker

Specifies how DIAdem REPORT repeats the markers of a polar curve.

## Signature

```python
return_value = obj.Repetition
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
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionEveryNthPoint
oMyMarker.Repetition.NValue = 50
oMyMarker.Line.UseCurveColor = False
oMyMarker.Line.Color.SetPredefinedColor(dd.eColorIndexYellow)
oMyMarker.Line.Width = dd.eLineWidth0280
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Repetition_IRepPolarMarkerAdditionalInt.htm`*
